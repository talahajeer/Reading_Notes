# Local Storage

## Introduction to HTML5 storage
 It’s a way for web pages to store named key/value pairs locally, within the client web browser.
 <br>
 Similarity with cookies:
  This data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you.
 <br>
 Defferance from cookies:
  This data is never transmitted to the remote web server.
  <br>
 Check if your browser supports HTML5 storage

  function supports_html5_storage() {
      <br>
  try {
      <br>
    return 'localStorage' in window && window\['localStorage'\] !== null;
    <br>
  } catch (e) {
      <br>
    return false;
    <br>
  }
  <br>
 }

## When do we use the HTML5 storage?
 Imagin you are playing a game on a browser and you by mistake closed it.If your browser doesnt support localstorage then you will lose your progress in the game. But if your browser does support the localstorage it will save whether there is a game in progress.
 hen you reopen the game agian we call this fuction bellow to see if you have opened this before and what is your progress function resumeGame() {
  <br>
    if (!supportsLocalStorage()) { return false; }
    <br>
    gGameInProgress = (localStorage["halma.game.in.progress"] == "true");
   <br>
    if (!gGameInProgress) { return false; }
   <br>
    gPieces = new Array(kNumPieces);
    <br>
    for (var i = 0; i < kNumPieces; i++) {
	 <br>
   var row = parseInt(localStorage["halma.piece." + i + ".row"]);
	<be>
   var column = parseInt(localStorage["halma.piece." + i + ".column"]);
  <br>	
  gPieces[i] = new Cell(row, column);
   <br>
    }
    <br>
    gNumPieces = kNumPieces;
    <br>
    gSelectedPieceIndex = parseInt(localStorage["halma.selectedpiece"]);
    <br>
    gSelectedPieceHasMoved = localStorage["halma.selectedpiecehasmoved"] == "true";
    <br>
    gMoveCount = parseInt(localStorage["halma.movecount"]);
    <br>
    drawBoard();
    <br>
    return true;
<br>
}