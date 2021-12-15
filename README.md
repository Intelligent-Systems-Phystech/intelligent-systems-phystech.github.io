# Machine Learning Phystech WebSite

## Добавление курса: TODO --- сейчас не актуально
Для добавления нового курса требуется создать файл `course_name.md` в папке `_course/`. Далее требуется заполнить метаинформацию о курсе:
```
---
title: Сюда вписать названия курса (название которое во вкладке браузера )
name: Продублировать название курса (название которое будет на сайте)
type: bachelor (курс из бакалавриата или магистратуры, валидные поля bachelor/master)
avatar: название изображению в папке images/course (если поле пустое, то будет взято default.jpg изображение)
lecturers: лекторы через запятую, в качестве идентификатора использовать название файлов (без приставки .md) в папке _people (например strijov_vv,grabovoy_av)
site: основной сайт курса (можно не указывать), ВАЖНО! Без приставки https://
---
```

После заполенения метаинформации требуется указать описание самого курса в формате markdown.

## Добавление пользователя:  TODO --- сейчас не актуально
Для добавления нового пользователя требуется создать файл `lecturer_name.md` в папке `_people/`. Далее требуется заполнить метаинформацию о лекторе:
```
---
title: Сюда вписать имя фамилию преподавателя (название которое во вкладке браузера )
name: Продублировать имя преподавателя (так как на сайте будет)
position: phd (начная степень преподавателя или должность, возможные значения смотрите тут https://github.com/Intelligent-Systems-Phystech/intelligent-systems-phystech.github.io/blob/master/_config.yml#L81)
avatar: название изображению в папке images/people (если поле пустое, то будет взято default.jpg изображение)
mail: почта преподавателя (может быть пусто)
site: сайт преподавателя (может быть пусто)
scholar: ссылка на scholar (может быть пусто)
---
```

Вся дополнительная информация указывается ниже в формате markdown.

## Исправления текста локализации en/ru

Английский язык: [ссылка](https://github.com/Intelligent-Systems-Phystech/intelligent-systems-phystech.github.io/blob/master/_i18n/en.yml)

Русский язык: [ссылка](https://github.com/Intelligent-Systems-Phystech/intelligent-systems-phystech.github.io/blob/master/_i18n/ru.yml)

## Изменения страницы HOME

Метаинформация страницы: [ссылка](https://github.com/Intelligent-Systems-Phystech/intelligent-systems-phystech.github.io/edit/master/index.md)

Английская версия: [ссылка](https://github.com/Intelligent-Systems-Phystech/intelligent-systems-phystech.github.io/blob/master/_i18n/en/index.md)

Русская версия: [ссылка](https://github.com/Intelligent-Systems-Phystech/intelligent-systems-phystech.github.io/blob/master/_i18n/ru/index.md)

## Изменения страницы ABOUT

Метаинформация страницы: [ссылка](https://github.com/Intelligent-Systems-Phystech/intelligent-systems-phystech.github.io/edit/master/about.md)

Английская версия: [ссылка](https://github.com/Intelligent-Systems-Phystech/intelligent-systems-phystech.github.io/blob/master/_i18n/en/about.md)

Русская версия: [ссылка](https://github.com/Intelligent-Systems-Phystech/intelligent-systems-phystech.github.io/blob/master/_i18n/ru/about.md)

## Изменения страницы Applicants

Метаинформация страницы: [ссылка](https://github.com/Intelligent-Systems-Phystech/intelligent-systems-phystech.github.io/edit/master/applicants.md)

Английская версия: [ссылка](https://github.com/Intelligent-Systems-Phystech/intelligent-systems-phystech.github.io/blob/master/_i18n/en/applicants.md)

Русская версия: [ссылка](https://github.com/Intelligent-Systems-Phystech/intelligent-systems-phystech.github.io/blob/master/_i18n/ru/applicants.md)
