# Judge Duel

A multiplayer game for 2 to 8 players where you act like an LLM response evaluator. Every round shows a prompt and two AI answers. Pick the one a careful rater would prefer, and race your friends.

**Live game:** https://naveedakhtar-88.github.io/judge-duel/

## How to play

1. Open the live link and type your name.
2. Press Create a room, or enter a friend's code and press Join.
3. The host presses Start game when everyone is in.
4. Each round, read the prompt and choose Response A or Response B. Think accuracy, following the instruction, safety and tone.
5. A matching pick scores 100 points plus up to 50 for speed. After the reveal you see the reason. 8 rounds, highest score wins.

## How it works

- Single HTML file, no build step and no server of my own.
- Players connect directly to each other with WebRTC through PeerJS. The room code is the host's peer id.
- The host keeps the game state, scores answers and sends the shared view to every player.
- A bank of 13 prompt pairs covers accuracy, instruction following, tone, safety, faithfulness and audience fit. Sides are shuffled every game.

## Tech

HTML, CSS, JavaScript, PeerJS (WebRTC), GitHub Pages.

## Author

Naveed Akhtar. Portfolio: https://naveedakhtar-88.github.io/
