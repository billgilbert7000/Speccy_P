SPECCY P 
Эмулятор ZX Spectrum v0.14.6
 OTG USB клавиатура и USB мышь + PS/2 клавиатура
 I2S звук, PSRAM, HARD/Soft Turbosound 
 режимы  NORMAL / TURBO / FAST
 и так далее
![photo_2024-10-22_19-43-45](https://github.com/user-attachments/assets/a3ccf7db-5753-448e-acc6-ef78bebc59d1)
 
  //=============================================================================
2024/07/24
Добавленна одновременная работа USB клавиатуры/мыши через USB OTG 
и PS/2 клавиатуры

- Для работы OTG на черной пико необходимо замыкать трёхногий диод!

- 

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

 SPECCY P 
The ZX Spectrum emulator v0.14.6
OTG USB keyboard and USB mouse + PS/2 keyboard
 I2S sound, PSRAM, HARD/Soft Turbosound 
 NORMAL/ TURBO/FAST modes
and so on
  //=============================================================================
2024/07/24
Added simultaneous operation of USB keyboard/mouse via USB OTG
and PS/2 keyboards

- For OTG to work on a black pico, a three-legged diode must be closed!

- 

- Work on mistakes
-- fixed NES Joy
-- brakes are removed at INT 50Hz in TURBO mode 
-- and the rest of the little things

- Launch TRD and SCL files from the file menu WITHOUT selecting a disk
  -- the [SPACE] key or the NES button of the joystick [B]
-- resets with AUTOMATIC loading of the selected image from disk A:
-- the [ENTER] key or the NES button of the joystick [A] continues 
     allows you to connect images to any of the 4 drives 

-keyboard 
F1 Help
F2 quick save
F3 loading saves
F5 Quick save to slot 0 + save configuration file
F9 NMI interrupt call button (optional)
F10 Normal/Turbo/Fast
NORMAL 3.5MHz Int 50Hz 
  TURBO  Int 50Hz 
  FAST   Int 100Hz 
F11/WIN/Ins file menu / exit file menu F11/WIN/Ins
F12/Home settings menu 
F7 Volume down 
F8 Volume up
ESC exit menus and so on.

-NES joystick
-- START+down arrow - log in to the file browser/ exit by pressing [START+down arrow] again  or [B] on joy
                       - [A] file selection
                       - [START] Exit
                       - [B] Launching TDA, SCL images  
-- START+up arrow - enter the settings menu / [A] joystick - select / exit it with the [B] joystick button
-- START+left arrow - enter the SAVE / [A] joystick menu - select/exit [B] joystick
-- START+right arrow - enter the menu LOAD / [A] joystick - select / exit [B] joystick
-- exit the file menu using the [START] key 

- Auto-start when turned on or hard reset
-- configured in the settings menu [F12] item [AutoRUN]
-- TRD, SCL files from disk A [File TR-DOS]
     if the image was connected in the file menu 
     and the current configuration was recorded [Save config]
-- "fast boot" Slot 0 [QuickSave Slot 0]
  
   That is, after switching on, a fully working machine is loaded 
     with all files and attached disk images and so on,
     which was saved by pressing the [F5] button or from the "fast boot" in slot 0
-- the ability to disable the autostart [OFF]

--- VGA 60Hz firmware  
--- HDMI 90Hz firmware with 1.0 divider
--- HDMI 60Hz firmware with 1.5 divider
--- TFT ili9341 firmware has not been tested
--- the TFT_st7789 firmware has not been tested

 //=============================================================================

