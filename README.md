Quantum Poker

Our team decided to pursue the Microsoft/IonQ challenge of game-making, with the idea to create something that can be used instructively and that would foster an appreciation for the expressibility of quantum computing. We settled on the concept of a multiplayer game where players build a circuit that reproduces an ideal quantum state, with the hope that upon measurement, the measured bitstring matches a goal bitstring.
Players start with a 6-qubit circuit initialised in the zero states, and are given three random gates or cards that they can choose to apply each round. Each turn, the players may choose to apply any number of gates from their hand either to any bit in their own circuit, or to any bit in an opponent's circuit, in an effort of sabotage. After the player’s turn is ended, gates are drawn from the randomised deck to maintain 3 cards in their hand. The game ends once the gate deck is empty and the last player has gone, after which measurements are taken of each player’s circuit. The similarity of the player’s measured bitstring with the goal bitstring is calculated by the game, and the player whose bitstring is closest to the goal bitstring wins. Gates are chosen via QRNG or classical randomness, as QNRG may take some time.
Some game details:
Players cannot see other players’ circuits 
Players can specify the qubit(s) which gates are to be applied to
Players can apply gates to other players’ qubits

How to play Quantum Poker:

1.Once the program is run from the game.ipynb file, you will play the game in the terminal.

2.You are first prompted to enter the number of players. Input the amount and press enter to start playing the game. You may have up to six players in a game.

3.After this, the goal bitstring is announced. Players must apply gates to their own circuits to get as close to this bitstring as possible.

4.Player one is the first to start the round, and is presented with their live circuit updated in real time and the three gates in their hand.

5.The player is then asked the number of cards they wish to play. To apply a gate from their hand to one of their own bits, the player is prompted to enter the gate which they want to apply (‘x’: X, ‘y’: Y, ‘z’: Z, ‘h’: H, ‘c’: CNOT, ‘s’: S or ‘t’: T), followed by the player whose bits they want to apply it to, and the target bit. If the gate is a CNOT operation, they must additionally enter it. 

6.Once a player has applied the number of gates expressed, their turn is ended and the game is passed to the next player.  

7.The player can choose to apply one to all of their gates, or can choose not to apply any gates, by entering zero as the amount of cards they wish to play. 

8.The game is passed from player to player, until all the cards in the deck are exhausted. At this point, each player’s circuit is measured, similarity scores are calculated, and the winner is announced. 

Find our presentation here! 

