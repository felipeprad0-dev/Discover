# Cascade

    * The choice of which rule to apply is the browser, if there are many rules for the same element.
    * Your style is read from top to bottom.
  
    * 3 factors are considered 
        1. Style source 
        2. Specificity
        3. Importance 
   

## Irigin Of The Style 

    inline > tag style > tag link 


## Specificity 

It is a mathematical calculation where each type of selector and style source have values ​​to consider.

    1. Universal selector, combinators e negation pseudo-class (:not())
    2. Element type selector e pseudo-elements (::before, ::after)
    3. Classes e attribute selectors ([type="radio"]) (class="title") .title
    4. ID selector (id="title") #title
    5. Inline 
    