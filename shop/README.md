# Bangla Ludu: server-driven shop files

The game downloads shop items added after the app was built from this folder (the server's `catalog.json` lists them
with these file names). A file is downloaded once and kept on the phone, so a changed picture needs a NEW file name.

Files ending in `_test` are previews used for testing (only shown to the test account).

`core/` holds the pictures of the game's own paid shop items (avatars `AvatarsShop/avs_N.png`, painted token skins
`Tokens/art_N_C.png`, painted boards `Boards/board_N.png`, `bg_N.png`, `yard_N_K.png`). They are not inside the app:
every phone downloads them in the background from its first start. Master copy: chokka repo `RemoteArt/core/`.
Never rename or change these files in place (phones keep what they downloaded); a new picture needs a new item.
