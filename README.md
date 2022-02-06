# Code Refactor Starter Code

# Horiseon

##Purpose
Update source code to follow accessibility standards, improves search engine optimization and improve overall code efficiency and clarity by utitlizing semantic html elements and reducing repetative/re-written css code.

##Built With
* HTML
* CSS

#Website
https://7krich.github.io/urban-octo-telegram/Develop/index.html

#Contribution
Made by Kyle Richnafsky

# Updates made

Sequential order (to best of recolection)...

ISSUE: Header formatting required classes. It didn't need a class, header can simply be listed as header

ACTION: flipped class="header" to header to fix semantics

ISSUE: title did not apply to the webpage.

ACTION: updated title to reflect "Horiseon" for search engine optmizaiton and meet creteria.

ISSUE: Semantic structure (divs and h2, h3) needed to be updated to sections, articles and accurate headings. This will aid search engine optimization and formatting.

ACTION: updated div tags to articles & sections along with correcting h2 & h3 tags.

ISSUE: Search engine optimization and index page link not working.

ACTION: Corrected id to link to the search engine optimization article so when clicked, page skips down to seciton. Also updated index link to bring used back to home page in event additional pages are added later.

ISSUE: No alt tags included for photos. Vision impaired users would have issues reading the webpage.

ACTION: alt tag added to photos with concise description.

ISSUE: During adding comments I realized the CSS was ordered in a way that mixed our informational seciton and benefits section. This was only clerical, but it was easier to break these styles up separately so they are easier to view and debug later on.

ACTION: Moved all benefit section element after the information section elemnts in style.css

ISSUE: The entire information content section is styled the same way. The articles already include an id and class. We do not need both of these items. The class makes more sense to change since we are styling multiple elements the same way.

ACTION: Deleted id="" and kept class="" and updated the name to "content-container" since it applies in more than one place. Updated css items listed by class (.) to id (#). This was done for the images and the content. Deleted duplicate css code that repeated itself with multiple id's since one class is now styling all 3 elements.

ISSUE: Informational content section had all of the same h2 styling but used detail css items to style these elements. It was calling out each class, add h2 as so ".online-reputation-management h2". Since all of these are styled the same and included in the same containter it was easier to go to the element's parent and style the h2's that way. This reduces the css code needed.

ACTION: Removed ".online-reputation-management h2" tags and updated them to ".content h2" to style the h2 elements.

ISSUE: benefit lead brand and cost classes are all the same. If they were different they should be id's, but since they are the same I am switching them all to the same class name. This will properly use the class selector and reduce css code. This allows me to consolidate all the css code for the same tags with the child elements h3 and img. Now all 3 css tags for benefit article are articulated in css with just 3 selctors instead of 9.

ACTION: update names of these classes to be synonymous as "benefit-article". Delete repetitive, un-needed code in style sheet.

ISSUE: Removal of id's above created issue where links were not working. The href in the header had nothing to link to.

ACTION: id's added back for search engine optimization, online reputation management and social media marketing. Links working again.

ISSUE: After doing addiitonal research I realized the article html elements I used did not fit the purpose.

ACTION: Changed article tags to div>and kept necessary class tags.

