# CSS Trick 
Just note tricks in css to reference

## Ways to override Style
  1. Declare order
  The order of the class declarations in the <style> section are what is important. The second declaration will always take precedence over the first. 
  
    *Note: It doesn't matter which order the classes are listed in the HTML element.*
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
  <h3 style="color: bule; font-size">Hello World!</h3> (Color is blue, Markdown can't change text color, man)
  
  2. Id selector
    Id declarations override class declarations, regardless of where they are declared in your style element CSS.
   
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
   <h3 style="color: orange">Hello World!</h3>  (Color is orange)
   
   3. Inline style
   In-line styles will override all the CSS declarations in your style element.
   
   ```
   <style>
      .pink-text {
        color: pink;
      }
      .blue-text {
        color: blue;
      }
      #orange-text {
        color: orange;
      }
  </style>
  <h3 id="orange-text" class="pink-text blue-text" style="color: white">Hello World!</h3>
   ```
   ↓↓
   <h3 style="color: white">Hello World!</h3> (White color)
   
   4. Using Important
    When you absolutely need to be sure that an element has specific CSS, you can use !important
    
    ```
    <style>
      .pink-text {
        color: pink !important;
      }
      .blue-text {
        color: blue;
      }
      #orange-text {
        color: orange;
      }
    </style>
    <h3 id="orange-text" class="pink-text blue-text" style="color: white">Hello World!</h3>
    ```
    ↓↓
    <h3 style="color: pink">Hello World!</h3> (Pink color)
