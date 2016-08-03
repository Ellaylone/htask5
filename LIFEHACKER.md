# LIFEHACKER.RU

![DevTools Audit resources](https://cloud.githubusercontent.com/assets/4200528/17379662/15aa35f2-59cc-11e6-91d6-5afb81b691f3.jpg)

Большое количество JS и CSS файлов, каждый из них - дополнительный запрос. Нужно объединить и минифицировать JS и CSS файлы. 

![PageSpeed Insights js in head](https://cloud.githubusercontent.com/assets/4200528/17380106/0e9c5a90-59ce-11e6-9a00-4e8c4d493003.jpg)

JS в начале страницы замедляет отображение контента - нужно переместить его из начала файла в конец или использовать async/defer чтобы не блокировать html рендеринг. 

На главной странице подгружается большое количество неиспользуемого css - DevTools Audit показывает до 89% неиспользованных css правил, есть смысл подгружать изначально только правила необходимые на странице.

![DevTools Audit css](https://cloud.githubusercontent.com/assets/4200528/17379600/d0b89b50-59cb-11e6-990b-743a794ca334.jpg)

Так же стоит сжать изображения, сделать спрайты для иконок, использовать srcset или тэг picture для загрузки изображений разного размера под разные платформы.

Подключить gzip сжатие и кеш для статики позволят значительно уменьшить объем загружаемых данных.

![PageSpeed Insights cache](https://cloud.githubusercontent.com/assets/4200528/17379592/c99d7dea-59cb-11e6-9ce9-a6ee04acbda5.jpg)
![PageSpeed Insights gzip](https://cloud.githubusercontent.com/assets/4200528/17379591/c99b220c-59cb-11e6-9f18-b118c6d5f0c2.jpg)
