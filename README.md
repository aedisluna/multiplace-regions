# MultiPlace — пакеты карт

Этот публичный репозиторий содержит только подготовленные данные карт и каталог загрузок. Исходники приложения, пользовательские вложения, поисковые запросы и геолокация сюда не публикуются.

## Москва · тестовый район

[Скачать пакет .mpregion](https://github.com/aedisluna/multiplace-regions/releases/download/moscow-sample-2026-10-10/moscow-sample-2026-10-10.mpregion) — 19,445,309 байт; 56 110 мест OpenStreetMap. Покрытие: долгота 37.575–37.720, широта 55.725–55.825. Это небольшой район, не вся Москва. Zoom карты 10–15, увеличение в приложении до 18.

SHA-256: `5b9629c2b46856b7e3914a318121b5ab8d8727d20b30cf07b5be13b7eda7bfa8`.

В MultiPlace откройте «Карты и регионы» → «Скачать и использовать» либо «Установить пакет из файла». После установки карта и поиск работают без сети. В ZIP входят manifest, PMTiles, SQLite, локальный стиль и ZIP подписей/шрифта. Все размеры и контрольные суммы указаны в manifest; SQLite базы предоставляются внутри архива.

[Каталог для приложения](https://github.com/aedisluna/multiplace-regions/releases/latest/download/regions.json). Загрузки происходят только по запросу пользователя. Аккаунт и токен GitHub приложению не нужны.

## Адреса и происхождение

POI и адресные ориентиры: [OpenStreetMap France, московский extract](https://download.openstreetmap.fr/extracts/russia/central_federal_district/), снимок 2026-10-09T00:30:14Z, SHA-256 входного PBF `1e373d80a6c6b5ed1163159c9e692d301cef9efc36cf124799b34a2bd7146ba7`. Карта: [Protomaps snapshot 20261008](https://build.protomaps.com/20261008.pmtiles), OSM 2026-10-08T04:00:00Z. Сведения и хэши шрифта — в [SOURCES.json](SOURCES.json).

Адрес берётся из улицы/номера самого POI или содержащего его адресованного здания. Иначе указан ближайший известный дом с пометкой «Рядом» и расстоянием до ориентира; это не подтверждённый адрес организации. Точность и актуальность зависят от OSM. Импорт сохраняет только поля места, координаты и происхождение; авторы OSM, uid/changeset, контакты/email и исходные теги не переносятся.

## Лицензии

© OpenStreetMap contributors. Данные OSM, включая базу мест и адресное обогащение: [Open Database License 1.0](https://opendatacommons.org/licenses/odbl/1-0/), [атрибуция OSM](https://www.openstreetmap.org/copyright). Доступная внутри пакета SQLite содержит производную базу в машиночитаемом виде; описание преобразования приведено выше.

Natural Earth: [public domain](https://www.naturalearthdata.com/about/terms-of-use/). Noto Sans Regular: [SIL Open Font License 1.1](https://openfontlicense.org/), полный OFL.txt включён в labels ZIP. Локальный стиль: MIT; предоставляется с разрешением использовать, копировать, изменять и распространять, без гарантий. Лицензии составных данных сохраняются.
