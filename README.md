# jQuery Scroll Image Inside v0.1
A jQuery plugin allowing you to scroll an image within a container element

![Demo](https://github.com/ashwebstudio/jquery-scrollimageinside/blob/main/assets/demo.gif)

# Usage
```html
<div id="window">
    <img src="really-long-image.jpg" alt="" />
</div>
<script>
$( document ).ready(function(){
	$( '#element' ).scrollimageinside();
});
</script>
```

Recommend the following CSS for the up/down hover
```html
.scrollimage-up { position: absolute; z-index: 999; top: 0; left: 0; right: 0; bottom: 50%; transition: all .2s; background: linear-gradient(0deg, rgba(25,30,34,0) 0%, rgba(25,30,34,0.4) 100%); opacity: 0; }
.scrollimage-up:hover { opacity: 1; }
.scrollimage-down { position: absolute; z-index: 999; top: 50%; left: 0; right: 0; bottom: 0; transition: all .2s; background: linear-gradient(0deg, rgba(25,30,34,.4) 0%, rgba(25,30,34,0) 100%); opacity: 0; }
.scrollimage-down:hover { opacity: 1; }
```

# Options
```html
$( '#element' ).scrollimageinside({
    easing: 'linear', // Set easing
    speed: 1500, // Scroll speed
    height: 500 // Explicitly set height of scroll window if not set in your own CSS
});
```

# Examples
See the examples folder or [my portfolio site this was built for](https://www.ashwebstudio.com/portfolio/sunshine-photo-cart/)
