# OpenCart Banners Modification
Add in Baners **Description** for OpenCart 3.x

# INSTALL

Go to **Extensions -> Installer**

Then click the blue Upload button and provide the route to your extension "banner_modification.ocmod.zip" archive.

Then go to **Extensions -> Modifications** click the blue refresh button

# IMPORTANT 

You must have ALTER privilege MySql.

===============================================================================

# EXAMPLE

Go to **Design -> Banners** and choose your banner or add new banner and you should see a new field **Description**. Below is an example of an image, as should look

![Example 1](https://github.com/azikooo777/opencart-banners-modification/blob/master/images/example-1.png)

Let's write the text **example** and save.

Now we have a new variable **description in banners array** 
and it is available in the following templates
  * **catalog/view/theme/your-theme-name or default/template/extension/module/slideshow.twig**
  * **catalog/view/theme/your-theme-name or default/template/extension/module/carousel.twig**
  * **catalog/view/theme/your-theme-name or default/template/extension/module/banner.twig**
  
Let's display our previously written text **example**. I wrote this text in banners slideshow.

Go to **catalog/view/theme/your-theme-name or default/template/extension/module/slideshow.twig**. Bellow example image code before.

![Image Before](https://github.com/azikooo777/opencart-banners-modification/blob/master/images/example-2.png)

I add code {{banner.description}}. Bellow example image code after.

![Image After](https://github.com/azikooo777/opencart-banners-modification/blob/master/images/example-3.png)

Now go to our site and you should text **example**. Bellow example image.

![Image Last](https://github.com/azikooo777/opencart-banners-modification/blob/master/images/example-4.png)
