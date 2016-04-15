nodenticon
============

GitHub-style identicons in NodeJS.



Credits
----
Biblioteca basada en [identicon.js](https://github.com/stewartlord/identicon.js) 
de [stewartlord](https://github.com/stewartlord)



Options
----
* **hash** - [Optional] A unicode string that will be used to generate the image. Defaults to a random hash based on the current time.
* **options** - [Optional] An options object used to customize the generated image.
    * **background** - The background color expressed as an rgba value array to use for the image background. For example, use [255,0,0,255] for red. Defaults to an opaque light gray [240,240,240,255].
    * **margin** - The decimal fraction of the size to use for margin. For example, use 0.2 for a 20% margin. Defaults to 0.08 for an 8% margin.
    * **size** - The size in pixels of the height and width of the generated (square) image. Defaults to 64 pixels.



Installation
-----
```npm install nodenticon```



Usage
-----
##### Simple
Generate the Identicon by supplying a hash string and size.
// create a base64 encoded PNG
var data = new Identicon('hash', 420).toString();

// write to a data URI
document.write('<img width=420 height=420 src="data:image/png;base64,' + data + '">');
```