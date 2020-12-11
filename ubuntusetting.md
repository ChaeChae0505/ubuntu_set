0. sudo gedit ~/.bashrc 
1. chrome install
2. untitled Document in right click 
	$ touch ~/Templates/"Untitled Document"
3. install korea key
	$ ibus-setup 
	> input method 
	> add
	> korea
	
	settings > launguage > keyboard hanguel 추가!
[4. nvdia driver setting](#4,5-solution)
[5. cudnn install] 

#### 4,5 solution
```
$ sudo lshw -C display 
- see your driver version everything
$ nvidia-smi 
- driver version check
$ ubutntu-drivers devices
- recommended > drive install
```
