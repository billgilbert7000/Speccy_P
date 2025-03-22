	SPECCY P v1.0.0
Эмулятор ZX Spectrum
 OTG USB клавиатура и USB мышь + PS/2 клавиатура
 I2S звук, PSRAM 8Mb, HARD/Soft Turbosound 
 режимы  NORMAL / TURBO / FAST
 и так далее
![photo_2024-10-22_19-43-45](https://github.com/user-attachments/assets/a3ccf7db-5753-448e-acc6-ef78bebc59d1)
 
SPECCY P ТЕСТОВАЯ ВЕРСИЯ!
Эмулятор ZX Spectrum v1.0.0 (SDK 2.1.1)
Прошивки для платы ПЕРВОГО Мурмулятора
 -Pico 2 RP2350A  m1p2
 -Pico   RP2040   m1p1
 OTG USB клавиатура и USB мышь + PS/2 клавиатура
 PSRAM по версии первого мурмуятора (GPIO 18,19,20,21)
 планируется поддержка "бутербродной" PSRAM для pico2
 (работает и без неё только Spectrum 128),
 HARD/Soft Turbosound  I2S звук
 #SpeccyP #Scorpion #Pentagon #cash #pico2 #rp2350 #rp2040
 //=============================================================================
  2025/02/11 v1.0.0
- SDK 2.1.1
  
[F12] настройки
[F11] файловое меню / [SPACE] быстрый запуск TDS и SCL файлов
[F1] Help
!!! [Scroll Lock] переход в режим прошивки !!!
-  Дизассемблер клавиша [END] 
-- Перекючение на дамп памяти [ENTER]
-- Выход [ESC]
------------------------------
ZX Spectrum  128 
Pentagon     512 
Pentagon 512CASH 
Pentagon    1024 
Scorpion     256 
ScorpionGMX 2048 
Navigator    256 
MurmoZavr    8Mb
-------------------------------
- Aвтостарт при включении или hard reset
  -- настраивается в меню настроек [F12] пункт [AutoRUN]
  -- файлов TRD , SCL с диска A [File TR-DOS]
     если образ был подключен в файловом меню 
     и была записана текущая конфигурация [Save config]
  -- SLOTa 0  "быстрой загрузки" [QuickSave Slot 0]
  
   То есть после включения загружается полностью рабочая машина 
     со всеми файлами и подключенными образами дисков и так далее,
     которая была сохранена по кнопке [F5] или из "быстрой загрузки" в slot 0
   -- возможность отключения автостарта [OFF]
-------------------------------- 
-прошивки rp2350a m1p2
--- VGA 60Hz  
--- HDMI 60Hz с делителем 1.5
--- TFT ili9341 / переворот в настроках 
--- TFT_st7789 / переворот в настроках пока не работает
-прошивки rp2040 m1p1
--- VGA 60Hz  
--- HDMI 60Hz с делителем 1.5
--- TFT ili9341 / переворот в настроках 
--- TFT_st7789 / переворот в настроках пока не работает
//=============================================================================
 2025/01/28 v0.16.7
- Работа над ошибками 
-- Исправленно чтение из порта 0xFF (порт атрибутов)
-  Дизассемблер клавиша [END] 
-- Перекючение на дамп памяти [ENTER]
-- Выход [ESC]
[F12] настройки
[F11] файловое меню / [SPACE] быстрый запуск TDS и SCL файлов
[F1] Help
-прошивки
--- VGA 60Hz  
--- HDMI 90Hz с делителем 1.0
--- HDMI 60Hz с делителем 1.5
--- TFT ili9341 / переворот в настроках 
--- TFT_st7789 / переворот в настроках пока не работает
-тестовые прошивки
--- VGA 60Hz RP20040 400МГц 
      speccyP_0.16.7_CPU400Mz_VGA_60Hz 
--- VGA 60Hz PSRAM на пониженной частоте 
      speccyP_0.16.7_lowPSRAM_VGA_60Hz
!!! [Scroll Lock] переход в режим прошивки !!!
//=============================================================================
2025/01/23 v0.16.6
-  Дизассемблер клавиша [END] 
-- Перекючение на дамп памяти [ENTER]
-- Выход [ESC]
[F12] настройки
[F11] файловое меню / [SPACE] быстрый запуск TDS и SCL файлов
[F1] Help
--- прошивка VGA 60Hz  
--- прошивка  HDMI 90Hz с делителем 1.0
--- прошивка HDMI 60Hz с делителем 1.5
--- прошивка TFT ili9341 / переворот в настроках 
--- прошивка TFT_st7789 / переворот в настроках пока не работает
- Работа над ошибками 
!!! [Scroll Lock] переход в режим прошивки !!!
//=============================================================================
2024/12/25 v0.16.3 
- Работа над ошибками 
- Добавлена конфигурация Pentagon 512 с CASH 32Kb [Pentagon 512CASH]
-- переключение по портам IN (0xFB) - включить кэш, IN (0x7B) - выключить
-- вход по Magic/NMI клавиша [F9]
- Настройка переворота TFT
- Увеличена громкость бипера в режиме i2s 
--- прошивка VGA 60Hz  
--- прошивка HDMI 60Hz с делителем 1.5
--- прошивка TFT ili9341 
//=============================================================================
2024/12/13 v0.15.8 TEST!
- Работа над ошибками 
-- исправлена маска AY в режиме soft AY/TS
- тест запуска без обнуления памяти 128kB и выше при reset (экспериментально)
- возможность изменение палитры в меню настроек и по [F6] (экспериментально)
-[PrinttScreen] входа в режим обновления прошивки , анологичен нажатию кнопки BOOT !
---  378 MHz
--- прошивка VGA 60Hz  
--- прошивка  HDMI 90Hz с делителем 1.0
--- прошивка HDMI 60Hz с делителем 1.5
--- прошивка TFT ili9341 
--- прошивка TFT_st7789 
---  315 MHz
--- прошивка HDMI 75Hz с делителем 1.0
 #SpeccyP #Scorpion 
 //=============================================================================
2024/12/05 v0.15.7
- Работа над ошибками
-- Исправленно стерео в режиме soft AY//TS (лево<>право) ABC
-- Корректное выключение-включение звука в режиме Hard AY/TS 
   при входе в меню и по кнопке PAUSE
-- Добавлен выход из файлового меню по клавише [ESC]   
-- Раздельное сохранение уровня громкости для SoftAY/TS и i2s звука
-- регулировка громкости [F7] [F8]
-- по умолчанию включен звук SoftTS 

-  Scorpion ZS256 
-- вход в Теневой Сервис Монитор  [F9] NMI/Magic
-- отключение ПЗУ и включение ОЗУ bank 0, по биту D0 порта #1FFD

- Пунк выключения с сохранением текущей конфигурации [Power OFF] ;)
- Вход в режим обновления прошивки [Update mode], анологичен нажатию кнопки BOOT 
- Работа с геймпадом XBox в режиме кемстон джойстика / только кнопки и крестовина 
- Работа с китайским беспроводным геймпадом в режиме кемпстон джойстика
--- прошивка VGA 60Hz  
--- прошивка HDMI 90Hz с делителем 1.0
--- прошивка HDMI 60Hz с делителем 1.5
--- прошивка TFT ili9341 
--- прошивка TFT_st7789 

#SpeccyP #Scorpion 
//=============================================================================
2024/12/04 v0.15.6
- Работа над ошибками
- режим Scorpion ZS256 
-- починен пункт меню входа в TR-DOS / теперь не зависает
-- вход в Теневой Сервис Монитор  [F9] NMI/Magic
-- отключение ПЗУ и включение ОЗУ bank 0, по биту D0 порта #1FFD
-- корректная работа через RST8
- исправленны некоторые ошибки эмулятора процессора Z80  
- Добавлен пункт Spectrum 48
- шрифт 6x7 интерфейса
- по умолчанию включен звук SoftTS 
  при переключении на I2S рекомендуется 
  отрегулировать громкость [F7] [F8]
- по Soft reset  сброс TAP файлов на начало 
- F4 вызов помощи по клавишам ZX Spectrum ( by Technocat)
- Исправена работа с файлами образов с атрибутом ReadOnly и Archive
- Исправлена работа с укороченными TRD файлами нестандартной длины / ReadOnly
- Исправлена работа с SCL файлами / ReadOnly
- Добавлен пунк выключения с сохранением текущей конфигурации
- Добавлен пунк входа в режим обновления прошивки , анологичен нажатию кнопки BOOT 
- Работа с геймпадом XBox в режиме кемстон джойстика / только кнопки и крестовина 
- Работа с китайским беспроводным геймпадом в режиме кемпстон джойстика
--- прошивка VGA 60Hz  
--- прошивка HDMI 90Hz с делителем 1.0
--- прошивка HDMI 60Hz с делителем 1.5
--- прошивка TFT ili9341 
--- прошивка TFT_st7789 не тестировалась

#SpeccyP #Scorpion #XBox
//=============================================================================
2024/11/11 v0.15.4s
- Работа над ошибками
- Добавлен пункт Spectrum 48

- по Soft reset  сброса TAP файлов на начало 
- F4 вызов помощи по клавишам ZX Spectrum ( by Technocat)
- Исправена работа с файлами образов с атрибутом ReadOnly и Archive
- Исправлена работа с укороченными TRD файлами нестандартной длины / ReadOnly
- Исправлена работа с SCL файлами / ReadOnly
- Исправлен баг с отображением директорий как файлов
- Добавлен пунк выключения с сохранением текущей конфигурации
- Добавлен пунк входа в режим обновления прошивки , анологичен нажатию кнопки BOOT 
- Работа с геймпадом XBox в режиме кемстон джойстика
- Работа с китайским беспроводным геймпадом в режиме кемпстон джойстика
//=============================================================================
2024/07/24 v0.14.6
Добавленна одновременная работа USB клавиатуры/мыши через USB OTG 
и PS/2 клавиатуры

- Для работы OTG на черной пико необходимо замыкать трёхногий диод!

- Работа над ошибками
-- починен NES Joy
-- убраны тормоза при INT 50Hz в режиме TURBO 
-- и остальное по мелочи

- Запуск TRD и SCL файлов из файлового меню БЕЗ выбора диска
  -- клавиша [SPACE]  или кнопка NES джойстика  [B] 
  -- происходит сброс с АВТОМАТИЧЕСКОЙ загрузкой выбранного образа с диска A:
  -- клавиша [ENTER]  или кнопка NES джойстика  [A] попрежнему 
     позволяют подключать образы к любому из 4 дисководов 

-клавиатура 
F1 Help
F2 быстрое сохранение
F3 загрузка сохранений
F5 Быстрое сохранение в slot 0 + сохранение файла конфигурации
F9 кнопка вызова прерывания NMI (опционально)
F10 Normal/Turbo/Fast
  NORMAL 3.5MHz Int 50Hz 
  TURBO  Int 50Hz 
  FAST   Int 100Hz 
F11/WIN/Ins  файловое меню / выход из файлового меню F11/WIN/Ins
F12/Home меню настроек 
F7 Volume down 
F8 Volume up
ESC  выход из менюшек и так далее.

-NES джойстик
-- START+стрелка вниз  - вход в файловый браузер/ выход повторное нажатие [START+стрелка вниз]  или [B] на джое
                       - [A] выбор файла
                       - [START] Выход
                       - [B] Запуск образов TDA, SCL  
-- START+стрелка вверх  - вход в меню настроек / [A] джойстика - выбор / выход из него кнопкой [B] джойстика
-- START+стрелка влево -  вход в меню SAVE / [A] джойстика - выбор / выход  [B] джойстика
-- START+стрелка вправо - вход в меню LOAD / [A] джойстика - выбор / выход [B] джойстика
-- выход из файлового меню по клавише [START] 

- Aвтостарт при включении или hard reset
  -- настраивается в меню настроек [F12] пункт [AutoRUN]
  -- файлов TRD , SCL с диска A [File TR-DOS]
     если образ был подключен в файловом меню 
     и была записана текущая конфигурация [Save config]
  -- SLOTa 0  "быстрой загрузки" [QuickSave Slot 0]
  
   То есть после включения загружается полностью рабочая машина 
     со всеми файлами и подключенными образами дисков и так далее,
     которая была сохранена по кнопке [F5] или из "быстрой загрузки" в slot 0
   -- возможность отключения автостарта [OFF]

--- прошивка VGA 60Hz  
--- прошивка HDMI 90Hz с делителем 1.0
--- прошивка HDMI 60Hz с делителем 1.5
--- прошивка TFT ili9341 не тестировалась
--- прошивка TFT_st7789 не тестировалась

 //=============================================================================
2024/07/16 тестовая версия
Добавленна одновременная работа USB клавиатуры/мыши через USB OTG 
и PS/2 клавиатуры
- Для работы OTG на черной пико необходимо замыкать трёхногий диод!
-- Загрузка и работа демо Elisium State (но есть одно НО связанное с видедрайвером)
--- прошивка VGA 60Hz  
--- прошивка HDMI 90Hz с делителем 1.0
--- прошивка HDMI 75Hz с делителем 1.5
//=============================================================================
2024/06/20
- Исправление громкости 1го чипа AY
- Исправленны каналы SoftAY/TS  & i2s  AY/TS
("перепаял лево-право")
-- Left   > Chanel A
-- Right  > Chanel C
-- Middle > Chanel B
//=============================================================================
v0.14.3 
2024/06/18 
- Добавленна поддержка i2s звука на TDA и PCM5102
-- на TDA не тестировал, на PCM5102 уровень звука вроде нормально, но нужно проверять
-- Изменен алгоритм регулировки громкости клавишами [F7] и [F8] 
-- в Soft AY/TS от 0 до 32
-- в I2S AY/TS от 0 до 255
-- настройки текущей громкости можно сохранить в файле конфигурации
-- beeper по i2s работает но всё же не совсеи правильно  
-- Режимы звука переключаются с сохранением конфигурации и перезагрузкой!
-- Опртимизирован алгоритм эмуляции AY в Soft AY/TS и I2S AY/TS
-- прошивка HDMI 90Hz с делителем 1.0
-- прошивка HDMI 75Hz с делителем 1.5
//=============================================================================
2024/06/16
- Добавленна поддержка i2s звука на TDA и PCM5102
-- на TDA не тестировал, на PCM5102 уровень звука вроде нормально, но нужно проверять
-- добавлена регулировка громкости клавишами [F7] и [F8] в Soft AY/TS и I2S AY/TS 
-- настройки текущей громкости можно сохранить в файле конфигурации
-- beeper по i2s работает но всё же не совсеи праввильно  
-- Режимы звука переключаются на лету, на сколько это возможно.
   для сохранения режима вывода звука необходимо сохранить конфигурацию.
   -- Режим Hard TurboSound требует сохранения и перезагрузки!

- Добавлена возможность включения режимов 
  по клавише [F10] циклически или из меню настроек [Speed Mode]:
  NORMAL 3.5MHz Int 50Hz 
  TURBO x1.5 Int 50Hz (Пока это максимальная скорость эмулятора Z80)
  FAST  x2.0 Int 100Hz 
-- Настройки скорости не сохраняются в файле конфигурации!
- Pico работает теперь на частоте 378MHz из-за режима TURBO
 и соответственно теперь HDMI 60Hz

- Незначительная оптимизация
- Работа над ошибками

- Запуск TRD и SCL файлов из файлового меню БЕЗ выбора диска
  -- клавиша [SPACE]  или кнопка NES джойстика  [B] 
  -- происходит сброс с АВТОМАТИЧЕСКОЙ загрузкой выбранного образа с диска A:
  -- клавиша [ENTER]  или кнопка NES джойстика  [A] попрежнему 
     позволяют подключать образы к любому из 4 дисководов 

-- START+стрелка вниз  - вход в файловый браузер/ выход повторное нажатие [START+стрелка вниз]  или [B] на джое
                       - [A] выбор файла
                       - [START] Выход
                       - [B] Запуск образов TDA, SCL  
-- START+стрелка вверх  - вход в меню настроек / [A] джойстика - выбор / выход из него кнопкой [B] джойстика
-- START+стрелка влево -  вход в меню SAVE / [A] джойстика - выбор / выход  [B] джойстика
-- START+стрелка вправо - вход в меню LOAD / [A] джойстика - выбор / выход [B] джойстика
-- выход из файлового меню по клавише [START]   
-- (Пока такое управление , рассмотрю другие варианты)

-- Как обычно поддержка PSRAM для расширения памяти ZX Spectrum > 128Кб.

- !!! НОВЫЙ файл конфигурации zxcon142.dat в корне SD карты !!!
-- старый zxconfig.dat или zxconа14.dat  можно удалить или оставить для старых версий прошивки 

- Aвтостарт при включении или hard reset
  -- настраивается в меню настроек [F12] пункт [AutoRUN]
  -- файлов TRD , SCL с диска A [File TR-DOS]
     если образ был подключен в файловом меню 
     и была записана текущая конфигурация [Save config]
  -- SLOTa 0  "быстрой загрузки" [QuickSave Slot 0]
  -- если будет востребованна данная функция, 
     то возможно будет сделано сохранение и всей расширенной памяти.
     пока сохраняется только 128Кб с сохранением всех подключенных дисков TR-DOS
     и всех других настроек. 
     То есть после включения загружается полностью рабочая машина 
     со всеми файлами и подключенными образами дисков и так далее,
     которая была сохранена по кнопке [F5] или из "быстрой загрузки" в slot 0
   -- возможность отключения автостарта [OFF]
//============================================================================================================
2024/05/07
ТЕСТОВАЯ ВЕРСИЯ  +i2s Sound  +Turbo CPU Z80
- Добавленна поддержка i2s звука на TDA и PCM5102
-- на TDA не тестировал, на PCM5102 уровень звука вроде нормально, но нужно проверять
-- добавлена регулировка громкости клавишами [F7] и [F8] в Soft AY/TS и I2S AY/TS 
-- настройки текущей громкости можно сохранить в файле конфигурации
-- beeper работает , но громкость не настроенна
-- Режимы звука переключаются на лету, на сколько это возможно.
   для сохранения режима вывода звука необходимо сохранить конфигурацию.
   -- Режим Hard TurboSound требует сохранения и перезагрузки!

- Незначительная оптимизация
- Работа над ошибками
- 
- Запуск TRD и SCL файлов из файлового меню БЕЗ выбора диска
  -- клавиша [SPACE]  или кнопка NES джойстика  [B] (Переделал на [B] так как не у всех есть [С])
  -- происходит сброс с АВТОМАТИЧЕСКОЙ загрузкой выбранного образа с диска A:
  -- клавиша [ENTER]  или кнопка NES джойстика  [A] попрежнему 
     позволяют подключать образы к любому из 4 дисководов 

-- START+стрелка вниз  - вход в файловый браузер/ выход повторное нажатие [START+стрелка вниз]  или [B] на джое
                       - [A] выбор файла
                       - [START] Выход
                       - [B] Запуск образов TDA, SCL  
-- START+стрелка вверх  - вход в меню настроек / [A] джойстика - выбор / выход из него кнопкой [B] джойстика
-- START+стрелка влево -  вход в меню SAVE / [A] джойстика - выбор / выход  [B] джойстика
-- START+стрелка вправо - вход в меню LOAD / [A] джойстика - выбор / выход [B] джойстика
-- выход из файлового меню по клавише [START]   
-- (Пока такое управление , рассмотрю другие варианты)

-- Как обычно поддержка PSRAM для расширения памяти ZX Spectrum > 128Кб.

- !!! НОВЫЙ файл конфигурации zxcon141.dat в корне SD карты !!!
-- старый zxconfig.dat или zxconа14.dat  можно удалить или оставить для старых версий прошивки 

//=============================================================================
2024/05/03
ТЕСТОВАЯ ВЕРСИЯ  ТОЛЬКО VGA 60Hz и HDMI 75Hz
- Переписан модуль TR-DOS  
-- Запускаются и работают демки типа UNREAL 
   и другие проблемные в плане фоновой загрузки с диска.
-- Работает стандартное форматирование из под TR-DOS образов *.TRD
--- образы форматируются как двухсторонний диск 80 дорожек 

- Запуск TRD и SCL файлов из файлового меню БЕЗ выбора диска
  -- клавиша [SPACE]  или кнопка NES джойстика  [B] (Переделал на [B] так как не у всех есть [С])
  -- происходит сброс с АВТОМАТИЧЕСКОЙ загрузкой выбранного образа с диска A:
  -- клавиша [ENTER]  или кнопка NES джойстика  [A] попрежнему 
     позволяют подключать образы к любому из 4 дисководов 

-- START+стрелка вниз  - вход в файловый браузер/ выход повторное нажатие [START+стрелка вниз]  или [B] на джое
                       - [A] выбор файла
                       - [START] Выход
                       - [B] Запуск образов TDA, SCL  
-- START+стрелка вверх  - вход в меню настроек / [A] джойстика - выбор / выход из него кнопкой [B] джойстика
-- START+стрелка влево -  вход в меню SAVE / [A] джойстика - выбор / выход  [B] джойстика
-- START+стрелка вправо - вход в меню LOAD / [A] джойстика - выбор / выход [B] джойстика
-- выход из файлового меню по клавише [START]   
-- (Пока такое управление , рассмотрю другие варианты)

-- Как обычно поддержка PSRAM для расширения памяти ZX Spectrum > 128Кб.

- !!! НОВЫЙ файл конфигурации zxconf14.dat в корне SD карты !!!
-- старый zxconfig.dat можно удалить или оставить для старых версий прошивки 

- Работа над ошибками
 //=============================================================================
2024/04/10
- SoftAY
//=============================================================================
2024/04/03
- Работа над ошибками
Добавлена персональная прошивка для ультимейта с клоком AY на 21 пине,
соответственно отключенна поддержка расширеной памяти >128Кб на PSRAM
speccyP_0.13.8_AY21_NOPSRAM_VGA.uf2
!!! При первом запуске прошивки во избежании глюков !!!
!!! необходимо удалить старый файл конфигурации     !!!
!!! zxconfig.dat в корне SD карты                   !!!
-- Кое какие испаравления , все равно это никто не читает
-- добавлены новые глюки
//=============================================================================
2024/04/03
- Aвтостарт при включении или hard reset
  -- настраивается в меню настроек [F12] пункт [AutoRUN]
  -- файлов TRD , SCL с диска A [File TR-DOS]
     если образ был подключен в файловом меню 
     и была записана текущая конфигурация [Save config]
  -- SLOTa 0  "быстрой загрузки" [QuickSave Slot 0]
  -- если будет востребованна данная функция, 
     то возможно будет сделано сохранение и всей расширенной памяти.
     пока сохраняется только 128Кб с сохранением всех подключенных дисков TR-DOS
     и всех других настроек. 
     То есть после включения загружается полностью рабочая машина 
     со всеми файлами и подключенными образами дисков и так далее,
     которая была сохранена по кнопке [F5] или из "быстрой загрузки" в slot 0
   -- возможность отключения автостарта [OFF]

- Запуск TRD и SCL файлов из файлового меню БЕЗ выбора диска
  -- клавиша [SPACE]  или кнопка NES джойстика  [C]
  -- происходит сброс с АВТОМАТИЧЕСКОЙ загрузкой выбранного образа с диска A:
  -- кто-то спрашивал про кнопку RUN ;) теперь эта кнопка в принципе не нужна
  -- клавиша [ENTER]  или кнопка NES джойстика  [A] попрежнему 
     позволяют подключать образы к любому из 4 дисководов 

- Добавлен очередной экспериментальный пункт меню 
  --Bass boost (фильтр высоких частот + усиление НЧ) для soft AY
  --Звук на попробовать, используется алгоритм простого фильтра ;)

- Небольшие  исправления в файловом меню

!!! При первом запуске прошивки во избежании глюков !!!
!!! необходимо удалить старый файл конфигурации     !!!
!!! zxconfig.dat в корне SD карты                   !!!

P.S. игра из файла "GRYZOR (EMELYANOV PAVEL).TAP теперь запускается
     
-- START+стрелка вниз  - вход в файловый браузер/ выход повторное нажатие [START+стрелка вниз]  или [B] на джое
                       - [A] выбор файла
                       - [B] Выход
                       - [C] Запуск образов TDA, SCL  (у меня на джое эта кнопка иногда почемуто срабатывает как [A])
-- START+стрелка вверх  - вход в меню настроек / [A] джойстика - выбор / выход из него кнопкой [B] джойстика
-- START+стрелка влево -  вход в меню SAVE / [A] джойстика - выбор / выход  [B] джойстика
-- START+стрелка вправо - вход в меню LOAD / [A] джойстика - выбор / выход [B] джойстика
-- (Пока такое управление , рассмотрю другие варианты)
-клавиатура 
F2 быстрое сохранение
F3 загрузка сохранений
F5 Быстрое сохранение в slot 0 + сохранение файла конфигурации
F9 кнопка вызова прерывания NMI (опционально)
F11 файловое меню
F12 меню настроек
ESC  выход из менюшек и так далее.
//==================================================================================
2024/03/28
- Работа над ошибками
- Небольшие изменения в softAY и Soft TS
- Исправленна работа с SD картой в режиме tr-dos (SPI)
- Добавленно дополнительное отображение длинных имен файлов 
- Добавлены новые глюки
P.S. Пунк меню настроек [Memory] это не полная поддержка названной там машины!
     А только расширение памяти больше 128Кб по данному стандарту!
     Pentagon-512: #7FFD, биты 0,1,2,6, 7 
     Pentagon-1024: #7FFD, биты0,1,2 5,6, 7; (5-й бит НЕ выполняет блокировку в 48-й режим)
     Profi-1024: #DFFD, биты 0, 1, 2; #7FFD: биты 0,1,2;
     Scorpion ZS 256: #1FFD бит 4; #7FFD: биты 0,1,2;
     Scorpion GMX 2048: #DFFD, биты 0, 1, 2; #1FFD бит 4; #7FFD: биты 0,1,2;
     Unreal 4096: #DFFD, биты 0, 1, 2; #7FFD: биты 0,1,2,6, 7; HE СУЩЕСТВУЮЩИЙ В ПРИРОДЕ СТАНДАРТ
//==================================================================================
2024/03/20
- Исправлен звук  в режимах Soft AY и Soft TS (огибающие)
-- подкрученна тональность
-- Добавлен пункт выбора таблиц амплитуд AY [ AY Table ]
    (пока в тестовом режиме, но сохраняется в файл конфигурации)

- Добавлена эмуляция существовавщего в ОДНОМ экземпляре Speccy 
"Navigator 256Kb" расширение памяти по 7 биту порта 0x7ffd   
в нем работает кнопка NMI [F9]  и есть диззасемблер ( ЭТО НЕ STS!)
 с возможностью редактирования памяти , пресловутый POKE ;)
 описание утеряно так что всё методом тыка, если интересно.
 -- при выборе [Navigator 256] необходимо сохранить конфмгурацию и перезагрузить.
 (в дальнейшем возможно исправлю)
 -- Navigator 256 добавил из-за ностальгии и не закрытого гештальта ;)
    мой speccy для которого и был написан данный монитор и т.д.

 -- возможно еще что то добавил, но уже не помню.   


в архиве 4 файла прошивки:
speccyP_0.13.4_HDMI_75Hz.uf2 
speccyP_0.13.4_TFT_ili9341.uf2
speccyP_0.13.4_TFT_st7789.uf2   
speccyP_0.13.4_VGA_60Hz.uf2
//==================================================================================
2024/03/18
- Поддержка дисплеев на контроллерах   ili9341 и st7789  (320x240)
-- Исправленна инициализация дисплея на контроллере st7789.
   NB: Всё таки коианды инициализации у эти дисплеев отличаются, 
   если делать полную инициализацию , а не запускать по умолчанию.
   NB: Теперь дисплей на st7789 работает без управления сигналом CS.
--- ili9341 работает на 100Гц [если нужно могу изменить Frame Ratio 61...119 Hz ]
--- st7789 работает на 50Гц   [если нужно могу изменить Frame Ratio 39...119 Hz]
-- Подключение TFT дисплея :
    TFT_CLK_PIN (13)
    TFT_DATA_PIN (12)
    TFT_RST_PIN (8)
    TFT_DC_PIN (10)
    TFT_CS_PIN (6)   // Пин CS !ЛЮБОГО! дисплея можно к pico не подключать, а притянуть к GND 
                     // Оставил 0 на GPIO 6 для совместимости   
    TFT_LED_PIN  (9)  // Подсветка  ШИМ 100Гц LED подсветки дисплея по дефолту 70% яркости

- Изменено управление NES джойстиком
-- START+стрелка вниз  - вход в файловый браузер/ выход повторное нажатие [START+стрелка вниз]  или [B] на джое
-- START+стрелка вверх  - вход в меню настроек / [A] джойстика - выбор / выход из него кнопкой [B] джойстика
-- START+стрелка влево -  вход в меню SAVE / [A] джойстика - выбор / выход  [B] джойстика
-- START+стрелка вправо - вход в меню LOAD / [A] джойстика - выбор / выход [B] джойстика
-- (Пока такое управление , рассмотрю другие варианты)

//==================================================================================
2024/03/14
- Управление NES джойстиком
-- MODE - вход в файловый браузер/ выход повторное нажатие [MODE] на джое
-- MODE+стрелка вверх  - вход в меню настроек / [A] джойстика - выбор / выход из него кнопкой [B] джойстика
-- MODE+стрелка влево -  вход в меню SAVE / [A] джойстика - выбор / выход  [B] джойстика
-- MODE+стрелка вправо - вход в меню LOAD / [A] джойстика - выбор / выход [B] джойстика
-- (Пока такое управление , рассмотрю другие варианты)

- Кнопка [PAUSE] клавиатуры - старт/стоп эмулятора
- Кнопка [START] джойстика  - старт/стоп эмулятора

- Убран режим выбора TFT дисплея , теперь для каждого дисплея своя прошивка
  (Пока так, думаю как лучше объединить)
-- Поддерживаются дисплеи на контроллерах   ili9341 и st7789  (320x240)
-- Подключение TFT дисплея
    TFT_CLK_PIN (13)
    TFT_DATA_PIN (12)
    TFT_RST_PIN (8)
    TFT_DC_PIN (10)
    TFT_CS_PIN (6)   // Пин CS дисплея на ili9341  можно к pico не подключать, а притянуть к GND (тестовый вариант)
    TFT_LED_PIN  (9)  // Подсветка
---
в архиве 5 файлов прошивки:

speccyP_0.13.2_HDMI_75Hz.uf2 
speccyP_0.13.2_TFT_ili9341.uf2
speccyP_0.13.2_TFT_st7789.uf2    дисплей без инверсии тест
speccyP_0.13.2_TFT_st7789inv.uf2 дисплей с инверсией тест
speccyP_0.13.2_VGA_60Hz.uf2

//==================================================================================
2024/03/12
- Скорректированна скорость управления в меню настроек и файловом меню 
- Добавлена возможность входа в файловое меню по кнопке NES джойстика [MODE] 
- Незначительные исправления в Hard TurboSound 
- Исправленны некоторые баги и добавленны новые
//==================================================================================
2024/03/09
-- Только для TFT дисплеев ili9341 и st7789
--Добавлена возможность использование дисплеев на этих контроллерах

--Добавлен пункт регулировки яркости TFT дисплеев в меню настроек 5% ... 100%
  ШИМ 100Гц LED подсветки дисплея по дефолту 70% яркости
====================================================================================
2024/03/07
- Исправленно подключение TFT дисплея
    TFT_CLK_PIN (13)
    TFT_DATA_PIN (12)
    TFT_RST_PIN (8)
    TFT_DC_PIN (10)
    TFT_CS_PIN (6) 
    TFT_LED_PIN  (9) 
    ШИМ 100Гц LED подсветки дисплея пока без регулировки 
    установлен на 70% яркости
===================================================================================
2024/03/06
-Корректное определение обЪема PSRAM памяти

- Добавлен пункт изменения скорости SPI SD карты [SPI baudrate]
  25Mbd, 12Mbd, 10Mbd, 8Mbd
  SPI baudrate автоматически устанавливается ближайщий возможный для данного железа
  по дефолту стартует на 12 Mbd  
  настройки SPI baudrate сохраняются в файл конфигурации

- в наличии четыре  прошивки VGA 60Hz , HDMI 60Hz/75Hz и TFT на ili9341
 (75Hz пока убрал)

-nes джойстик работает (убрал некоректное сообщение при старте)

-добавлен шим на GPIO 9 подсветки TFT пока стоит на 50% (у себя не проверял)
 драйвер TFT пока сырой могут возникать очень неожиданные эффекты на дисплее,
 типа горизонтального скролла (разбираюсь)

- уменьшил задержку при работе с USВ клавиатурой через адаптер USB_to_i2c 
  (usb клавиатура через адаптер работает слишком быстро, 
  разбираюсь как устранить последствия этого)

- по подключению USB_to_i2c
с пики USB_to_i2c  gpio0 gpio1 на gpio0 и gpio1  мурмулятора. 
 i2c заведен на разъём ps/2... 
 т.е. прошивка сама определяет чего туда подключено i2c или ps/2 клавиатура. 
//================================================================================


1. Поддержка PSRAM для расширения памяти ZX Spectrum.

По стандарту Пентагон 512,Пентагон 1024, 
Профи 1024, Scorpion ZS256, Scorpion 2048 
и несуществующий стандарт на 4096кБ.
1.1 если PSRAM отсутствует (определение наличия PSRAMпри запуске)
 то доступна только одна конфигурация памяти Spectrum 128. (Что логично)

1.3  Pentagon-512: #7FFD, биты 0,1,2,6, 7 (5-й бит выполняет стандартную блокировку всех портов расширения памяти, превращая компьютер в 48-й);

1.4 Pentagon-1024: #7FFD, биты0,1,2 5,6, 7; (5-й бит НЕ выполняет блокировку в 48-й режим)

1.5 Profi-1024: #DFFD, биты 0, 1, 2; #7FFD: биты 0,1,2;

1.6 Scorpion ZS 256: #1FFD бит 4; 
#7FFD: биты 0,1,2;

1.7 Scorpion GMX 2048: #DFFD, биты 0, 1, 2
#1FFD бит 4; #7FFD: биты 0,1,2;

1.8 Unreal 4096: #DFFD, биты 0, 1, 2;
#7FFD: биты 0,1,2,6, 7; 

 
2. Поддержка USB мыши и клавиатуры при использовании адаптера на второй пико usb to i2c.
(Подключается на GPIO 0 и GPIO1)
Определяется автоматически что подключено к разъему PS/2.

3. Поддержка soft AY и soft Turbosound.

4. Поддержка реальных AY-3-8910, YAMAHA и т.д.
   Hard TurboSound через сдвиговые регистры по стандарту Мурмулятора.
   Clock AY на GPIO29.

5. Корректно работающий TR-DOS .

5.1 Запускается boot Enlight'96 и многое другое.

5.2 Поддерживается 4 виртуальных дисковода A, B, C, D.

5.3 Загрузка файлов SCL, только для дисковода А.
    При монтировании файлов SCL дополнительно в диск прописывается boot ,
    для простого запуска файлов на SCL . 
    Образы SCL монтируются в режиме Read Only,
    для защиты таких образов от порчи при попытке записи на них.
5.4 Для ностальгии добавлен звук перемещения головок флопика , 
    работает пока только в режиме softAY и softTurboSound. 
	Звук FFD можно отключить в меню настроек.
	
5.5 Команда FORMAT пока работает некорректно,
    форматирует образ TRD как односторонний (разбираюсь).
	
6. Интерфейс SPI sd карты, разгоняется до 24 MBd.
    Пункт изменения скорости SPI SD карты [SPI baudrate]
    25Mbd, 12Mbd, 10Mbd, 8Mbd
    SPI baudrate автоматически устанавливается ближайщий возможный для данного железа
    по дефолту стартует на 12 Mbd  
    настройки SPI baudrate сохраняются в файл конфигурации
   
7. Быстрое сохранение и загрузка состояния памяти Спектрума,
   посредством вызова соответствующих меню, по клавишам F2-save и F3-load.
   Всего доступно 25 слотов сохранения,
   с визуализацией того что находится в слоте.
   
8. Вызов помощи по клавише F1, чтобы было ;)
   Выход почти из всех меню без выбора по клавише ESC .
   
9. Все настройки вынесены в отдельное меню 
   по кнопкам F12 или HOME.
   
9.1 Текущие настройки можно сохранить на SD карту
    в файл конфигурации, который читается при загрузке.
	При проблемах его можно удалить. zxconfig.dat.
	
10. Вызов файлового менеджера 
    по кнопке F11 или WIN или INSERT.
	
10.1 поддерживается 5 вложений папок 
     и максимум 128 файлов в директории. 
	 (сделал столько для отладки, но так и оставил, мне хватает)
	 
10.2 Длина имени файла 16 символов вместе с расширением, 
     если больше то отображается в укороченном варианте.
	 
11. CNTRL+ALT+DEL сброс ZX Spectrum
    SHIFT+ALT+DEL перезагрузка микроконтроллера.
    Кнопка PAUSE работает как пауза :)

12. Мгновенная загрузка файлов TAP.
    Через перехват точек входа в ПЗУ Спектрума.
    Большинство файлов что есть у меня загружается и работает,
	есть только один момент некоторые игры
	предназначенные для 48к некорректно загружаются
	через меню 128 Спектрума.
	И даже запускается и работает файл badapple2.tap ,
	на нем и тестировал.
	
12.0 Загрузка через линейный вход ПОКА отключена.
     (Разбираюсь)
	
12.1 SAVE TAPE тоже пока не работает.

13. RP2040 "pico" работает на 315 МГц 
    
14. Есть пока ТРИ версии прошивки с поддержками VGA, HDMI и TFT ili9341 

	
14.1 Драйвер VGA/HDMI  и TFT от Алекс Екб, за что ему огромная благодарность.


14.2	Распиновка подключения экранов TFT ILI9341 / ST7789
	TFT_CS_PIN (6) 
	TFT_RST_PIN (8)
	TFT_DC_PIN (10)
	TFT_DATA_PIN (12)
	TFT_CLK_PIN (13)
	TFT_LED_PIN (9)

	 
15. Глюки будут гарантирую, но это не точно.

16. NES джойстик работает . 

P.S.  Использованы исходники от мурмулятора января 2023 года и различные доработки 
P.S.S я еще тот программист, хоть на Си хоть еще на чем .
     Единственно на чем я писал то это ассемблер Z80 
	 и это было четверть века назад. 
	 Так что конструктивная критика и советы приветствуются.
     Исходники кода будут в ближайшее время доступны на GitHub, «говнокод» присутствует.
     





2024.03.12
