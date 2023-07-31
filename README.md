# Magicbook Pro 16.1 Hackintosh 2019&2020 Стабильная версия Black Apple [адаптация для AMD]

> Установите macOS Monterey 12.4 21F79 на Honor Magicbook Pro 2019&2020
> _Адаптация репозитория под версию AMD Ryzen 5_

### Характеристики 

|     Параметр      | Honor на Intel                                    | Honor на AMD (мой)           |
| :---------------: | :------------------------------------------------ | :--------------------------- |
|      Модель       | Magicbook Pro 2019&2020                           | Magicbook Pro 2020 HLYL-WFQ9 |
|       CPU1        | Intel Whiskey Lake i3-8145U & i5 8265U & i7-8565U | AMD Ryzen 5 4600H            |
|       CPU2        | Intel Comet Lake i5-10210u & i7-10710U            |                              |
|       RAM         | DDR4 2666 МГц 8 Гб                                | DDR4 МГц 2666 16 Гб          |
| Графическая карта | Intel UHD620 2048 MB & NVIDIA MX250               | AMD Radeon(TM) Graphics      |
|    Видеокарта     | NVIDIA GeForce MX250 (недоступно)                 | AMD Radeon Vega 6            |
|   Жёсткий диск    | HS (Hikvision) C2000 Pro 1TB*                     | SSD 512 Гб                   |
|  Звуковая карта   | Realtek ALC 256                                   | Realtek ALC 256              |
|      Тачпад       | ELAN 2204                                         |                              |
|       Экран       | Full HD (1920x1080)                               | Full HD (1920x1080)          |
|      SMBIOS       | Macbook Pro 15,4                                  |                              |
|      Clover       | Обновлён до 5100                                  |                              |
|     OpenCore      | Обновлён до 0.8.1                                 |                              |
|       macOS       | До версии Monterey Release 12.4                   |                              |

\* Купите и замените самостоятельно. [Почему?](###В настоящее время жёсткий диск Samsung PM981 может использовать только Clover)

### О выпуске Magicbook Pro (2020 г.)

Адаптация 2020 года завершена, функции работают нормально, а ситуация с использованием такая же, как и в версии 2019 года!

### О выпуске Magicbook Pro (2019 г.)

Эта группа была адаптирована к версиям Magicbook для непрофессионалов (i3, i5, i7) 2019 и 2020 годов выпуска, синхронизировав все обновленные функции

### Долгосрочное обновление

Я получил электронные письма от друзей, которые помогали с тестированием, и все они предложили провести мне вести долгосрочное обновление за символическую плату. Если вы считаете, что оно того стоит, пожалуйста, оплатите технические услуги (QR-код удалён) и получите бесплатные обновления для технического обслуживания на более позднем этапе.
Теоретически, репозиторий будет постоянно обновляться на официальном сайте Honor. Стоймость ноутбука можно узнать на Taobao (или на Яндекс Маркете), чтобы опредилить цену Black Apple, установка tb пока не обновит вас (что за бред?!). 

> Более того, "Установка", "Стабильное использование" и "Долгосрочное обновление" Black Apple — это три совершенно разных понятия. Смысл Black Apple заключается в обновлении и его обслуживании. 

Просто пригласите владельца группы на чашечку кофе. Он вложил сотни или даже тысячи часов напряженной работы в этот EFI. В настоящее время для новой версии необходим пароль, который находится в группе.
Есть подробное восстановление Clover/OpenCore/PM981 используя руководство по установке метода в группе, а также восторженные рекомендации владельца группы и единомышленики. Xiaobai может быстрее помочь вам!
Присоединяйтесь к группе за сумму более 9,9 юаней\*. Посмотрите на неё и передайте в группу QQ номер 963407871

> Курс 9,9 юаней к рублю (с округлением):
>
> -  31 июля 2023 г. — 128 рублей,
> -  10 июня 2020 г. — 100 рублей (последнее редактирвоание README).

### В группе уже есть встроенный тестовый драйвер Intelwifi и в его ежедневном использовании нет ничего плохого.

### Оборудование доступное в настоящее время

-  Intel 9560 CNVi Wi-Fi（идеально подходит для ежедневного использования, MagicBook Pro 2020 г. также поддерживает)
-  Выходы USB-C/HDMI (выход одновременно нормальный, плюс в общей сложности 4 монитора с Suihang в порядке, профессиональный тест!）
-  [Relay](https://www.imore.com/how-use-icloud-private-relay-mac#section-what-is-icloud) ([Handoff](https://support.apple.com/ru-ru/HT209455))
-  [Suihang](https://russianblogs.com/article/43853362863/) (sidecar) (имеет проводное подключение, но беспроводное временно недоступно)
-  Airdrop временно недоступен
-  Основная видеокарта
-  Тачпад (поддерживает многозадачные жесты)
-  Bluetooth (Может быть запущен холодным способом, может включаться и выключаться, подключение нормальное)
-  Динамик/гарнитура/микрофон (AppleALC)
-  USB3.0/2.0
-  Регулировка яркости монитора (системные настройки монитора)
-  Регулировка яркости (F1, F2), подсветка клавиатуры (F3), регулировка громкости (F4 – отключение звука, F5 – уменьшение громкости, F6 – увеличение громкости)
-  Индикатор уровня заряда батареи (быстрая зарядка в норме)
-  Закройте для спящего режима и откройте для выхода из него
-  Преобразование частоты процессора, турбо-частота, гиперпоточность - это нормально

Преобразование частоты процессора, турбо-частота и гиперпоточность являются нормальными (эмм... как это перевести...)

### Обновлять OpenCore

– 2022.6.10 v8.1 Release только для Monterey

1. Обновление до версии OpenCore 0.8.1
2. Поскольку конфигуратор Opencore еще не адаптирован к версии 0.8.1, пожалуйста, нажмите настройки в левом верхнем углу при его использовании. На второй странице измените атрибут версии на версию разработки 0.8.1!
3. Адаптация к официальной версии macOS Monterey 12.4 21F79
4. Исправлены проблемы с загрузочной картой и заставкой, с которыми сталкивались некоторые друзья по группе

– 2022.4.23 v8.0 Release только для Monterey

1. Обновление до версии OpenCore 0.8.0
2. Обновите пакет семейства драйверов
3. Адаптация к официальной версии macOS Monterey 12.3.1 21E258
4. Некоторые корректировки деталей

– 2022.1.15 v6.7 Release только для Monterey

1. Обновление до версии OpenCore 0.7.7 Release
2. Обновите пакет семейства драйверов
3. Обновите драйвер Wi-Fi до Airportitlwm-v2.1.0-stable
4. Обновите драйвер Bluetooth до IntelBluetoothFirmware-v2.1.0-stable
5. Адаптирован к MacOS Monterey 12.1 21C52 (Официальная версия)

– 2021.11.11 v6.5 Release только для Monterey

1. Обновление до версии OpenCore 0.7.5 Release
2. Обновите пакет семейства драйверов
3. Адаптирован MacOS Monterey 12.0.1 21A559 (Официальная версия)

– 2021.10.9 v6.4 Release for Big Sur Only

1. Обновление до версии OpenCore 0.7.4 Release
2. Обновите пакет семейства драйверов

– 2021.9.14 v6.3 Release for Big Sur Only

1. Обновление до версии OpenCore 0.7.3 Release
2. Обновите пакет семейства драйверов
3. Обновите драйвер Wi-Fi до Airportitlwm-v2.0.0-stable– 20210807
4. Адаптирован MacOS Big Sur 11.6 20EG165 (Официальная версия)

– 2021.8.8 v6.2 Release for Big Sur Only

1. Обновление до версии OpenCore 0.7.2 Release
2. Обновите пакет семейства драйверов
3. Обновите драйвер Wi-Fi до Airportitlwm-v2.0.0– 20210807
4. Адаптирован MacOS Big Sur 11.5.1 20G80 (Официальная версия)

– 2021.7.11 v6.1.1 Release

1. Обновление до версии OpenCore 0.7.1 Release
2. Обновите пакет семейства драйверов
3. Обновите драйвер Wi-Fi до Airportitlwm-v1.3.0-stable
4. Адаптирован MacOS Big Sur 11.5 20G71 (Официальная версия)

– 2021.6.10 v6.0 Release for Big Sur Only

1. Обновление до версии OpenCore 0.7.0 Release
2. Обновите пакет семейства драйверов
3. Адаптирован MacOS Big Sur 11.4 20F71 (Официальная версия)
4. Обновите драйвер Wi-Fi до Airportitlwm-v2.0.0– 20210608

– 2021.5.5 v5.9 Release for Big Sur Only

1. Обновление до версии OpenCore 0.6.9 Release
2. Обновите пакет семейства драйверов
3. Адаптирован MacOS Big Sur 11.3.1 20E241 (Официальная версия)
4. 使用 Airportitlwm-v2.0.0-Alpha，大幅提升网速(理论上可以跑满 1000M)

– 2021.4.8 v5.8 Release for Big Sur Only

1. Обновление до версии OpenCore 0.6.8 Release
2. Обновите пакет семейства драйверов
3. Адаптирован MacOS Big Sur 11.2.3 20D91 (Официальная версия)

– 2021.3.3 v5.7 Release for Big Sur Only

1. Обновление до версии OpenCore 0.6.7 Release
2. Обновите пакет семейства драйверов
3. Адаптирован MacOS Big Sur 11.2.2 20D80 (Официальная версия)
4. 修复部分群友遇到的盒盖唤醒后外接显示器黑屏的问题
5. 更新 Airportitlwm-v1.2.0-stable，减少睡眠唤醒断网的情况（网速相应也变慢了）

> Остальные версии OpenCore пока переводятся...

<!--
– 2021.2.3 v5.6 Release for Big Sur Only

1. Обновление до версии OpenCore 0.6.6 Release
2. Обновите пакет семейства драйверов
3. Адаптирован MacOS Big Sur 11.2 (Официальная версия)
4. 更新 Airportitlwm– 20210203，再次大幅提升速度和稳定性（群主自测上传 40Mbps，下载 200Mbps）


 – 2021.1.8 v5.5 Release for Big Sur Only
1. Обновление до версии OpenCore 0.6.5 Release
2. Обновите пакет семейства драйверов
3. 调整了一些性能设置
4. 更新Airportitlwm– 20210102，大幅提升速度和稳定性（自测上传30Mbps，下载100Mbps）

– 2020.12.12 v5.4 Release for Big Sur Only
1. Обновление до версии OpenCore 0.6.4 Release
2. Обновите пакет семейства драйверов
3. 更新Airportitlwm– 20201204

– 2020.11.26 v5.3.3 Release
1. 更新Airportitlwm– 20201115，提升稳定性（链接成功率，睡眠唤醒断网修复等等）

– 2020.11.16 v5.3.2 Release
1. 修复群友心心念念的下载速度显示为0的问题
2. 一些细节调整

– 2020.11.6 v5.3.1 Release
1. Адаптирован Big Sur 11.0.1 (Официальная версия)

– 2020.11.6 v5.3 Release
1. Обновление до версии OpenCore 0.6.3 Release
2. Обновите пакет семейства драйверов
3. 更新Airportitlwm
4. 支持至Big Sur Release Candidate 11.0.1
5. 一些细节改进,优化在Big Sur下的表现

– 2020.10.6 v5.2 Release
1. Обновление до версии OpenCore 0.6.2 Release
2. Обновите пакет семейства драйверов
3. 添加Z大Airportitlwm，舍弃Heliport客户端，请直接在状态栏使用系统自带wifi
4. 支持至Big Sur Developer Beta 9
5. 加入长按电源键两秒锁屏，三秒弹出“关机重启菜单”功能

– 2020.9.24 v5.0.1 Release
1. 对Big Sur Developer Beta 8 进行细节Адаптирован ，经测试可以直接全新安装 -->

### Обновите Clover

– 2020.4.7 v3.4 Release

1. Модифицировать USBports связанный，удалить USBpower
2. Обновите все драйверы（Lilu, AppleALC, Nvmefix и т.д.）

## О вознаграждениях

Если вы признаете мою работу, пожалуйста, поддержите мои последующие обновления с помощью вознаграждений. Так как бесплатно поддерживать Heiguo очень утомительно. С каждым обновлением системы требуется много времени для её оптимизации.
Для входа в группу требуется вознаграждение через WeChat или Alipay, что очень добросовестно по сравнению с tb. Не забудьте отправить сообщение на свой номер QQ за вознаграждение, а затем, когда вы подадите заявку на вступление в группу, дайте мне знать.
Если изображения на GitHub зависают, вы можете перезагрузмит VPN и обновить страницу или выполнить прямой поиск в группе QQ, чтобы найти владельца группы в списке участников.

| Alipay                 | WeChat                 |
| ---------------------- | ---------------------- |
| ![Alipay](Alipay1.jpg) | ![Wechat](Wechat1.jpg) |

| Группа в QQ           |
| --------------------- |
| ![963407871](QQ1.jpg) |

### В настоящее время недоступно

-  Камера (В Pro версии может распознавать её, но показывает чёрный экран, доступно в Magicbook 2019)
-  Отпечаток пальца
-  NVIDIA GeForce MX250 (Лао Хуан из NVIDIA порвал контракт с Apple и, возможно, ему будет трудно управлять автомобилем при жизни (юмор?)

### !!! В настоящее время жёсткий диск Samsung PM981 может использовать только Clover

В настоящее время жёсткий диск Samsung PM981 может использовать только Clover для загрузки* (поскольку патч не поддерживает OpenCore)*, и в то же время он может использовать только метод восстановления для установки Black Apple. Чтобы решить проблему с установкой метода восстановления Samsung PM981 в Gun you, Clover 2020.3.25 v3.2 был специально обновлен. Подробное содержание обновления приведено ниже содержания обновления OpenCore. Тем не менее, PM981 иногда выходит из строя без причины, перезагружается, не удается напрямую обновить систему и возникают другие странные проблемы (для получения подробной информации, пожалуйста, обратитесь к Baidu: Black Apple PM981), поэтому, если вы хотите стабильно использовать Black Apple, рекомендуется заменить жёсткий диск PM981 для спокойной работы. Если вы используете 2019 Pro, вы можете установить HDD SATA.

### Хочу подлагодарить

1. Список долгосрочного обслуживания Black Apple на GitHub:

   -  [Zero-zer0/Matebook_D_2018](https://github.com/Zero-zer0/Matebook_D_2018_Hackintosh_OpenCore)
   -  [hjmmc/Honor-Magicbook](https://github.com/hjmmc/Honor-Magicbook)
   -  [Zero-zer0/Matebook_13_14_2020](https://github.com/Zero-zer0/Matebook_13_14_2020_Hackintosh_OpenCore)
   -  [frezs/MateBook14-Hackintosh](https://github.com/frezs/MateBook14-Hackintosh)
   -  [4323770/Hackintosh-For-Matebook-X](https://github.com/4323770/Hackintosh-For-Matebook-X)

2. [Black Fruit Soldier] [Официальная версия macOS Catalina 10.15.3 19D76 с оригинальным изображением Clover 5103](https://blog.daliansky.net/macOS-Catalina-10.15.3-19D76-Release-version-with-Clover-5103-original-image-Double-EFI-Version.html)
3. [Black Fruit Soldier] Инструмент для взлома (ранее Intel FB-Patcher) Учебное пособие и поза для вставки
4. [Vision Forum](http://www.pcbeta.com) — сообщество гиков Microsoft
