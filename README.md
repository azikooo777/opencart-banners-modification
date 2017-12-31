# opencart-banners-modification
Add in Baners Description for OpenCart 3.x

# INSTALL

Go to Extension **Extensions -> Installer**

Then click the blue Upload button and provide the route to your extension "banner_modification.ocmod.zip" archive.

Then go to **Extensions -> Modifications** click the blue refresh button

# IMPORTANT 

After installation. Go to **Design -> Banners** to create 
automatically column **description** in table tablePrefix_banner_image. Since opencart 3.x does not support index.php and install.sql when installing.

===============================================================================

# EXAMPLE

Go to **Design -> Banners** and choose your banner or add new banner and you should see a new field description. Below is an example of an image, as should look
![Example 1](https://github.com/azikooo777/opencart-banners-modification/blob/master/images/example-1.png)

Let's write the text **example** and save.

now we have a new variable description in banners array 
and it is available in the following templates
  * **catalog/view/theme/your-theme-name or default/template/extension/module/slideshow.twig**
  * **catalog/view/theme/your-theme-name or default/template/extension/module/carousel.twig**
  * **catalog/view/theme/your-theme-name or default/template/extension/module/banner.twig**
  
Let's display our previously written text **example**. I wrote. This text in slideshow.

Go to **catalog/view/theme/your-theme-name or default/template/extension/module/slideshow.twig** bellow example image code before
![Image Before](https://octodex.github.com/images/yaktocat.png)
I add code {{banner.description}}. bellow example image code after
![Image After](https://octodex.github.com/images/yaktocat.png)

Now go to our site and you should text **example** bellow example image
![Image After](https://octodex.github.com/images/yaktocat.png)
