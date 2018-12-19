
#### Three pillars of writin good HTML and CSS
 * Responsive Design
 * Maintainable and Scalable code
 * Web Performance

 ##### Responsive Design
* Fluid Layouts
* Media Queries
* Responsive Images
* Correct Units
* Desktop-first vs Mobile-first

##### Maintainable and Scalable code
* Clean
* Easy to understand 
* Growth
* Reusable
* How to orginize files
* How to name classes 
* How to structure HTML

##### Web Performance

* Less HTTP requests
* Less code
* Compress code
* Use a CSS preprocessors
* Less images
* Compress images

#### How CSS works behind the scene

When HTML is loaded in the browser it parses the HTML and when it comes to head part it loads the CSS files. At the same time it builds DOM from the HTML and also builds CSSOM from CSS files. Then browser creates Render Tree, after that browser creates The Visual Formatting Model then finally, website will be rendered.

##### Cascade
Process of combining different stylesheets and resolving conflicts between different CSS rules and declarations, when more than one rule applies to a certain element.
### Importance > Specificty > Source order
Order explained in Slides

* CSS declarations marked with !important have the highest priority;
* But, only use ! important as a last resource. It is better to use correct specifications - more maintanable code!
* Inline styles will always have priority over in external stylesheets;
* A selector that contains 1 ID is more specific than one with 1000 classes;
* The Universal selector * has no specificity value (0, 0, 0, 0);
* Rely more on specifity than on the order of selectors;
* But, rely on order when using 3rd-party stylesheets, always put your author stylesheet last.

#### How CSS values are processed

All the relative unit values like rem, vh, percentage, etc.. and ultimatly converted to absolute units (pixel) and always in relation to parent element. Font sizes are always relative to the root font size of the element.

* Each property has an initial value, used if nothing is declared;
* Browsers specify a root font-size for each page;
* Percentage and relative values are alwaysnconverted to pixels;
* Percentages are measured relative to their parent's font-size, if used to specify font-size;
* Percentages are measured relative to their parent's width, if used to specify length;
* ` em ` are measured relative to their parent font-size, if used to specify font-size;
* ` em ` are measured relative to their current font-size, if used to specify font-size;
* ` rem ` are always measured relative to the document's root font-size;
* ` vh ` and ` vw ` are simply percentage measurements of the viewport's height and width;


#### Inheritence in CSS

Each and every property must have a value.

* Inheritence passes the values for some specific properties from parents to children - more maintanible code;
* Properties related to text are inherited: font-family. font-size, color, etc;
* The computed value of a property is what gets inherited, not the declared value;
* Inheritence of a property only works if no one declares a value for that property;
* The `inherit` keyword forces inheritance on certain property;
* The initial keyword resets a property to its initial value;

#### The visual formatting model

Algorithm that calculates boxes and determines the layout of these boxes, for each element in the render tree, in order to determine the final layout of the page.

* Dimensions of boxes: the box model;
* Box type: inline, block and inline-block;
* Positioning scheme: floats and positioning;
* Stacking contexts;
* Other elements in the remder tree;
* Viewport size, dimensions of images, etc.

#### CSS Architecture

THINK > BUILD > ARCHITECT

BEM : Block Element Modifier
The 7-1 Pattern: seven different folders for partial Sass files, and one main Sass file to import all other files into a compiled CSS stylesheet.