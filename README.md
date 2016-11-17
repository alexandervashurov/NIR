\documentclass[12pt]{article}  

\title{The game Othello using Monte Carlo}  
\date{}  
\author{Vashurov Alexander}

\begin{document}  
  \maketitle  
\section{Introduction}
	This paper deals with the construction of an AI player to play the game Othello. A lot of techniques are already known to let AI players play the game Othello. We will not try to improve on these techniques, but to use a completely different and very simple approach to play the game.
\subsection{Artificial Intelligence}
	In this section, we will give some information about Artificial Intelligence. On the second Dartmouth Conference in 1956, organized by John MeCerthy, the name "Artificial Intelligence" was used first time. The first work in AI however started more than 10 years before the Dartmouth conference and was done by War- ren McCulloch and Walter Pitts in 1943. Chess was tackled by Konrad Zuse, Claude Shannon, Norbert Wiener and Alan Turing already in 1950. In 1956, a checkers was demonstrated by Arthur Samuel to be able to play at a strong amateur level.
\subsection{Beginning of the game}
	In our research, we consider the game Othello. This game was introduced in 1975. Few years later the game has changed its name to Reversi. This game got a lot of popularity in England in 1898.
\subsection{AI Othello}
In this paper, we developed an AI player that is capable of playing the game Othello. The human world champions were beaten by the best AI Othello players. We did not try to improve on the existing techniques, but investigated a different approach to play Othello. This different approach is the Monte Carlo algorithm. An advantage of the Monte Carlo algorithm is that it is fast and does not use any domain knowledge.
\subsection{Algorithm}
The Monte Carlo algorithm has many applications, also in the game field. For example, the algorithm has been used to play the game Go. Go is a very complex game that is very hard to tackle in AI.
\section{The Game Othello}
    This section describes the game Othello. First, we will give the rules of the game. Next we will show some strategies that are commonly known to stronger players.
\subsection{The rules}
    For the specific game of Othello, the rules state that the game begins with four disks placed in a square in the middle of the grid, two facing white side up, two pieces with the dark side up, with same-colored disks on a diagonal with each other. Convention has initial board position such that the disks with dark side up are to the north-east and south-west, though this is only marginally meaningful to play. If the disks with dark side up are to the north-west and south-east, the board may be rotated by 90° clockwise or counterclockwise. The dark player moves first.\\
	Dark must place a piece with the dark side up on the board, in such a position that there exists at least one straight occupied line between the new piece and another dark piece, with one or more contiguous light pieces between them.\\
	After placing the piece, dark turns over all light pieces lying on a straight line between the new piece and any anchoring dark pieces. All reversed pieces now show the dark side, and dark can use them in later moves—unless light has reversed them back in the meantime. In other words, a valid move is one where at least one piece is reversed.\\
	If a player cannot make a legal move, he has to pass. If both players have to pass, the game is over. The player who has the most discs with his color flipped up, wins the game.
\subsection{Strategies}
Othello is considered to be a game that is ‘a minute to learn, a lifetime to master’. This slogan accurately captures the game, because the rules of the game are very simple, but playing the game well is very difficult.
\subsubsection{Openings}
For relatively inexperienced players the opening part of a game of Othello is generally not very easy to make sense of. A rule of thumb on the opening is that a good opening is one that leads to a good middle-game. By and large, good moves in the very earliest stages are determined by whether there is a refutation to a move only and few other truly general considerations aside from what exactly constitutes a refutation. The first move by dark is no choice at all other than for the purpose of the player's possible sense of ideal visualization. The first move by light gives three choices, and it is generally accepted at the highest level that one of these actually may be successfully refuted, that being what is known as the Parallel opening. The other two choices by light are called the Diagonal opening and the Perpendicular opening.
\subsubsection{Corners}
Corner positions remain immune to flipping for the rest of the game, being termini of horizontal, vertical and diagonal lines. More generally, a piece is stable when, along all four axes, it is in terminal position or if from it along the axis one reaches a terminal disk passing only through disks the same color. These are not the only kinds of stable disk, however, and occupying a corner may often be a grave error if one allows one's opponent to create a wedge that results in him or her gathering more stable disks. This can render occupying the corner largely useless, and often much worse than that because of loss of tempo.
\subsubsection{Mobility}
An opponent playing with reasonable strategy will not so easily relinquish the corner or any other good moves. So to achieve these good moves, a player must force its opponent to play moves that relinquish those good moves. One of the ways to achieve this involves reducing the number of moves available to the player's opponent. Ideally, this will eventually force the opponent to make an undesirable move.
\subsubsection{Edges}
Edge pieces can anchor flips that influence moves to all regions of the board. If played poorly, this can poison later moves by causing players to flip too many pieces and open up many moves for the opponent. However, playing on edges where an opponent can not easily respond drastically reduces possible moves for that opponent.\\
 	The square immediately diagonally adjacent to the corner, when played in the early or middle game, typically guarantees the loss of that corner. Nevertheless, such a corner sacrifice is sometimes played for some strategic purpose. Playing to the edge squares adjacent to the corner can also be dangerous if it gives the opponent powerful forcing moves.
\subsubsection{End-game}
For the end-game the strategies will typically change. Special techniques such as sweeping, gaining access, and the details of move order can have a large impact on the outcome of the game. Actual counting of disks in the very final stages is often critical, but sometimes in human play an inaccurate choice, for disk differential can be better than an accurate one in terms of the expected outcome.
\section{The Monte Carlo Algorithm}
\end{document}
