# add the user
	adduser yje 
	passwd yje 
	adduser yje sudo
	adduser yje root
# prepare the env
- modefy the source 
	vi /etc/apt/sources.list
- change the default desktop env
	vi ~/.banshrc 
	"cd Desktop"
- add sougo input type
	ref:http://blog.topspeedsnail.com/archives/6948
	sudo apt install -f fcitx-bin fcitx -y
	
	ref-file:http://202.118.253.12/files/31360000016306C4/cdn2.ime.sogou.com/dl/index/1509619794/sogoupinyin_2.2.0.0102_amd64.deb	
	sudo dpkg -i sogoupinyin_2.2.0.0102_amd64.deb

- fanqiang
	- shadowsocks
	sudo apt install python-pip -y 
	sudo pip install shadowsocks
	sudo sslocal -s 104.225.156.218 -p 443 -l 1080 -k hOuvdSTb7n -t 600 -m AES-256-CFB &
	sudo echo "sudo sslocal -s 104.225.156.218 -p 443 -l 1080 -k hOuvdSTb7n -t 600 -m AES-256-CFB &" /etc/rc.local
	- google-chrome
	ref-file:http://www.google.cn/chrome/browser/desktop/index.html
	ref-doc: https://jingyan.baidu.com/article/46650658c18964f549e5f8c3.html
	sudo dpkg -i google-chrome-stable_current_amd64.deb
	sudo apt-get -f install
	- switchyOmega
	ref-file:
	ref-doc:https://www.switchyomega.com/download.html
	- privoxy
	ref:http://www.privoxy.org/user-manual/quickstart.html	
	apt-get install privoxy
	
# install cuda
	ref:http://blog.csdn.net/masa_fish/article/details/51882183
	ref-file:https://developer.nvidia.com/cuda-80-ga2-download-archive
	ref-doc:http://developer2.download.nvidia.com/compute/cuda/8.0/secure/Prod2/docs/sidebar/CUDA_Installation_Guide_Linux.pdf?XsFZciNUIATezVL5kgMeNVlsoVaWExToCf02sGQ_6lMXR_QNvLufftgUy-_QD2K3yJL5bAIEJ8z0eAjoc_3yDBvQN_i3JpxqV_EFxAFI3DvevSUTy-xIoC342LbHgZULTZU8jD2FZLxzQMC8WkQYT0hoQYJdZeA_DWv1UuUOu70JVltiNuJviIUe6Q


