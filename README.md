# CSS Trick 
Just note tricks in css to reference

## Centering CSS
https://css-tricks.com/centering-css-complete-guide/

## Display Property CSS
http://taneppa.net/display_other01/

## Overflow trick
http://www.stubbornella.org/content/2009/07/23/overflow-a-secret-benefit/

## 9 Most Common IE Bugs
https://code.tutsplus.com/tutorials/9-most-common-ie-bugs-and-how-to-fix-them--net-7764

## Put footer in the end of page
```
html {
  position: relative;
}
body {
  margin-bottom: 50px; // equals or higher than .footer height
}
.footer {
  position: absolute;  // set footer is absotule so it's position is compare with <html> tag
  bottom: 0;   // it's space to bottom of <html> tag is 0, so .footer always in the end of document
}
```
## Grid by example
https://gridbyexample.com/examples/
