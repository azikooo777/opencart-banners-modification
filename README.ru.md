# OpenCart Модификатор Баннеров
Добавляет в Баннеры **Описание** для OpenCart 3.x

# Установка

Перейдите **Модули/Расширения -> Установка расширений**

Затем кликните по синий кнопки Загрузить и предоставте путь к файлу "banner_modification.ocmod.zip" archive.

Затем Перейдите **Модули/Расширения -> Модификаторы** и кликните по синий кнопки обновить

# ВАЖНО

Вы должны иметь привелегии ALTER MySql.

===============================================================================

# ПРИМЕР

Перейдите **Дизайн -> Баннеры** и выберите ваш баннер или добавте новый и вы должны увидеть новое поля **описание**. Ниже приведен пример с изображением того как должно выглядеть

![Example 1](https://github.com/azikooo777/opencart-banners-modification/blob/master/images/example-1.png)

Давайте напишем текст **example** и сохраним.

Теперь мы имеем новую переменую description в массиве banners
и эта переменая доступна на сдедуших шаблонах
  * **catalog/view/theme/your-theme-name or default/template/extension/module/slideshow.twig**
  * **catalog/view/theme/your-theme-name or default/template/extension/module/carousel.twig**
  * **catalog/view/theme/your-theme-name or default/template/extension/module/banner.twig**
  
Давайте отобразим наш ранее написаный текст **example**. Я написал этот текст в баннере slideshow.

Перейдем в **catalog/view/theme/your-theme-name or default/template/extension/module/slideshow.twig**. Ниже приведен пример с изображением кода до.

![Image Before](https://github.com/azikooo777/opencart-banners-modification/blob/master/images/example-2.png)

Я добавил код {{banner.description}}. Ниже приведен пример с изображением кода после.

![Image After](https://github.com/azikooo777/opencart-banners-modification/blob/master/images/example-3.png)

Теперь давайте перейдем на наш сайт и мы должны увидеть текст **example**. Ниже приведен пример с изображением того как выглядит.

![Image Last](https://github.com/azikooo777/opencart-banners-modification/blob/master/images/example-4.png)
