# Lenovo-T460-EFI-Hackintosh
Latest EFI for Lenovo T460 using Opencore. Supports the most recent MacOS, Sonoma.
----------------------------------------------------------------------------------
This is my Personal Lenovo T460 OpenCore (OC) EFI that supports most of the features of MacOS.

Whats Working 😃:                                                                      
(-) Wifi (provided you have a wireless intel card supported by IntelWireless)    
                                                                                    
(-) Bluetooth 
                                                                                      
(-) Keyboard 

(-) iServices 
                                                                                              
(-) Trackpad 
                                                                                                                            
(-) Batteries (Programmed a script to load them together as one to enable longer battery life and better performance)                                       
                                                                                                                                              
(-) Overclocking (DO NOT Further try to overclock the PC. Doing this will result in either your battery dying, proccessor melting or the thermal paste fries like chicken)
                                                                                                                                                                            
If you really want to try to overclock this don't go to google and look up "Overclock T460", this will result in you getting wild goose chases and belive me I have tried 😭.
Instead look up a nifty little tool that leverages Intel Turbo Boost Technology, just enable it in the bios, install the program on your new mac and boom, clocked that sucker 
from 2Ghz to 2.7Ghz 😁.

Whats Not working 😭:
                                                                                              
(-) Most of the Continuity Features in MacOS                                                                                              


I have added two EFI's One is for Ventura if you want a much much smoother performance with wifi and iServices, and the other supports Sonoma but uses itlwm.kext which requires you to download heliport in order to use the wifi 💀.
Its not that bad except that the kext is in the development stage and is not stable at all. Best to accept the fact that you don't own you pc anymore if you install Sonoma, your PC owns you and will not hesitate to make you spend countless hours trying to figure out what the fuck happened to it.

Before I leave you to install macos you need balena ether and a vanila image from orillia.com look it up on google cuz I am too lazy to hyper link 💀. (EDIT) Please download SMBIOS Generator and follow intructions to generate your own, it should not be that hard After that your good to go. It should basicly download a image ending with the extension .raw . That is ok and is supposed to be like that, just hit flash from file in balena ether, hit target as your EXTERNAL Flash Drive Don't click internal because its not gonna work like that. After you do that grab another flash drive or unleash your skills of partitioning and mount the already created EFI partition and copy the efi files from there. Final product should either be a single USB with two partitions, one with the raw image flashed on and the other with the EFI to boot the computer. 

If you still are here and you are not crying (yet) go ahead and spam F12 after restarting your computer, it should take you to the boot sector, from there select your flash drive/USB and hit enter, should boot up to OC picker, and select the one that says install macos. Should bring you to the recovery os and hit diskutility, format your PC's SSD or HDD if you're still old, then format as APFS and then exit diskutility and click install Ventura/Sonoma and select the APFS container you just formatted. Now you should go do some yard work because it will take a while for it to get installed. Once your done boot up again from the USB and boot to the same APFS container you formated and mac will boot up. At this point Congratulations, you did it and yet there still is more 😭. I won't go into details but look up Dortinas Opencore guide and navigate to postinstall and follow intructions from there

If you want more stuff like this or custom EFIs for other computers shoot me an email at jpgardzinski@gmail.com and I will be right back with you. Peace out and happy hackintoshing
