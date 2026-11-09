# Fitting Room

A phone-first wardrobe app, published as a private Claude artifact:
https://claude.ai/artifact/LNqdCq5bEo5vD9NHTE12td

`fitting-room.html` is the whole app (one file, Preact + htm from jsDelivr). It runs inside Claude and uses the
artifact runtime for storage (`db`), photo storage (`assets`), Claude vision and styling (`sample`), the
owner check (`user`) and the JSON backup (`downloads`). Opened anywhere else it loads but cannot save.

Sections: Closet, Add (photo queue, review), Style (stylist, shop check), Looks (lookbook, pairs, wear diary),
Insights (palette, dress-code and heat spread, gaps, wishlist, let-go history, backup), and Mock me (figure and stylist notes).

To update the live app, edit the HTML and republish it to the same artifact URL.
