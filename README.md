# User Centric Design resume

#### New Dictionary 
1. BootstrapCDN: bootstrap content delivery network. to enter bootstrap externally
2. 


#### Steps
1. Put together the basic project components
- create initial boilerplate 
- add bootstrap and font awesome links
- add basic tags used cross project (3 sites: index.html, contact.html, resume.html)
2. add a profile image to the header
- set 1/3 of the screen for image, and 2/3 for others
- import fonts from googlefonts to css file
- add some basic margin to set up the page
- add the profile photo as logo for the page which always take user to home page. anchor tag, column class, logo class to set up the features
3. add the owner's name and title
- add row and col in the other 2/3 of the row and editing bg color
4. add navigation elements and link to other pages
- set row and columns under name&title row
- edit the backgound colors for each list item
- remove these spaces between each nav-bar item
- close the gutter of bootstrap colums
5. add icons for navbars
- set up class and area-hidden property for <i> elements
- add a new "menuitem" class to make list elements height matches the total header height
- target .menuitem a {} to edit the font color, text-decoration of 4 nav items
- target .menuitem a i {} to edit icons
- target .menuitem a span {} to edit font propoerties
- merge the bottom of navbar, and make it even with logo picture
6. add hover effect
- get hover.css link from https://cdnjs.com/ (a content delivery network for open source projects)
- add hvr-sweep-to-bottom class to each anchor tag
- edit hvr-sweep-to-bottom class in .css file. switch to a nicer background color when hovered
     


#### Important to understand or mistakes!!!!
1. line31 class="col-6 col-sm-3" means tow columns in mobile screen and 4 columns on any device larger than small screen! (bootstrap is mobile first)
2. line32 <span> inside <a> tag is because we need to target it later when using font awesome and hover.css
3. line30 the 4 navigation elements are 4 <li> elements, not 4 <a>!! When put 4 anchors into one list, they will squezed in one column. but when put 4 list items, they will seperate into 4 columns, but still 1 column was wrapped into the others
4. ! line30 when we display inline items, the white space in HTML file becames visible as single space between items. the way to solve this, is to creat a container with a font-size of 0. 
5. ! in order to solve the problem that font-size is 0 in menucontainter class. we override the font-size by targeting ID #nav and all list items inside it
6. line17,22,28 to close all gutters of columns (bootstrap padding to all columns by default), add no-gutters class to all the rows