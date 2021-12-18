# 360 Degree Images in HTML and WordPress via the Panellum JavaScript Library

Integrate 360 degree images from Ricoh Theta in HTML and WordPress.

* panellum.html - *how to do it in HTML*
* wordpress-in-page-post.htm - *how to do it in a WordPress post*

The 360 degree view is made thanx to the [Panellum Library](https://pannellum.org/).

## Note: WordPress

If you add the code to a page or post remember that the custom HTML field will add p-tags if there are blank lines. So remove all blank lines - and then the code will work.

~~~~
<script>
  window.onload = function() {
    const author = "Per Thykjaer Jensen"
    const img = "ADD-URL-TO-YOUR-IMAGE-HERE.JPG";
    pannellum.viewer('panorama', {
      "type": "equirectangular",
      "panorama": img,
      "title": "The Old Town - dec. 17th. 2021, Aarhus",
      "author": author,
      "autoLoad": true
    });
  } // document ready
</script>
~~~~
