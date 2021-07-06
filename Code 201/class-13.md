# HTML5 Local Storage
- HTML5 storage is web storage
  - aka DOM storage
- way for web pages to store named key/value pairs locally
  - in the client's web browser (like cookies)
- data persists after you navigate away from that web page, close the tab, or exit the browser
- unlike cookies, the data isn't sent to a remote web server
- it is implemented natively in web browsers
- check for HTML5 storage
```js
function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}
```
- using HTML5 storage
  - data being stored can be of any type: string, Boolean, number, etc
  - data actually stored as a string
- HTML5 storage in action
  - saving game data
  ```js
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
  ```
  - resume game data
  ```js
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
