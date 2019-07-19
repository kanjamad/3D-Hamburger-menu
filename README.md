# 3D Hamburger Menu
* Click on hamburger menu it will be transformed into X.
* Then will display Navbar and new background image from top and bottom size
* When hover on navbar items will see 3D effects
* This project will based on HTML CSS and JavaScript
* This project will fully responsive


### create hamburger menu

```
<div class="hamburger-menu">
    <div class="line line-1"> </div>
    <div class="line line-2"> </div>
    <div class="line line-3"> </div>
</div>

```

```
.hamburger-menu {
    width: 35px;
    height: 30px;
    position: fixed;
    top: 40px;
    right: 50px; 
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    cursor: pointer;
}

.line {
    width: inherit;
    height: 5px;
    background-color: #16c3cf;
}

```

* Class line  line-1 : first for common style, second for individual styling 
* Inherit : we need width equal to their parent elements width = 35px, So instead of defining it manually I can use value called inherit.
* Create space between line used flexbox