jQuery-ajaxPending
==================
Easily bootstrap ajax loading animations.

Show "spinner" and dim effect on element X when url Y has a pending ajax call

Usage
--------
``
$("some-element").ajaxPending(url, override_css)
``
 
Usage examples
--------------
```
$("#weather").ajaxPending("/weather/update");
```

```
$("#news-feed").ajaxPending("/news/fetch-more", {"background-color": "rgba(50,50,50,0.5)"});
```

Spinner element default styling
-------------------------------
```
{
        "display": "block",
        "position": "absolute",
        "z-index": "1000",
        "background-image": "url('data:image/gif;base64,<Base64 encoded gif data>')",
        "background-repeat": "no-repeat",
        "background-color": "rgba(255,255,255,0.5)",
        "background-size": "auto",
        "background-position": "50% 10%"
}
```
The spinner gif is included as base64 encoded data inside the plugin.

Author
------
Hugo Heyman

License
-------
MIT License