🚀 EOTHello - Enhanced Othello AI Game
[ [ [

A professional implementation of the classic Othello (Reversi) board game in Python, featuring a powerful Minimax with Alpha-Beta Pruning AI opponent. Built as a Jupyter Notebook for easy experimentation, simulation, and visualization. Supports 8x8 board, valid move detection, flipping mechanics, scoring, and full gameplay automation.
​

✨ Features
Initial Board Setup: Standard 8x8 Othello starting position (3,3 & 4,4 White; 3,4 & 4,3 Black).

Valid Moves Detection: Identifies all legal moves by checking opponent flips in 8 directions.

Move Application: Automatically flips opponent discs during placement.

Evaluation Function: Simple score-based heuristic (Black: +1, White: -1).

Minimax AI (Depth 4+): Alpha-Beta optimized for efficient decision-making; unbeatable against casual play.

Game Loop: Human vs. AI or full AI simulation with board printing.

Game Over Detection: Checks no valid moves for both players.

GUI Extension: Basic Tkinter prototype for interactive play (in development).

📊 Demo Output
text
  0 1 2 3 4 5 6 7
0 . . . . . . . .
1 . . . . . . . .
2 . . . . . . . .
3 . . . W B . . .
4 . . . B W . . .
5 . . . . . . . .
6 . . . . . . . .
7 . . . . . . . .
AI computes optimal moves like (2,3) or (3,2) for strategic advantage.
​

🛠️ Tech Stack
Component	Description
Language	Python 3.12
Environment	Jupyter Notebook
Algorithms	Minimax + Alpha-Beta Pruning
Data Structures	2D Lists for Board
Libraries	None (Pure Python) + Tkinter (GUI)
🚀 Quick Start
Clone the repo:

text
git clone https://github.com/yourusername/eothello.git
cd eothello
Run the notebook:

text
jupyter notebook eothello.ipynb
Execute cells sequentially to play! Use playgame() for full simulation.
​

🔍 Usage Examples
python
# Initialize board
board = initial_board()

# Print board
print_board(board)

# Get valid moves for Black
valid_moves(board, BLACK)

# AI best move (White's turn)
best_score, best_move = minimax_ab(board, depth=4, alpha=-float('inf'), beta=float('inf'), maximizing_player=True, player=WHITE)

# Play full game
play_game()
📈 Performance
AI Depth: Configurable up to 4 (balances speed/strength).

Move Generation: O(1) per direction check.

Scalability: Easily extend to deeper searches or advanced heuristics (e.g., mobility, corners).

🤝 Contributing
Fork the repo.

Create a feature branch (git checkout -b feature/amazing-feature).

Commit changes (git commit -m 'Add amazing feature').

Push (git push origin feature/amazing-feature).

Open a Pull Request!

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgments
Inspired by classic Othello rules.

Thanks to Jupyter for interactive development!

⭐ Star this repo if you find it useful! Questions? Open an issue.
​
