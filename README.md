# Filler_42

Filler is the one of the two algorithm projects you get to choose to do after completing ft_printf. The other is Push_Swap.

Filler is a rather simple and fun project. The official subject summarizes it as follows:
"Create your player to fight other students on the world famous Filler board. The concept is simple: two players earn points by placing tiles on a board one after the other. Each tile is randomly generated by the Game Master, in the form of a Ruby program. The game ends when no more tile can be placed."

Filler is one big parser with an added layer of algorithm on top.

In order to beat my opponent, I've opted for a circling strategy. To do that, at every turn, I initialize a heatmap version of the board in order to always know how far and in what direction my opponent is from me. With that information I then proceed to place the tile that was given to me as the close as possible to my enemie's position in order to surround him when we finally meet on the board.

Each tile may be placed on the board if only ONE of its elements is in contact with only ONE element of one of our previously place tiles.
The jist of it resides in a simple anchor-point manipulation in order to check for each possibly correct coordinate (board_Y; board_X) if all relative ones are also valid. (Tile_Y_of_Element1; Tile_X_of_e1), (Tile_Y_e2; Tile_X_e2) and so on.

