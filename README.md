# pythonChessAnalyzer 

Analyses games and positions. Possible to have a Game Report similar to the one from chess.com, including graphs.

## Requirements

You need chess and plotly(and everything that plotly needs).
```bash
pip install chess
pip install plotly
```

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pythonChessAnalyzer.

```bash
pip install chessAnalyzer
```

## Usage

```python
import os, chessAnalyzer, chessAnalyzer.main

# Always use a string for file paths!

ca = chessAnalyzer.main.AnnotatePosition(0.5, os.getcwd(), <engine file path(string)>)

ca.graph(pgn_loc, end_loc) # creates a graph
annotated_pgn = ca.annotate_game(pgn_loc) # annotates game
white_lost_positions: list, black_lost_positions: list, annotated game: list = ca.game_report(pgn_loc, annotate=True) # gets you a game report(saves graph elsewhere)
# and more!
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
[MIT](https://choosealicense.com/licenses/mit/)
