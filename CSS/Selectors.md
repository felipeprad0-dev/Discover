# Selectors

    * Selectors connect html elements with css

## Types 

* Global selector '*' 
* Element/Type selector 'h1, h2, p, div'
* ID Selector '#box, #container'
* Class Selector '.red, .m-4' 
* Attribute selector, Pseudo-class, Pseudo-element, e outros...

```HTML

<div id="container" class="m-40">
    <h1>Title</h1>
</div>    

```

```CSS 

* {
    margin: 0;
}

#container {
    width: 200px;
}

.m-40 {
    margin: 40px;
}

h1 {
    color: blue;
    font-size: 60px;
    background: gray;
}

```