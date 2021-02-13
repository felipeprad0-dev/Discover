# Shorthand 

    * Merging properties
    * Summed up 
    * Readable


```CSS
* {
    /* background properties */
    background-color: #000; 
    background-image: url(images/bg.gif);
    background-repeat: no-repeat;
    background-position: left top;

    /* background shorthand */
    background: #000 url(images/bg.gif) no-repeat left top;



    /* font properties */
    font-style: italic;
    font-weight: bold;
    font-size: .8em; 
    line-height: 1.2;
    font-family: Arial, sans-serif;

    /* font shorthand */
    font: italic bold .8em/1.2 Arial, sans-serif;
}
```


## Details

    * Will not consider previous properties 
    * Will assume default value if no value is specified 
    * It doesn't usually matter the order described, but if there are many properties with similar values, we may find problems


## Properties that allows shorthand  

    all, animation, background, border, border-block-end, border-block-start, border-bottom, border-color, border-image, border-inline-end, border-inline-start, border-left, border-radius, border-right, border-style, border-top, border-width, column-rule, columns, flex, flex-flow, font, gap, grid, grid-area, grid-column, grid-row, grid-template, list-style, margin, mask, offset, outline, overflow, padding, place-content, place-items, place-self, scroll-margin, scroll-padding, text-decoration, text-emphasis, transition.