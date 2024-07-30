# NSFW-Data

NSFW data — это порнографические данные, собранные из разных источников.

[delete bad urls](https://github.com/Serfetto/NSFW-Data/blob/main/delete_bad_urls.ipynb) - Ноутбук, который удаляет из текстового файла репозитория неоткрывающиеся ссылки из репозиториев [alex000kim/nsfw_data_scraper](https://github.com/alex000kim/nsfw_data_scraper) или [yuanyuanhuiyi/alexkimxyz](https://github.com/yuanyuanhuiyi/alexkimxyz). Чтобы изменить когда сохранять файл измените в коде вот эту строчку: 

```path_to_file = f"/content/nsfw_data_scraper/raw_data/{folder}/new_urls_{folder}.txt"```

[new_raw_data](https://github.com/Serfetto/nsfw_data/tree/main/new_raw_data) — это папка, содержащая текстовые файлы со ссылками на фотографии в жанрах hentai, porn, sexy и neutral, а также на рисунки. Данные были взяты из репозитория [yuanyuanhuiyi/alexkimxyz](https://github.com/yuanyuanhuiyi/alexkimxyz), который был создан около 5 лет назад. Некоторые ссылки в репозитории перестали работать, поэтому я решил обработать неработающие ссылки. На момент публикации этого репозитория в нём содержатся все рабочие ссылки.

[nsfw_detect](https://huggingface.co/datasets/deepghs/nsfw_detect) — это размеченный датасет, аналогичный первому. Я не проверял, не повторяются ли в них фотографии из первого набора данных.

Фотографии с сайта rule34 были получены с помощью библиотеки [pyrule34](https://github.com/Hypick122/pyrule34), которая позволила получить данные с сайта и расширить набор фотографий на тематику хентая. Ноутбук [Parse_images_from_rule34.ipynb](https://github.com/Serfetto/NSFW-Data/blob/main/Parse_images_from_rule34.ipynb). 

```num_of_pages``` - вы можете изменить эту настройку, чтобы сайт загружался с определённой страницы.

```tags``` - вы можете изменить эту переменную, чтобы указать, по каким тегам будет выполняться поиск на сайте. Для этого нужно указать список строк.

[hentai pack](https://drive.google.com/drive/folders/13rMPxoGLIsfq8XNqBh0B7qg2a1mP91Cn?usp=sharing) — это личный набор фотографий с хентаем, собранный из разных источников в интернете. В нём около 3500 фотографий.

[images_links.txt](https://drive.google.com/file/d/1VwqsUvuw11htJ2Dqs5PShg7QGq5a7VLs/view?usp=sharing) - текстовый файл, в котором содержится около 1 600 000 ссылок на порнографические фотографии. Взято с данного [датасета](https://pastebin.com/xb4X99cq)

Также есть другой [датасет](https://archive.org/details/dataset-nude), скачанный с торрента, который содержит фотографии в жанрах хентай и порно, разделённые на папки train, test и validation. Классы, на которые они разделены: nude (обнажённые) и safe (безопасные).
