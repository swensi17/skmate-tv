# SkMate IPTV на телевизоре LG (webOS)

SkMate для LG ставится файлом `.ipk` через режим разработчика LG и бесплатную программу **webOS Dev Manager**. В магазине LG приложения нет.

> Сборка для LG сделана из того же кода, что и для Samsung, но на телевизоре LG её ещё не проверяли. Если что-то не работает, напишите в [Issues](https://github.com/swensi17/skmate-tv/issues) или в Telegram [@swensi17](https://t.me/swensi17).

## Какие телевизоры подходят

| Год | webOS | Работает |
|---|---|---|
| 2018 и новее | 4.0 и новее | должно работать (не проверено) |
| 2017 и старше | 3.x и ниже | нет: браузер телевизора слишком старый |

Версия webOS: «Настройки» → «Поддержка» → «Информация о ТВ» (названия пунктов зависят от модели).

## Что нужно

- Телевизор LG и компьютер с Windows, macOS или Linux в одной сети Wi-Fi.
- Бесплатный аккаунт разработчика LG.
- Около 15 минут один раз.

## Шаг 1. Аккаунт разработчика LG

1. На компьютере откройте https://webostv.developer.lge.com и войдите или создайте аккаунт LG.
2. Подтвердите почту.

## Шаг 2. Режим разработчика на телевизоре

1. На телевизоре откройте магазин **LG Content Store** и найдите **Developer Mode**. Установите.
2. Запустите **Developer Mode** и войдите в аккаунт из шага 1.
3. Включите **Dev Mode Status**. Телевизор перезагрузится.
4. Снова откройте **Developer Mode** и включите **Key Server**.

## Шаг 3. webOS Dev Manager на компьютере

1. Скачайте webOS Dev Manager для своей системы: https://github.com/webosbrew/dev-manager-desktop/releases/latest
2. Установите и запустите.
3. Добавьте телевизор: укажите его IP-адрес. Если программа попросит **Passphrase**, этот код показан в приложении Developer Mode на телевизоре.

## Шаг 4. Поставить SkMate

1. Скачайте файл: [SkMate-IPTV-webos.ipk](https://github.com/swensi17/skmate-tv/releases/latest/download/SkMate-IPTV-webos.ipk)
2. В webOS Dev Manager откройте список приложений телевизора и установите этот файл.
3. На телевизоре SkMate IPTV появится в списке приложений.

## Важно: срок режима разработчика

- Режим разработчика LG работает до **1000 часов** (около 41 дня). Когда срок кончается, телевизор **удаляет** приложения, поставленные так, и SkMate тоже.
- Чтобы этого не было, время от времени открывайте **Developer Mode** и нажимайте **EXTEND**: срок начнётся заново.
- Если срок уже кончился, включите режим разработчика заново и поставьте SkMate ещё раз.
- С одного аккаунта разработчика режим работает только на одном телевизоре.

## Обновление

Скачайте новый `SkMate-IPTV-webos.ipk` и поставьте его так же, как в шаге 4.

## Если не получается

- **Dev Manager не находит телевизор**: телевизор и компьютер должны быть в одной сети; после перезагрузки телевизора снова включите **Key Server** в Developer Mode. IP телевизора может смениться: лучше закрепить его в настройках роутера.
- **SkMate пропал с телевизора**: кончился срок режима разработчика, см. выше.

---

*Для разработчиков.* Пакет собирается командой `npm run package` (папка `web/release/webos`), затем `ares-package --no-minify web/release/webos` из webOS CLI. `--no-minify` нужен, чтобы упаковщик не переписывал уже собранный код. ID приложения: `uz.skmate.iptv`.

---

# SkMate IPTV on LG TVs (webOS)

Install the `.ipk` file through LG Developer Mode and the free **webOS Dev Manager**. The app is not in the LG Content Store. The LG build uses the same code as the Samsung build but has not been tested on an LG TV yet.

Supported: webOS 4.0 and newer (2018+ models), not tested. webOS 3.x and older: no.

1. Create or sign in to an LG account at https://webostv.developer.lge.com.
2. On the TV: install **Developer Mode** from the LG Content Store, sign in, turn on **Dev Mode Status** (the TV restarts), then turn on **Key Server**.
3. On the computer: install [webOS Dev Manager](https://github.com/webosbrew/dev-manager-desktop/releases/latest) and add the TV by its IP (the passphrase, if asked, is shown in the Developer Mode app).
4. Download [SkMate-IPTV-webos.ipk](https://github.com/swensi17/skmate-tv/releases/latest/download/SkMate-IPTV-webos.ipk) and install it from Dev Manager.

Developer Mode lasts up to 1000 hours; when it expires, the TV removes sideloaded apps. Press **EXTEND** in the Developer Mode app from time to time.
