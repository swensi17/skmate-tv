# Политика конфиденциальности SkMate IPTV для Smart TV

Действует с 26 ноября 2026 года. Относится к приложению SkMate IPTV для телевизоров Samsung (Tizen) и LG (webOS).

## Коротко

- Аккаунт не нужен. Мы не собираем и не храним ваши персональные данные на своих серверах.
- Нет рекламы, аналитики и счётчиков.
- Всё, что вы вводите (плейлисты, логины Xtream, PIN-коды, избранное, настройки), хранится **только на вашем телевизоре**.

## Какие данные хранятся на телевизоре

Плейлисты и их адреса, логины и пароли Xtream Codes, избранное, история просмотра, телепрограмма, профили, PIN-коды и настройки. Эти данные остаются на устройстве и удаляются вместе с приложением.

## Куда приложение подключается

Приложение обращается только к тем серверам, которые нужны для работы функций:

| Что | Куда | Что передаётся |
|---|---|---|
| Ваши плейлисты и каналы | серверы, которые **вы** добавили | обычный запрос плейлиста или видео; адрес, логин и пароль, которые вы ввели |
| Телепрограмма (EPG) | адреса из вашего плейлиста и общие источники телепрограммы (например, epg.one, epg.team, epg.it999.ru, tv.team) | запрос файла программы |
| Погода на главном экране | сервисы определения города по IP (ipapi.co, ipwho.is, ip-api.com) и Open-Meteo (погода) | IP-адрес вашего подключения (виден любому серверу, к которому подключается устройство); в ответ приходит примерный город, координаты города передаются в Open-Meteo |
| Постеры фильмов (если включены) | The Movie Database (api.themoviedb.org, image.tmdb.org) | название передачи и ваш ключ TMDB |
| Защищённый DNS (если включён в настройках) | выбранный вами сервис (Google, Cloudflare, Quad9) | имена серверов, к которым подключается приложение |
| Плейлист SkMate (если вы выбрали его) | сервер автора приложения | запрос плейлиста |

Эти сервисы работают по своим правилам конфиденциальности. Мы не передаём им ничего сверх того, что указано в таблице.

## Дети

Приложение не предназначено для сбора данных детей. Категории для взрослых скрыты, пока их не открыть PIN-кодом.

## Изменения

Если политика изменится, новая версия появится на этой странице с новой датой.

## Связь

Telegram: [@swensi17](https://t.me/swensi17) · GitHub: [swensi17/skmate-tv](https://github.com/swensi17/skmate-tv/issues)

---

# Privacy Policy — SkMate IPTV for Smart TV

Effective 26 November 2026. Applies to SkMate IPTV for Samsung (Tizen) and LG (webOS) TVs.

- No account. We do not collect or store your personal data on our servers. No ads, analytics or trackers.
- Everything you enter (playlists, Xtream logins, PINs, favourites, settings) is stored **only on your TV** and is removed with the app.
- The app connects only to: the playlist and stream servers **you** add; TV-guide sources (from your playlist and common public sources); IP-based city lookup (ipapi.co, ipwho.is, ip-api.com) and Open-Meteo for the weather on the home screen (your connection's IP address is seen by these services; the approximate city's coordinates go to Open-Meteo); The Movie Database for posters if you enable it with your own key; the secure-DNS provider you choose, if enabled; the author's server, if you choose the SkMate playlist.
- These services have their own privacy policies. We send them nothing beyond the above.
- Adult categories stay hidden until unlocked with a PIN.
- Contact: Telegram [@swensi17](https://t.me/swensi17), GitHub [issues](https://github.com/swensi17/skmate-tv/issues).
