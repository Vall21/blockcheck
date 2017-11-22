

BlockCheck v0.0.9.6
+

Для получения корректных результатов используйте DNS-сервер провайдера и отключите средства обхода блокировок.


Проверка работоспособности IPv6: IPv6 недоступен.
IP: 37.20.174.xxx, провайдер: Kemerovo Regional Telegraph, branch of Kuzbass Pub/ Ростелеком МРФ "Сибирь"


[O] Тестируем IPv4 DNS
	Через системный DNS:	 ['184.173.136.161', '195.8.215.136', '195.82.146.214', '5.178.68.100', '95.167.13.50', '95.167.13.50']
	Через Google DNS:	 ['104.20.134.45', '104.20.135.45', '104.24.10.70', '104.24.11.70', '184.173.136.161', '195.8.215.136', '195.82.146.214', '5.178.68.100']
	Через Google API:	 ['104.20.134.45', '104.20.135.45', '104.24.10.70', '104.24.11.70', '184.173.136.161', '195.8.215.136', '195.82.146.214', '5.178.68.100']
	Несуществующий DNS не вернул адресов (это не ошибка)
[☠] DNS-записи подменяются
[✓] DNS не перенаправляется

[O] Тестируем HTTP (по настоящим IP-адресам сайтов)
	Открываем  http://a.putinhuylo.com/
[✓] Сайт открывается
	Открываем  http://furry.booru.org/
[✓] Сайт открывается
	Открываем  http://furry.booru.org/index.php?page=post&s=view&id=111173
[☠] Получен неожиданный ответ, скорее всего, страница-заглушка провайдера. Пробуем через прокси.
[✓] Сайт открывается через прокси
	Открываем  http://pbooru.com/
[✓] Сайт открывается
	Открываем  http://pbooru.com/index.php?page=post&s=view&id=303026
[☠] Получен неожиданный ответ, скорее всего, страница-заглушка провайдера. Пробуем через прокси.
[✓] Сайт открывается через прокси
	Открываем  http://rutracker.org/forum/index.php
[☠] Получен неожиданный ответ, скорее всего, страница-заглушка провайдера. Пробуем через прокси.
[✓] Сайт открывается через прокси

[O] Тестируем HTTPS
	Открываем  https://e621.net/
[☠] Сайт не открывается
	Открываем  https://lolibooru.moe/
[☠] Сайт не открывается
	Открываем  https://rutracker.org/forum/index.php
[☠] Сайт не открывается
	Открываем  https://www.dailymotion.com/
[☠] Сайт не открывается

[O] Тестируем обход DPI
	Пробуем способ «дополнительный пробел после GET» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «заголовок hOSt вместо Host» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «заголовок hoSt вместо Host» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «значение Host БОЛЬШИМИ БУКВАМИ» на pbooru.com
[!] Сайт не открывается, обнаружен пассивный DPI!
	Пробуем способ «необычный порядок заголовков» на pbooru.com
[!] Сайт не открывается, обнаружен пассивный DPI!
	Пробуем способ «отсутствие пробела между двоеточием и значением заголовка Host» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «перенос строки в заголовках в UNIX-стиле» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «перенос строки перед GET» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «табуляция в конце домена» на pbooru.com
[☠] Сайт не открывается
	Пробуем способ «точка в конце домена» на pbooru.com
[!] Сайт не открывается, обнаружен пассивный DPI!
	Пробуем способ «фрагментирование заголовка» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «фрагментирование заголовка, hoSt и отсутствие пробела одновременно» на pbooru.com
[✓] Сайт открывается
	Пробуем способ «дополнительный пробел после GET» на rutracker.org
[!] Сайт не открывается, обнаружен пассивный DPI!
	Пробуем способ «заголовок hOSt вместо Host» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «заголовок hoSt вместо Host» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «значение Host БОЛЬШИМИ БУКВАМИ» на rutracker.org
[!] Сайт не открывается, обнаружен пассивный DPI!
	Пробуем способ «необычный порядок заголовков» на rutracker.org
[!] Сайт не открывается, обнаружен пассивный DPI!
	Пробуем способ «отсутствие пробела между двоеточием и значением заголовка Host» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «перенос строки в заголовках в UNIX-стиле» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «перенос строки перед GET» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «табуляция в конце домена» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «точка в конце домена» на rutracker.org
[!] Сайт не открывается, обнаружен пассивный DPI!
	Пробуем способ «фрагментирование заголовка» на rutracker.org
[✓] Сайт открывается
	Пробуем способ «фрагментирование заголовка, hoSt и отсутствие пробела одновременно» на rutracker.org
[✓] Сайт открывается

[!] Результат:
[⚠] Ваш провайдер подменяет DNS-записи, но не перенаправляет сторонние IPv4 DNS-серверы на свой.
 Вам поможет смена DNS, например, на Яндекс.DNS 77.88.8.8 или Google DNS 8.8.8.8 и 8.8.4.4.
[⚠] Ваш провайдер полностью блокирует доступ к HTTPS-сайтам из реестра.
[⚠] У вашего провайдера "обычный" DPI. Вам поможет HTTPS/Socks прокси, VPN или Tor.
