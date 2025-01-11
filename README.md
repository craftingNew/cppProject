
# <p align="center"> Tic-Tac-Toe Artificial Intelligence :joystick: </p>

<p align="center">
  <img src="assets/ai-demo.gif" alt="AI Demo">
</p>

## Minimax Algorithm 

1. Considers all potential board layouts that could result from its moves and your responses, like a branching tree of possibilities.
2. Assigns a score to each possible end state (win, loss, or tie). It aims to choose moves leading to the highest-scoring branches (wins for the AI).
3. When it's your turn, the AI assumes you'll make the smartest move against it. It aims to pick moves that force the lowest score on you.

## Alpha-Beta Pruning

**1. Best and Worst Guarantees:**
* **Alpha:** *The best (highest) score the AI can achieve, regardless of your moves, for a given branch of moves.*
* **Beta:** *The worst (lowest) score the AI can force you into, for a given branch of moves.*
  
**2. Smart Pruning:** If the AI ever sees a branch guaranteed to be worse than its current 'Beta' (meaning you found a better move against it), it discards that whole branch without further analysis - saving lots of time! The same logic with 'Alpha' discards poor choices for you.
