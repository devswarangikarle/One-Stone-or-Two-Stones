# One-Stone-or-Two-Stones

Raj and Ritu are playing a game. There are two piles numbered 1 and 2. Pile 1 contains X stones while Pile 2 contains Y stones. Raj starts the game.
In his turn, Raj can either remove 1 stone each from both the piles or remove 2 stones from pile 1.
On the other hand, Ritu, in her turn, can either remove 1 stone each from both the piles or remove 2 stones from pile 2.
The player who cannot make a move loses. Determine the winner if both players play optimally?

def find_winner(X, Y):

    if X > Y:
        return "Raj"
    else:
        return "Ritu"

t = int(input())
for _ in range(t):

    X, Y = map(int, input().split())
    print(find_winner(X, Y))
