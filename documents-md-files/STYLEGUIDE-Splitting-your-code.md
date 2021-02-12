# CSS writing style guide
The team style guide should always win over your own personal preferences. Consistency is important.


## Folder structure

main.css is the only file outside all other folders. In main.css we import all other css files. 

### Folder ''abstracts'' includes:
* resets and normalize files, 
* variables, 
* typography, 
* mixins

### Folder ''components'' includes files:
* helper classes
* buttons
* sections, which may be made into components

### Folder ''sections'' includes sections, which 'may be included in all the pages (header, footer, etc.)

### Folder ''pages'' includes:
* home pages styles
* about page styles (if relevant)
* collection page styles (if relevant)
* product page styles (if relevant)

## Splitting your styles

### Try to split your CSS / SCSS into logical sections

It is a good idea to have all of the common styling first in the stylesheet. 
This means all of the styles which will generally apply unless you do something special with that element. You will typically have rules set up for:

* body
* p
* h1, h2, h3, h4, h5
* ul and ol
* The table properties
* Links

### Put comments whenever you begin a new section

```
/* GENERAL STYLES */

...

/* HEADER AND NAVIGATION */

...

/* SECTION SIDEBAR */

...

/* SECTION MAIN CONTENT */

...

/* FOOTER */

...
```

### Documentation on the top of the CSS / SCSS file :
- write which sections your CSS file consists of in the beginning of the file for easier search
```
/*
1. GENERAL STYLES
2. HEADER AND NAVIGATION
3. SECTION SIDEBAR
4. SECTION MAIN CONTENT
5. FOOTER
*/
```
 