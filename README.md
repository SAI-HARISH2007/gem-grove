# Gem Grove — an HTML5 playable ad

**Play it:** https://sai-harish2007.github.io/gem-grove/

A match-3 playable ad in a single HTML file: no libraries, no build step, HTML5 Canvas only.
Built as a portfolio piece demonstrating the anatomy of a playable:

1. **The 3-second hook** — an animated hand shows a winning swap before the player has to think.
2. **One mechanic** — drag or tap-tap to swap adjacent gems; 3+ in a row pops, gems fall, cascades multiply the score.
3. **Pressure** — 12 moves to reach 600 points, with a live progress bar.
4. **The end card** — win or lose, the session ends on a pulsing CTA ("PLAY FREE") and a replay option.

## Details

- 6×6 board, 5 gem colors, radial-gradient gems with specular highlights drawn per frame on Canvas.
- Smooth-step swap animation, revert on invalid swap (no move spent), gravity with acceleration on refill, cascade multipliers with floating score text, particle bursts on every match, confetti on the win screen.
- Boards are generated without starting matches and reshuffled if no valid move exists.
- Mouse and touch input; responsive layout sized for portrait phones.
- ~450 lines in one `index.html`. Open it in a browser — that's the whole deployment.

Built in one evening with Claude Code, by Sai Haresh Anand S. All rendering and game
logic is hand-rolled Canvas 2D; the gem art is procedural (gradients), so the file has
zero asset dependencies.
