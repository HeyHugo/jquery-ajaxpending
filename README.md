jQuery-ajaxPending
==================
Easily bootstrap ajax loading animations.

Show "spinner" and dim effect on element X when url Y has a pending ajax call

[demo](http://jsfiddle.net/HeyHugo/GdR2y/)

Usage
--------
``
$("some-element").ajaxPending(url, options)
``
 
Usage examples
--------------
```
$("#weather").ajaxPending("/weather/update");
```

```
$("#news-feed").ajaxPending("/news/fetch-more", {interval: 35, container_css: {"background-color": "rgba(50,50,50,0.5)"}});
```

Default options
-------------------------------
```
{
    animation_interval: 35,
    sprite_count: 19,
    container_css: {
        "display": "block",
        "position": "absolute",
        "z-index": "1000",
        "background-color": "rgba(255,255,255,0.5)"
    },
    spinner_css: {
        "display": "block",
        "width": "32px",
        "height": "32px",
        "margin-top": "10%",
        "z-index": "1001",
        "background-repeat": "no-repeat",
        "background-image": "url('<base64 encoded png sprite>')",
        "position": "relative"
    }
}
```
The spinner sprite is included as base64 encoded data inside the plugin.


Author
------
Hugo Heyman

License
-------
MIT License
