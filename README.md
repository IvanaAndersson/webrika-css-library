# CSS writing style guide
The team style guide should always win over your own personal preferences. Consistency is important.

## Splitting your CSS

### Try to split your CSS / SCSS into logical sections

It is a good idea to have all of the common styling first in the stylesheet. 

This means all of the styles which will generally apply unless you do something special with that element. You will typically have rules set up for:

body
p
h1, h2, h3, h4, h5
ul and ol
The table properties
Links

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

### Documentation on the top of the CSS file - write which sections your CSS file consists of in the beginning of the file for easier search
```
/*
1. GENERAL STYLES
2. HEADER AND NAVIGATION
3. SECTION SIDEBAR
4. SECTION MAIN CONTENT
5. FOOTER
*/
```


## Syntax guidelines

### 1. Use expanded syntax

Write this:
```
p {
  color: white;
  background-color: black;
  padding: 1rem;
}
```

Not this:
```
p { color: white; background-color: black; padding: 1rem; }
```

* Include a space between the selector(s) and the opening curly brace.
* Always include a semi-colon at the end of the last declaration, even though it isn't strictly necessary.
* Put the closing curly brace on a new line.
* In each declaration, put a space after the separating colon, but not before.
* Use 2 spaces for code indentation.

### 2. CSS comments 

Use CSS-style comments to comment code that isn't self-documenting:
``` 
/* This is a CSS-style comment */
```
Put your comments on separate lines preceding the code they are referring to:

```
h3 {
  /* Creates a red drop shadow, offset 1px right and down, w/2px blur radius */
  text-shadow: 1px 1px 2px red;
  /* Sets the font-size to double the default document font size */
  font-size: 2rem;
}
```

## 3.Don't use !important
!important is a last resort generally only used when you need to override something and there is no other way. It is a bad practice and you should avoid it wherever possible.

Bad:
```
.bad-code {
  font-size: 4rem !important;
}
```

## Selectors

### 1. Avoid overly-specific selectors

### 2. Don't use ID selectors
Except when you need to override an id selector from a Shopify theme


### 3. Put multiple selectors on separate lines

```
h1,
h2,
h3 {
  font-family: sans-serif;
  text-align: center;
}
```

## Folder structure

main.css is the only file outside all other folders. In main.css we import all other css files. 
 