# install-double-system-win7-ubuntu
the problem i meet
first system is win7
use ultraiso and easybcd make usb system disk

download from https://mirrors.tuna.tsinghua.edu.cn/ubuntu-releases/16.04.4/
notice:desktop version is different from sever veersion

the way use ultraiso make usb system disk is baidu,very easy.

one ubuntu system you'd better set 4 part, 
/ 'pirmary 100g function like cdisk in win7,contain unbuntu system' 
/boot 'logical use to contain start up boot' 
/home 'logical 400g' 
swap '12g exchange space' 

the most important thing is the start up boot set,always bug is relate to it

when i install ubuntu under win7 often happen:
intall error,if i don't set elf
can not find ubuntu startup,if i set start up boot in ubuntu boot,this is coused by win7 startup cant find it
can not find win7 start up,if i don't set elf
the right way to intall need set elf and set start up boot in sda1 (the system disk of win7,and win7 start up is in it also) in
order to make the two start up boot together

/ 'pirmary 100g function like cdisk in win7,contain unbuntu system' 
/boot 'logical use to contain start up boot' 
/home 'logical 400g' 
swap '12g exchange space' 
elf 'important save win7 start up boot'

