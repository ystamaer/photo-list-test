# Техническое задание:

Средствами Vue.js реализуйте функционал для вывода и фильтрации списков фотографий.

**[Макет](https://www.figma.com/file/RRmuLYCS4pBbi7GCNivt5V/photobank-filter?node-id=3%3A0)**

Приложение состоит из одной страницы с попапом в центре, в котором отображается [список фотографий](http://jsonplaceholder.typicode.com/photos). Размер попапа имеет фиксированную высоту.
Ячейки с названиями фото выводятся внутри попапа в 4 равные колонки. Если высота колонки больше высоты попапа - следует реализовать внутренний скролл.

[ПРИМЕР реализации со скроллом](https://www.figma.com/proto/RRmuLYCS4pBbi7GCNivt5V/photobank-filter?node-id=3%3A0&viewport=2116%2C1124%2C0.5&scaling=min-zoom)

### Реализация в 2 этапа

#### 1 этап
Необходимо вывести список фотографий на странице, как в макете. 
По-умолчанию список фото выводится в алфавитном порядке. 
Все названия начинающиеся с одинаковой буквы формируются в блоки, где первым элементом является первая буква.
Не допускается разрыв блока по разным колонкам.

Каждый элемент списка должен содержать миниатюру изображения, название файла, символ “сердечко” - добавить в избранное. Или символ “х” - удалить из избранного (если уже в избранном).

####2 этап
**В header попапа отображаются 2 названия фильтров**

- “По альбомам”
- “Избранное"

**При выбранном фильтре “По альбомам”** - в попапе отображается список фотографий объединенных в блоки по альбомам. Первый элемент блока - название альбома. Блоки с альбомами выводятся по алфавиту.

**При выбранном фильтре “Избранное”** - в попапе отображается список фотографий. Формат вывода - по умолчанию.

Списки фото, а также их миниатюры доступны [тут](http://jsonplaceholder.typicode.com/photos). Для удобства использования в попапе следует выводить не более 32-х альбомов. Каждый из которых может содержать 5-10 элементов.

## Требования к функционалу:

- Все действия на сайте должны происходить без перезагрузки страницы.
- После перезагрузки страницы состояние списка должно сохраняться.

## Технические требования:

- В качестве языка разработки используется JavaScript библиотека Vuejs.
- В качестве препроцессора SCSS.
- Верстка должна быть выполнена в соответствии с данным шаблоном. Без использования UI библиотек.
- Адаптивность не обязательна, но приветствуется.
- Логика приложения должна быть разбита на разумное количество самодостаточных Vue-компонентов.

## Тестовое задание должно быть представлено в следующем виде:

- Ссылка на публичный репозиторий (GitHub, BitBucket, GitLab) с исходным кодом.
- Ссылка на сайт для тестирования функционала будет плюсом.

## Особое внимание стоит обратить на следующие моменты:

- Код должен быть написан понятно и аккуратно, с соблюдением табуляции и прочих элементов написания, без лишних элементов и функций, не имеющих отношения к функционалу тестового задания.
- Читабельность и наличие элементарной архитектуры.
- Чистота и оформление кода — не менее важный фактор. Код должен быть написан в едином стиле (желательно в рекомендуемом для конкретного языка). Также к чистоте относятся отсутствие копипаста и дублирования логики.

[ТЗ по внешней ссылке](https://docs.google.com/document/d/1afrk0V5KPFZSeaR5dG6QODKAgy8RB9YuX566jBrHZcQ/edit)