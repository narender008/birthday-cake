# birthday-cake

**Cake Party** is a birthday-cake cutting game for a two-year-old, played on a laptop. Four animal friends sit at a party table. She picks a cake, a present pops open, she blows out the candles, and every press cuts a slice while a friend sings the next line of Happy Birthday. The slice flies to whoever just sang, and they eat it: nom nom nom.

It is one HTML file. It runs offline, with no network, no ads, no tracking and no accounts.

## Open it

1. Download or clone this repository.
2. Double-click `index.html`. It opens in your browser from the file, with no server and no install.

Chrome or Edge works best: there the keyboard is locked in full screen, so shortcuts such as ⌘W or Ctrl+W can't close the game. Safari and Firefox work too, but a single Esc leaves full screen there.

## How to play (for grown-ups)

Turn the sound on. Any key, click, tap or big mouse wiggle is "a press". There is nothing to aim at, nothing to read and no way to lose.

1. **Pick a cake.** Three different cakes bounce in turn. A click picks the one clicked; any key picks the one that is bouncing. The first press also turns on sound and full screen.
2. **Peek-a-boo.** The cake hops onto the stand and a giggling present drops over it. A press pops the lid off and the cake jumps out.
3. **Candles.** A press blows them out; the friends cheer.
4. **Cut and sing.** Each press cuts a slice while the next friend sings the next line in its own voice (bear, bunny, kitty, then everyone). Line 3 holds on "dear…" so you can sing the name.
5. **Party.** After the last slice: confetti and a hooray, then three new cakes.
6. **Bye-bye.** After 3 cakes (you can change this) the friends wave, the room dims and everyone sleeps. Use "Start a new party" in the parent corner, or reload the page, to play again.

Extras: stars appear where each key sits on the keyboard, sparkles follow the mouse, and the cake wiggles if nothing happens for a while. Every cake is a new mix of inside, frosting colour and style, topping and fruit, and now and then a piñata cake spills candies on the first cut.

**To leave:** hold **Esc** for 2 seconds.

## Parent corner

Hold the **top-left corner** of the screen for 3 seconds (a ring fills up), or press **Ctrl+Shift+P**. There you can set:

- cakes before bye-bye (1 to 5, default 3);
- slices per cake: 4 (a whole line of the song per cut) or 8 (half a line per cut);
- which cake insides she can pick from;
- volume, and calm mode (fewer sparkles, smaller bounces);
- optional personal touches: a name, shown on a sign on the cake and a tag on the present, and a birthday, which adds a big number balloon during the birthday week.

Settings are saved in this browser's local storage on this laptop only. They are never sent anywhere and never go into this repository. "Forget name and birthday" clears them.

## Tips

- On a Mac, turn off trackpad "Swipe between pages" and Hot Corners on the laptop she uses.
- Keep the volume modest; the game already caps it.

## For developers

Everything is in `index.html`: a 2.5D canvas drawing, synthesised sounds (Web Audio) and no libraries. The code checks itself with `console.assert` on load (the cut order, that every visible cut face shows its layers, the settings cleaner and the birthday-week maths), so an open console that stays empty means the checks passed. Set `CHOIR = false` near the top to have a music box play the song instead of the friends singing.
