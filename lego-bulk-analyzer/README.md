# Brick Lot Appraiser

A single-page web app that checks whether a second-hand bulk LEGO lot is worth buying.

1. Enter the seller's asking price (and the weight, if the listing gives one).
2. Add photos of the lot.
3. Claude looks for minifigures, valuable parts and identifiable sets, values the generic
   remainder by weight, and compares the total resale value (after selling costs) to the asking price.

Each item has links to eBay sold listings and BrickLink, so you can check prices before you buy.
You can untick anything you disagree with to drop it from the total.

## Where it runs

The page is published as a claude.ai Artifact and uses the Artifact `sample` capability to send
photos to Claude on the viewer's own Claude account, so it needs no API key or server. It works in any
browser or in the Claude app on phone, tablet and PC.

Opening `index.html` directly from disk shows the example report only, because the page can't reach
Claude outside claude.ai.

## Limits

- Prices are Claude's estimates from photos and general market knowledge, not live listings.
- Photos are downsized to about 1.2 megapixels before analysis, so close-ups of pieces spread out on
  a flat surface work much better than one photo of a sealed bag.
