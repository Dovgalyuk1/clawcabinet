# CLAW — every meme is in the box, the claw is weak

Static one-page site. No build step: `index.html` + `assets/`.

## The idea
One coin buys one grab at a cabinet stuffed with every meme plush. Grip strength is rolled on
chain for every attempt and it is mostly terrible: the claw lifts the prize, carries it halfway
and lets go. Every coin fed in goes into the pot under the glass (minus a slice that burns),
everything the claw drops stays in the box, and whoever finally gets one all the way to the
chute takes the whole pot. Then a new plush drops in and the pot starts from zero.

## The game — THE CABINET
Two skill checks and one honest coin flip:
1. **Aim** — drag the claw (or ← →) over the plush you want.
2. **Grip** — after it descends, stop a fast oscillating meter; final grip = 62% meter + 38% aim accuracy.
3. **Three slip rolls** — on the lift, halfway across the box and right over the chute. Even a
   perfect grip gets out about two times in three; a sloppy one almost never does.

Eight prizes fill the shelf. Nine plushes are in the box — THE GUY at the back has never been
carried out and stays there as flavour.

## Assets
Cut from the single render Oleh sent: `assets/machine.webp` (whole cabinet) and
`assets/p-*.webp` (nine plushes: pepe, shiba, cat, bunny, penguin, hood, fox, smiley, wojak).
Background removed by flood-filling the cream from the image border (so the white cat's white
body survives), then per-plush elliptical masks + fill-holes, largest component.

## Sound
Coin-in jingle, servo whirr, claw clank, a descending sad tone on every slip, five-note win
fanfare; music is an arcade attract-mode chiptune loop (square lead + triangle bass + hats).

## Settings
```js
window.CONTRACT = "";   // contract address
window.TWITTER  = "";   // X link
window.BUY_URL  = "";   // buy link — BUY stays greyed out while empty
```
