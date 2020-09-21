# Storag in HTML
HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.

# How to check for HTML 5 storage
function supports_html5_storage() {

  try {

    return 'localStorage' in window && window['localStorage'] !== null;

  } catch (e) {

    return false;

  }
}

**Note:Instead of writing this function yourself, you can use Modernizr to detect support for HTML5 Storage.**

if (Modernizr.localstorage) {

  // window.localStorage is available!

} else {

  // no native support for HTML5 storage :(

  // maybe try dojox.storage or a third-party solution

}

# HTML5 STORAGE IN ACTION

Every time a change occurs within the game, we call this function:

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


