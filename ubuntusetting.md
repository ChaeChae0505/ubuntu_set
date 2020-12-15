
## Ubuntu 설정하기!
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
[5. cuda install](#CUDA)
[5. cudnn install](#CUDNN)



------------------------------------------------------------------------------
#### 4,5 solution
```
$ sudo lshw -C display 
- see your driver version everything
$ nvidia-smi 
- driver version check
$ ubutntu-drivers devices
- recommended > drive install
$ sudo add-apt-repository ppa:graphics-drivers/ppa
- add repository함
$ sudo apt-get install nvidia-driver-<recommended>
successfully >> nvidia-smi check
```

#### CUDA
- 우선 [cuda](https://developer.nvidia.com/cuda-10.1-download-archive-base?target_os=Linux&target_arch=x86_64&target_distro=Ubuntu&target_version=1804&target_type=debnetwork)
version에 맞게 설치 한 후 설치된 폴더 안으로 들어가서 아래 실행!

local을 설치하자! 그게 훨씬 빠르고 쉽다
software & update > other software가면 repository 추가 한 부분 apt-key 부분 확인 가능
```
`sudo dpkg -i cuda-repo-ubuntu1804-10-1-local-10.1.105-418.39_1.0-1_amd64.deb`
`sudo apt-key add /var/cuda-repo-<version>/7fa2af80.pub`
`sudo apt-get update`
`sudo apt-get install cuda`


~/.bashrc에 아래 부분 추가
export PATH=$PATH:/usr/local/cuda-10.1/bin
export CUDADIR=/usr/local/cuda-10.1
export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/local/cuda-10.1/lib64

```
#### CUDNN
- [cudnn](https://developer.nvidia.com/rdp/cudnn-archive)
- 3개 다운 받고 sudo dpkg -i < 다운 받은 것들 deb >

---------------------------------------------------------------------------------------------------

#### ROS install
- [install wiki](http://wiki.ros.org/melodic/Installation/Ubuntu)


### Git
```
first time 
$ git init
$ git add .
$ git status
$ git config --global user.email " "
$ git config --global user.name " "
$ git commit -m " "
$ git remote add origin {url}
$ git push -u origin master



$ rm -rf ./.git : git remove
$ git init : git initialize
$ git add . : every file updating local git
$ git status : status in local git
$ git commit -m "1st" : git commit message
$ git remote -v : when your git origin status
$ git push origin master : update local git ----> github 

$ git checkout -b <branch> : new <branch> and check in <branch> // local
$ git push --set-upstream origin <branch> : local branch upstream branch git hub 
```
