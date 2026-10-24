# Juicy Merge

A drop-and-merge fruit puzzle that runs in the browser. It is a single `index.html` with no build step and no assets: the art is drawn on a canvas, and the music and sound effects are synthesized with Web Audio.

- Drop fruit. Two of the same fruit merge into the next one. There are 14 fruits, from Cherry up to Golden Melon.
- **Timed**: choose a 1, 2 or 3 minute start. Every merge adds time, and each length keeps its own best score.
- **Endless**: no timer. The game ends if fruit stays above the dashed line for 3 seconds.
- Merges in quick succession build combos with a score multiplier.
- Choose a **difficulty** (Easy, Normal or Hard: pieces are 1.2×, 1.4× or 1.6× the base size), a **mode**, and for Timed a **time**, then press **START**. Each combination keeps its own best score.

- **Battle** (2 players, online): one player presses **Create room** and shares the 4-letter code, and the other types it in and presses **Join**. Every merge from Lemon up drops rocks into the opponent's box (bigger fruit and combos send more; a Golden Burst sends 8). After a short warning the rocks fall. Rocks never merge: to smash one, make a merge with a fruit that is touching it (+10 points). Your own merges cancel rocks that are still on their way to you. The first player to overflow loses. A mini view of the opponent's box sits in the HUD. Battles can't be paused, and both players play at the host's difficulty. The connection is peer-to-peer (WebRTC through the free PeerJS broker), so no server is needed, but both players must be online.

Controls: tap or drag to aim, then release to drop. On desktop you can also use the mouse, or the arrow keys and Space. P or Esc pauses.

Play locally by opening `index.html` in a browser.
