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

THE EMPTIED ROOM (Photoshop)
  Save it as  photos/wide_room_empty.jpg  (about 2000 px long side, same framing as wide_room.jpg).
  The last wide-room picture uses it automatically. Until then it shows the original.

THE OTHER ENDING
  Add  ?ending=room  to the web address. The room tone comes back over black instead of the street fading out.

TUNE THE LEVELS BY EAR
  Press M on the page. Sliders are in dB on top of your files (0 = exactly as you made them).
  "Copy mix" copies your settings so you can send them to me. "Jump to" scrolls to any chapter.
  DOOR_DELAY near the top of the script nudges the door sound against the film of the door.

YOUR AUDIO FILES ARE UNCHANGED
  Everything in audio/ is byte-for-byte what you exported from Premiere.

THE FILMS
  video/door.*, video/objects.* and video/flea_market.* are muted clips. door and objects are cut from screen
  recordings of stock footage: fine for class, but license or replace them before the page is public.
