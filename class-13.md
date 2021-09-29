# Local Storage 

Historically, web applications have had limited resources for data storage. Cookies are a type of data storage that were created early on but only provided minimal data storage solutions. Also, cookies can slow down a program. Therefore, web applications need a lot of storage space on the client that persists beyond a page refresh and isn't transmitted to a server.

Before HTML5 and many current modern browsers there were attempts to solve this issue. Microsoft created UserData and Adobe created Flash, each allowing up to 100kbs of local storage. The key take away is that each offered a different solution but was was really needed was a standard approach across all browsers. HTML5 has sought a way to standardize an API that is implemented natively and is consistent across multiple browsers without third-party plugins.

HTML5 storage is a way for web pages to store named key/value pairs locally and within the client web browser. This data presists and is never transmitted to a remote web server. You can access HTML5 Storage through a local storage object on the global `window` object. You can access it in one of two ways.

```js
//first example to access
function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}
//second example uses Modernizr
if (Modernizr.localstorage) {
  // window.localStorage is available!
} else {
  // no native support for HTML5 storage :(
  // maybe try dojox.storage or a third-party solution
}
```

Data is stored on named key/value pairs. The data is held by the named key. You can retrieve that daa with the same key and the named key is a string. The data can be any type supported by JavaScript but all data is actually stored as a string. So once you access it you may need to convert it.

You can access this information using `getItem()` and chang it using `setItem()`. Or, use other methods such as storing the reference in a variable and accessing via bracket notation.

You can also keep track of when the HTML5 storage area has changed. The storage event is supported everywhere the localStorage object is supported via the window object.

```js
if (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};
```

Currently we only have access to 5 megabytes of storage and is pretty consistent across browsers currently. If you are storing integers and floats, this data adds up quicker than if you stored strings. Be aware of using this approach and how it may impact usage.

The localStorage object can help save information presented on a screen. The best example of this would be  a game that runs a function every time a change occurs on the window object. The function takes the revised data and stores it allowing the browser to recall that information if it is refreshed or closed and reopened.

```js

//save progress
function saveGameState() {
    if (!supportsLocalStorage()) { return false; }
    localStorage["halma.game.in.progress"] = gGameInProgress;
    for (var i = 0; i < kNumPieces; i++) {
	localStorage["halma.piece." + i + ".row"] = gPieces[i].row;
	localStorage["halma.piece." + i + ".column"] = gPieces[i].column;
    }
    localStorage["halma.selectedpiece"] = gSelectedPieceIndex;
    localStorage["halma.selectedpiecehasmoved"] = gSelectedPieceHasMoved;
    localStorage["halma.movecount"] = gMoveCount;
    return true;
}

//resumes game
function resumeGame() {
    if (!supportsLocalStorage()) { return false; }
    gGameInProgress = (localStorage["halma.game.in.progress"] == "true");
    if (!gGameInProgress) { return false; }
    gPieces = new Array(kNumPieces);
    for (var i = 0; i < kNumPieces; i++) {
	var row = parseInt(localStorage["halma.piece." + i + ".row"]);
	var column = parseInt(localStorage["halma.piece." + i + ".column"]);
	gPieces[i] = new Cell(row, column);
    }
    gNumPieces = kNumPieces;
    gSelectedPieceIndex = parseInt(localStorage["halma.selectedpiece"]);
    gSelectedPieceHasMoved = localStorage["halma.selectedpiecehasmoved"] == "true";
    gMoveCount = parseInt(localStorage["halma.movecount"]);
    drawBoard();
    return true;
}
```

Using additional storage is an option and can be implemented using SQL. There are many flavors of SQLite is something that Google launched in 2007. There are a few variations and most of which I am unfamiliar with at this point but I am eager to better understand them.


[Back to TOC](README.md)