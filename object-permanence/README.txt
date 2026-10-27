OBJECT PERMANENCE  -  how to run it and change it

PUT IT ON GITHUB
  Copy this whole "object-permanence" folder into your course repo (replace the old one), commit, push.
  It is the same address as before:  .../object-permanence/   Hard refresh after it publishes (Cmd+Shift+R).

PREVIEW ON YOUR COMPUTER (optional)
  Terminal, in this folder:   python3 serve.py      then open http://localhost:8000   (headphones)
  Double-clicking index.html will NOT play sound. The browser blocks it.

HOW IT WORKS
  The picture is pinned. Scroll, and the text cards move up over it. The sounds follow the picture.
  After the flea market, the apartment sounds are gone for good. Scroll back up and you still see the rooms,
  but they stay silent except for the street. Reload the page to hear the first half again.

YOUR TEXT, ORDER AND LENGTH
  Open index.html in a text editor. The "STEPS" table near the top is the whole piece:
    text:"..."   the card(s) of words on that picture (a list = several cards)
    h:           how long that chapter lasts, in screen heights (bigger = more scrolling)
  Move a line to move a picture. Delete a line to cut one.

THE RETURN PICTURE
  The last picture before the black is photos/portrait.jpg (the feather bird beside the old portrait). To use a
  different one, change that one path in the STEPS table. The emptied wide room is no longer needed.

LINDA'S VOICE
  audio/linda_voice.mp3 plays once after "I could almost hear her." The other sounds drop 10 dB while she speaks
  (DUCK_DB near the top of the script) and come back when she finishes. The market cut stops her if the visitor
  scrolls past it. Her file is unchanged; the Linda slider in the mixer (press M) sets her level.

THE MARKET FILM
  It sits after the three market photos, plays once (60 seconds), then cuts to black. Scrolling away early stops it;
  coming back plays it again from the start. Its chapter length is the "h:" on the line  { video: "market" }.

THE OTHER ENDING
  Add  ?ending=room  to the web address. The room tone comes back over black instead of the street fading out.

TUNE THE LEVELS BY EAR
  Press M on the page. Sliders are in dB on top of your files (0 = exactly as you made them).
  "Copy mix" copies your settings so you can send them to me. "Jump to" scrolls to any chapter.
  The door sound starts DOOR_DELAY seconds (now 1.0) after the door film starts moving. Try other values without
  editing: add  ?door=1.5  to the web address (bigger = later). Once you like it, set DOOR_DELAY to that number.

YOUR AUDIO FILES ARE UNCHANGED
  Everything in audio/ is byte-for-byte what you exported from Premiere.

THE FILMS
  video/door.* and video/flea_market.* are muted clips. The door is cut from a screen recording of stock footage:
  fine for class, but license or replace it before the page is public. (The objects film and the VHS table photo
  are no longer in the sequence, so they are not in this folder.)
