# vm_macos
setup mac os on vm (virtual box)
  
https://beginpc.ru/raznoe/install-macos-mojave-on-virtualbox
https://yandex.ru/turbo/lifehacker.ru/s/kak-ustanovit-macos-cherez-virtualnuyu-mashinu/

VBoxManage modifyvm mactest --cpuidset 00000001 000106e5 00100800 0098e3fd bfebfbff
VBoxManage setextradata mactest "VBoxInternal/Devices/efi/0/Config/DmiSystemProduct" "iMac11,3"
VBoxManage setextradata mactest "VBoxInternal/Devices/efi/0/Config/DmiSystemVersion" "1.0"
VBoxManage setextradata mactest "VBoxInternal/Devices/efi/0/Config/DmiBoardProduct" "Iloveapple"
VBoxManage setextradata mactest "VBoxInternal/Devices/smc/0/Config/DeviceKey" "ourhardworkbythesewordsguardedpleasedontsteal(c)AppleComputerInc"
VBoxManage setextradata mactest "VBoxInternal/Devices/smc/0/Config/GetKeyFromRealSMC" 1
VBoxManage setextradata mactest VBoxInternal2/EfiHorizontalResolution 1440
VBoxManage setextradata mactest VBoxInternal2/EfiVerticalResolution 900


VBoxManage registervm /home/sergiy/VirtualBox VMs/Ubuntu1804/Ubuntu1804.vbox
VBoxManage list vms
VBoxManage list vms --long

https://support.apple.com/ru-ru/HT201372
https://www.imymac.com/ru/mac-tips/mac-os-high-sierra-download-dmg.html
  
  kpartx linux util for img dmg iso
