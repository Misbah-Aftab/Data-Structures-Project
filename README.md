# Scrabble Game in C++ (Using SFML-library)
This project is a simple and fun version of the classic Scrabble game, made using C++ and the SFML library. It’s a two-player game where players take turns making words to score points, just like the original board game.

## Gameplay:
### 1-Main Menu Interface:
   •	Upon loading the game, a user-friendly menu is displayed with options to either "Play Game" or "Quit Game." Choosing "Play Game" starts the match. Each player draws seven tiles from the bag.
  
   •	The first player places a word on the center square of the board, covering it completely. This word must be at least two letters long.


### 2-Turn Based Gameplay:
   •	Players take turns to make words. 
  
   •	New words must connect to existing words on the board. 
  
   •	Words can be formed horizontally or vertically, but not diagonally. 
  
   •	Players use tiles from their rack to form words. 
  
   •	Each correct word increases the player’s score, while an invalid word triggers a message indicating that the word is not valid.
  
   •	 If a player can't make a word, they can Pass their turn.



### 3-Skip Turn Mechanism:
   •	Players may choose to skip their turn. 
  
   •	However, if a player skips their turn three consecutive times, they automatically lose the game, and the opposing player is declared the winner. This feature adds strategic depth to the gameplay.

### 4-Surrender Option:
   •	A player can give up at any time by selecting the surrender option, making the opponent the winner.

### 5-Tile Bag System:
   •	The game includes a tile bag that shows how many tiles are left.
  
   •	 As players use tiles, the number decreases, helping them track the game’s progress.

### 6-How the Game Ends:
   ⦁ The game ends when all tiles are used, or all possible words are made on the board,   leaving no moves or tiles. The player with the higher score wins.
  
   ⦁	If a player skips their turn three times in a row, they lose the game.

   ⦁	A player can also win if their opponent surrenders.

## DSA Concepts Used in This Game:

  1. Trie(Prefix Tree): Used in: TrieDictionary class Purpose: Efficiently stores and looks up valid words by allowing fast prefix matching.

  2. HashMap/Dictionary: Used in: TileBag, Player classes Purpose: Stores and retrieves tiles in the bag and the tiles a player holds, enabling quick access.

  3. Vector(Dynamic Array): Used in: Player, TileBag, Game classes  Purpose: Dynamically stores data like player tiles, remaining tiles in the bag, and the list of players in the game.

  4. Tree Traversal(for Valid Word Search): Used in: TrieDictionary class  Purpose: Traverses the Trie to check if a word is valid by exploring all possible prefixes.

  5. Recursion: Used in: Board class Purpose: Used in backtracking to recursively check and validate word placements on the board.


