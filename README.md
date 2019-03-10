# User Centric Design resume

### *New Dictionary 
1. BootstrapCDN: bootstrap content delivery network. to enter bootstrap externally
2. sr-only: screen reader only. will not be displayed on a regular screen


### *Steps

#### Set up header
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

#### Set up footer     
1. make footer a flexible full width container
2. break footer into 3 sections: about me, download my CV and social links
3. creat a catch all set of style rules like .uppercase, .general-sub.
4. set up footer properties: bg color, font color, height, etc..
5. add footer content
- add a paragraph in About me section
- add up download link and icon (also sr-only)
- add a list of social media
- go to .css file to edit footer
- styling the social links
- make all footer elements less hocked up on top, add padding for footer

#### Add content to homepage
1. creat contact.html and resume.html files before content part, cause they are the same in each webpage
2. set up properties for container, table and each column
3. add rows for three reasons why hire Rosie
- set up header in one row
- add up new row for first reason to hire Rosie
- copy the new row code and change content for other two reasons
4. add new column of col-md-4 above col-md-8, casue elements are rendered in the order they appear in HTML by default
5. add header in new column and rows for info included
- styling the info section: create maxi space between each row
- positioned and styled each class level of personal info section
6. set up resume.html page
- set up basic grid of resume page
- add progress bar for resume skills by class="progress-bar" role="progressbar"
- style the progress bar in style.css file
7. add work history items
- firstly do styling, make work history background match header colors
- creat custom attributes called data-dates and data-...,the prefix "data-" is important for other developers to read
- <strong>set up the class value of timeline (which is a left border with a before/aftre pseudo class)</strong> 
8. edit contact.html page
- set up header for contact page
- insert a form snippt from bootstrap. this form will consist 4 components, 2 text input fields, 1 text area and a button
- styling contact heading and contact form
- start a media query to make contact form even smaller on desktop
9. creat CV.pdf download and wire up all pages together
- 

### *Important to understand or mistakes!!!!
1. line31 class="col-6 col-sm-3" means tow columns in mobile screen and 4 columns on any device larger than small screen! (bootstrap is mobile first)
2. line32 <span> inside <a> tag is because we need to target it later when using font awesome and hover.css
3. line30 the 4 navigation elements are 4 <li> elements, not 4 <a>!! When put 4 anchors into one list, they will squezed in one column. but when put 4 list items, they will seperate into 4 columns, but still 1 column was wrapped into the others
4. ! line30 when we display inline items, the white space in HTML file becames visible as single space between items. the way to solve this, is to creat a container with a font-size of 0. 
5. ! in order to solve the problem that font-size is 0 in menucontainter class. we override the font-size by targeting ID #nav and all list items inside it
6. line17,22,28 to close all gutters of columns (bootstrap padding to all columns by default), add no-gutters class to all the rows
7. in anchor tag, target="_blank" means the link will open in a new tab!!
8. line67, add transition to cv-pdf class. always add transition to parents class
9. div class="col-10 offset-1 offset-sm-0 col-sm-4 col-md-6" means 1 col in 10col size on mobile with 1col on left and right side as margin, no margin on tablet and desktop, 3 col on tablet and 2 col on desktop
10. <strong>! css file .timeline-item:before, do not understand at all why use a pseudo class here to make the sopt on left border</strong>

### *Question solved
1. Q10 the before/after pseudo elements: https://www.youtube.com/watch?v=zGiirUiWslI