# css_trick
Just note the css trick to reference

Ways to override Style
  1. Declare order
  The order of the class declarations in the <style> section are what is important. The second declaration will always take precedence over the first. 
```
    <style>
      .pink-text {
        color: pink;
      }
      .blue-text {
        color: blue;      // this style take precedence
      }
    </style>
  <h3 class="pink-text blue-text">Hello World!</h3>
```
  ↓↓
  <h3 style="color: bule; font-size">Hello World!</h3>
  
  2. Id selector
   It doesn't matter whether you declare style after or before another style that have conflict attribute, since id attribute will always take precedence.
   
   ````
    <style>
      .pink-text {
        color: pink;
      }
      .blue-text {
        color: blue;
      }
      #orange-text {
        color: orange;      // this style take precedence
      }
    </style>
    <h3 id="orange-text" class="pink-text blue-text">Hello World!</h3>
   ````
   ↓↓
   <h3 style="color: orange">Hello World!</h3>
   
