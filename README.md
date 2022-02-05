# Code Refactor Starter Code
Notes


Feb 5 changes
ISSUE: During adding comments I realized the CSS was ordered in a way that mixed our informational seciton
and benefits section. This was only clerical, but it was easier to break these styles up separately
so they are easier to view and debug later on.

ACTION: Moved all benefit section element after the information section elemnts in style.css

ISSUE: The entire information content section is styled the same way. The articles already include an id and class.
We do not need both of these items. The class makes more sense to change since we are styling multiple elements the same way.

ACTION: Deleted id="" and kept class="" and updated the name to "content-container" since it applies in more than one place.
Updated css items listed by class (.) to id (#). This was done for the images and the content. Deleted duplicate css
code that repeated itself with multiple id's since one class is now styling all 3 elements.

ISSUE: Informational content section had all of the same h2 styling but used detail css items to style these elements.
It was calling out each class, add h2 as so ".online-reputation-management h2". Since all of these are styled the same
and included in the same containter it was easier to go to the element's parent and style the h2's that way. This reduces
the css code needed.

ACTION: Removed ".online-reputation-management h2" tags and updated them to ".content h2" to style the h2 elements.

