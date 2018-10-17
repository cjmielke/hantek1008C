# [hantek 1008c](http://www.hantek.com.cn/en/ProductDetail_13_13170.html)

# проект на осцилограф 1008 от фирмы Hantek
# меняем проект c 1008 под осцилограф 1008C :)


пока-что работает только запись пакетов в файл.

Примеры для использования `csvexport.py`:
	`python3 csvexport.py mydata.csv -s 1 2`	запись с двух каналов (*нужно проверить)

TODO:
	- не разобрался как данны воспроизводить с программой 'analysis.py' в проекте.

### Для работы следует установить:
* Python >= 3.6
* pyusb;overrides
* добавить в файл "/etc/udev/rules.d/99-hantek1008.rules" with content => 
	ACTION=="add", SUBSYSTEM=="usb", ATTRS{idVendor}=="0783", ATTR{idProduct}=="5725", MODE="0666"
* sudo udevadm control -R
* переподключить устройство в USB-порт



