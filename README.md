Cara instalasi esp8266 wifi hotspot
Teruji di WeMos D1 Mini type C
Alat dan bahan
•	Esp8266+kabel data
•	Putty
•	Flashtool esp8266
•	File bin
Cara
1.	Ambil file bin dan buka espflashtool . dan upload spt berikut. (jan lupa eraser all dulu)
 
2.	Restart esp lwat tombolnya
3.	Buka putty masuk ke 192.168.4.1 7777 (saat default) 4.1 bisa diganti ip gateway jika sudah dimodif
  
4.	Done lakukan perintah dibawah yg sudah teruji. Dan peritah lainya di file pdf sebelah
Perintah teruji
Basic 
•	set ssid your_home_router's_SSID
•	set password your_home_router's_password
•	set ap_ssid ESP's_ssid
•	set ap_password ESP's_password
•	show (to check the parameters)
•	save
•	reset
Again, if you want to enter non-ASCII or special characters you can use HTTP-style hex encoding (e.g. "My%20AccessPoint") or, only on the CLI, as shortcut C-style quotes with backslash (e.g. "My\ AccessPoint"). Both methods will result in a string "My AccessPoint".
Lainnya 
•	set status_led GPIOno: selects a GPIO pin for the status LED (default 2, >16 disabled) set status_led GPIOno: selects a GPIO pin for the status LED (default 2, >16 disabled)
•	With "set status_led GPIOno" the GPIO pin can be changed (any value > 16, e.g. "set status_led 255" will disable the status LED completely). When configured to GPIO1, it works with the built-in blue LED on the ESP-01 boards. However, as GPIO1 is also the UART-TX-pin this means, that the serial console is not working. Configuration is then limited to network access.

Sumber: https://github.com/martin-ger/esp_wifi_repeater 
