# arch-manjaro-utils

- Fix optimus manager 

https://github.com/Askannz/optimus-manager/issues/272
yay -S $(pacman -Qoq /usr/lib/python3.9) --answerclean All

- Install wifi driver

Rtl8852ae

instalar kernel headers para el kernel que tenga (yay kernel headers)
Bajar https://github.com/lwfinger/rtw89\
(estas instrucciones están en el readme del git)
cd rtw89
make
sudo make install 

sudo modprobe rtw89pci            #This loads the module
sudo modprobe -r rtw89pci         #This unloads the module
