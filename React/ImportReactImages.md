# Importing React Images

Do not add the image folder in the src React folder.  

```
|--src
|   |--images
|   |   |--image.png
|   |--App.js
|   |--package.json
|--public
|   |--index.html
```

Instead create the images folder under the public folder.

```
|--src
|   |--App.js
|--public
|   |--index.html
|   |--images
|   |   |--image.png
|   |   |--image2.png

When you what to access it in an image tag src from the public/images folder, you can just write the path as follows:

>
> <img src="/images/image.png" alt="image"/>
>


If you were to try to write out the entire path in the image src tag, React will not see the image.  So don't try to put it in the public/image folder to write it out as follows: 

>
> <img src="../public/images/image1.png" alt="image1"/>
>

## Resources
 - [Import React Images: YT - Esterling Accime](https://youtu.be/taMJct5oeoI?si=mr43z-iaV8xu2dgc)