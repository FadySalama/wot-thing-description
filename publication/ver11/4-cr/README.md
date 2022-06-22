# How to edit the draft for publication

## Files here
* visualization/ - directory for images
* Overview.html - static HTML for publication
* diff.html - diff between the [previous published verion](https://www.w3.org/TR/2021/WD-wot-thing-description11-20210607/ and Overview.html
* index.html - same as the index.html at https://w3c.github.io/wot-thing-description/ as of Feb. 28
* static.html - static HTML generated by ReSpec from the index.html above

## How to generate each file
Overview.html is generated as follows:
 1. As the basis of the check and edit, index.html was copied from https://w3c.github.io/wot-thing-description/ .
 1. static.html was generated by ReSpec from the index.html above (click "ReSpec" top right and choose "Export" then export as "HTML"
 1. Overview.html copied from static.html above, and then got tidied up using HTML Tidy

## How to add your edits based on the Pubrules errors/warnings
After checking Overview.html using the [Pubrules checker](https://www.w3.org/pubrules/), we have to edit index.html and then regenerate the static HTML based on the procedure above to make it easier to generate a Pullrequest to update the original at https://w3c.github.io/wot-thing-description/index.html later.
 1. Edit index.html
 1. Generate static.html by ReSpec from the index.html (click "ReSpec" top right and choose "Export" then export as "HTML"
 1. copy static.html to Overview.html and tidy it up
 1. If there are any remaining errors/warnings with the Pubrues checker results, repeat the edit by going back to #1.