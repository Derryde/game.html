# game.html
developing a game
let lose = numGuesses > 5;
let lose = numGuesses > MAX_GUESSES;
const players = {
  '1': {
    name: '',
    score: 0
  },
  '-1': {
    name: '',
    score: 0
  }
};
// Check for winner
let winner = checkBoardForWinner();
if (winner) return winner;
// There's no winner, so
// check for tie - board still contains null(s)
return board.includes(null) ? null : 'Tie';
function render() {
  renderBoard();
  renderScores();
  renderControls();
  renderMessages();
}
function handleMove(evt) {
  // Check if we should exit the function
  // according to the current state
  // For example, ignore clicks if the
  // game has been won or is a tie:
  if (winner) return;
  // Logic/Code to update all impacted state
  ...
  // Visualize all state
  render();
}
<script defer src="js/main.js"></script>
