# How to Build a Website

## Example 1 : HTML

Creating your first `HTML` page.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Example 1</title>
</head>
<body>
    <h1>Hello world!</h1>
    <p1>My first HTML page :)</p1>    
</body>
</html>
```

## Example 2 : CSS

`index.html`
```html
<!DOCTYPE html>
<html>
<head>
    <link rel="stylesheet" type="text/css" href="./style.css">
    <title>Example 2</title>    
</head>
<body>
    <h1 style="color: gray; font-family: 'Helvetica Neue'; font-weight: 100; font-size: 70px;">Hello world</h1>
    <p class="myP">Test paragraph</p>
</body>
</html>
```

`style.css`
```css
p {
    color: red;
    font-size: 50px;
    font-family: "Helvetica Neue";
    font-weight: 100;
}

.myP {
    color: blue;
    font-size: 50px;
    font-family: "Helvetica Neue";
    font-weight: 100;
}
```

## Example 3 : Flexbox

`index.html`
```html
<!DOCTYPE html>
<html>
<head>
    <link rel="stylesheet" type="text/css" href="./style.css">
    <title>Flexbox example</title>
</head>
<body>

    <div class="container">
        <div class="card">1</div>
        <div class="card">2</div>
        <div class="card">3</div>
    </div>

</body>
</html>
```

`style.css`
```css
.container {
    display: flex;
    flex-direction: row;
    justify-content: center;
    flex-wrap: wrap;    
}

.card {    
    background-color: #F5F5F5;
    width: 250px;
    height: 300px;
    margin: 10px;
    text-align: center;
}
```

## Example 4 : Grid

`index.html`
```html
<!DOCTYPE html>
<html>
<head>
    <title>Example 4</title>
    <link rel="stylesheet" type="text/css" href="./style.css">
</head>
<body>
    <div class="gridContainer">
        <div class="cell">Test</div>              
        <div class="cell">Test</div>
        <div class="cell">Test</div>
        <div class="cell">Test</div>
        <div class="cell">Test</div>
        <div class="cell">Test</div>
        <div class="cell">Test</div>
        <div class="cell">Test</div>
        <div class="cell">Test</div>
        <div class="cell">Test</div>
        <div class="cell">Test</div>
        <div class="cell">Test</div>
    </div>
</body>
</html>
```

`style.css`
```css
.gridContainer {
    display: grid;
    grid-template-columns: 1fr 50px auto 50px 1fr;    
    grid-template-rows: 50px 50px 50px;
    grid-column-gap: 10px;
    grid-row-gap: 10px;
    grid-auto-flow: row;
    justify-content: center;
}

.gridContainerFluid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));    
    justify-content: center;
    grid-column-gap: 10px;
    grid-row-gap: 10px;
}

.cell {
    background-color: gray;    
}
```

## Example 5 : Bulma.io

`index.html`
```html
<!DOCTYPE html>
<html>
<head>    
    <title>Example 4: Bulma.io</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bulma/0.7.5/css/bulma.min.css">
    <link rel="stylesheet" type="text/css" href="./style.css">
</head>
<body>

    <div class="myContainer">
        <div class="constrain">                                            
            <h1 class="title">Hello world</h1>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed dignissim diam nec nunc ullamcorper, sed ultricies eros efficitur. Donec tincidunt aliquam urna a iaculis. Duis dictum augue eu convallis tincidunt. Sed nunc neque, varius et mauris a, consectetur venenatis dolor. Vivamus feugiat eros vel ipsum luctus, tincidunt ultricies ligula aliquam. Pellentesque lorem diam, dignissim ut ornare non, dictum non nibh. Vestibulum ac augue est.</p>
            <a class="button is-primary">Primary</a>
        </div>              
    </div>

</body>
</html>
```

`style.css`
```css
.myContainer {
    display: flex;    
    align-items: center; 
    text-align: center;    
    flex-direction: column;
    margin-top: 50px;
    width: 100%;
}

.constrain {
    width: 500px;
}

.button {
    margin-top: 20px;
}
```

## Example 6 : Personal website

### Project structure
```html
<!DOCTYPE html>
<html>

<head>    

    <!-- Metadata -->
    <title>My website</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <!-- Bulma.io -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bulma/0.7.2/css/bulma.min.css">

    <!-- Custom stylesheet -->
    <link rel="stylesheet" type="text/css" href="./style.css">

    <!-- JQuery -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
</head>

<body>
</body>
  
</head>
```

### Navbar
```html
<!-- Navbar -->
<nav class="navbar is-fixed-top">
    <div id="navbarBasicExample" class="navbar-menu scrollTo">
        <div class="navbar-end">                
            <a class="navbar-item" href="#home">Home</a>
            <a class="navbar-item" href="#portfolio">Portfolio</a>                
            <a class="navbar-item" href="#contact">Contact</a>
        </div>          
    </div>
</nav>
```

### Landing Page
```html
<!-- Landing Page -->
<section class="hero is-fullheight" id="home">
    <div class="hero-body">
        <div class="container has-text-centered">

            <!-- Basic placeholder title -->
            <!-- <h1 class="title">My name</h1> -->

            <!-- Cool typing effect -->
            <h1 class="title is-1 code">                   
                  <span class="txt-rotate" data-period="500"
                  data-rotate='[ "My name here", "student.", "developer.", "[insert cool fact here that is kinda funny but not really]"]'>                      
                  </span>
            </h1>

        </div>
    </div>
</section>
```

### Portfolio
```html
<!-- Portfolio -->
<section class="hero is-fullheight" id="portfolio">
    <div class="hero-body">
        <div class="container has-text-centered">

            <h1 class="subtitle is-3" style="margin-bottom: 50px;">Portfolio</h1>  

            <div class="cardGrid">

                <!-- Card 1 -->                    
                <div class="card" style="width: 300px;">
                    <!-- An option of putting a link on the card -->
                    <a href="https://google.com">
                        <div class="card-image">
                            <figure class="image is-4by3">
                                <img src="https://bulma.io/images/placeholders/1280x960.png" alt="Placeholder image">
                            </figure>
                        </div>
                        <div class="card-content">
                            <h1 class="subtitle is-4">Project 1</h1>
                            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis</p>
                        </div>
                    </a>
                </div> 

        </div>
    </div>
</section>
```
```css
/* Portfolio css */
.cardGrid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));    
    grid-gap: 1rem; 
    align-content: center;
}
.card {
    margin: 20px;
    place-self: center;
}
```

### Contact
```html
<!-- Contact -->
<section class="hero" id="contact">
    <div class="hero-body" style="background-color: #f5f5f5;">
        <div class="container has-text-centered">

            <h1 class="subtitle is-3" style="margin-bottom: 20px;">Contact</h1>  
            <p style="margin-bottom: 50px;">Feel free to connect with me on social :)</p>                

            <div class="contactContainer">
                <a class="button is-primary" href="https://Ngoogle.com">LinkedIn</a>
                <a class="button is-primary">Github</a>
                <a class="button is-primary">Resume</a>
                <a class="button is-primary">Twitter</a>
                <a class="button is-primary">Leetcode</a>
                <a class="button is-primary">YouTube</a>
            </div>
        </div>
    </div>
</section>
```
```css
/*Contact css*/
.contactContainer {
    display: flex;
    justify-content: center;
    align-content: center;
    flex-wrap: wrap;
}
.button {
    margin: 10px;
}
```

### Javascript/jQuery
Add this after metadata:
```javascript
<!-- Smooth Scrolling -->
<script>
    $(document).ready(function(){
      // Add smooth scrolling to all links
      $("a").on('click', function(event) {

        // Make sure this.hash has a value before overriding default behavior
        if (this.hash !== "") {
          // Prevent default anchor click behavior
          event.preventDefault();

          // Store hash
          var hash = this.hash;

          // Using jQuery's animate() method to add smooth page scroll
          // The optional number (800) specifies the number of milliseconds it takes to scroll to the specified area
          $('html, body').animate({
            scrollTop: $(hash).offset().top
          }, 800, function(){

            // Add hash (#) to URL when done scrolling (default click behavior)
            window.location.hash = hash;
          });
        } // End if
      });
    });
</script>    
```
Add this straight after your `</html>` closing tag:
```javascript
<!-- Custom script for cool landing page text -->
<script type="text/javascript">
    var TxtRotate = function(el, toRotate, period) {
      this.toRotate = toRotate;
      this.el = el;
      this.loopNum = 0;
      this.period = parseInt(period, 10) || 2000;
      this.txt = '';
      this.tick();
      this.isDeleting = false;
    };

    TxtRotate.prototype.tick = function() {
      var i = this.loopNum % this.toRotate.length;
      var fullTxt = this.toRotate[i];

      if (this.isDeleting) {
        this.txt = fullTxt.substring(0, this.txt.length - 1);
      } else {
        this.txt = fullTxt.substring(0, this.txt.length + 1);
      }

      this.el.innerHTML = '<span class="wrap">'+this.txt+'</span>';

      var that = this;
      var delta = 150 - Math.random() * 100;

      if (this.isDeleting) { delta /= 2; }

      if (!this.isDeleting && this.txt === fullTxt) {
        delta = this.period;
        this.isDeleting = true;
      } else if (this.isDeleting && this.txt === '') {
        this.isDeleting = false;
        this.loopNum++;
        delta = 500;
      }

      setTimeout(function() {
        that.tick();
      }, delta);
    };

    window.onload = function() {
      var elements = document.getElementsByClassName('txt-rotate');
      for (var i=0; i<elements.length; i++) {
        var toRotate = elements[i].getAttribute('data-rotate');
        var period = elements[i].getAttribute('data-period');
        if (toRotate) {
          new TxtRotate(elements[i], JSON.parse(toRotate), period);
        }
      }
      // INJECT CSS
      var css = document.createElement("style");
      css.type = "text/css";
      css.innerHTML = ".txt-rotate > .wrap { border-right: 0.08em solid #666 }";
      document.body.appendChild(css);
    };
</script>
```

## Conclusion

Thank you for reading!
