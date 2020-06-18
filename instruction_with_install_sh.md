# Инструкция по запуску
## Перед запуском, пожалуйста, прочитайте всю инструкцию  

- Скачайте архив с гугл диска нашей команды  
- Подключитесь к Wi-Fi сети, которую раздает коптер (имеет название `CLEVER-XXXX`, где X - цифра)  
- Скопируйте архив на Raspberry Pi с помощью программы FileZilla в папку `/home/pi/`  
- УДАЛИТЕ АРХИВ ИЗ ЗАГРУЗОК ВАШЕГО ПК!!!  
- Скопируйте файл `install.sh` на Raspberry Pi с помощью программы FileZilla в папку `/home/pi/`  
- Откройте страницу `http://192.168.11.1`  
- Откройте веб-терминал `Open web terminal (Butterfly)` 
- Запустите файл `install.sh`:  
`source install.sh`    
- Запустите код, используя следующую команду:  
`roslaunch l22_aero_code run.launch`  

## После запуска кода
- Откройте страницу `http://192.168.11.1`
- Откройте список топиков `View image topics (web_video_server)`
- Откройте топик `/qr_debug` (вывод распознавания qr-кода)  
- Затем откройте топик `/l22_aero_color/debug_img` (вывод изображения с распознанными цветными маркерами)  

## После выполнения кода
- Завершите выполнение roslaunch комбинацией ```Ctrl+C```
- Скопируйте видео из папки `/home/pi/L22_AERO_LOG/` на ПК с помощью программы FileZilla  
- Отправьте это видео нам