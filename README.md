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


### Perspective
* The perspective CSS property gives an element a 3D-space by affecting the distance between the Z plane and the user.

### Inser text of each navigation item
* I need to insert text of each navigation item
* I can do manully by using an child selector But I have a better solution. As I value of content property I can insert the value of HTML attribute. In this case will add each link element attribute called data-text and assign them to property values.
* After value of content I need to insert method called attributes with arguments call data-text
* Then as see after navigation item will have appropriate content.
* Next just find position


```
/* CSS */

.nav-link::after {
    content: attr(data-text);
}

```


```
/* HTML */

 <nav class="top-nav">
    <ul class="nav-list">
        <li>
            <a href="#" class="nav-link" data-text="Home">Home</a>
        </li>
        <li>
            <a href="#" class="nav-link" data-text="About Us">About Us</a>
        </li>
        <li>
            <a href="#" class="nav-link" data-text="Our Team">Our Team</a>
        </li>
        <li>
            <a href="#" class="nav-link" data-text="Services">Services</a>
        </li>
        <li>
            <a href="#" class="nav-link" data-text="Contact">Contact</a>
        </li>
    </ul>
</nav>

```



## Additional Resources

1. <a href="https://css-tricks.com/almanac/properties/p/perspective/" target="_blank">Perspective animation</a>
