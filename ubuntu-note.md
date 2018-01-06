这个文档中的内容参考markdown的语法进行，具体为：http://xianbai.me/learn-md/index.html

# 1. add the user
	adduser yje 
	passwd yje 
	adduser yje sudo
	adduser yje root
# 2. prepare the env
## 2.1 change the source 
	vi /etc/apt/sources.list
## 2.2 change the default desktop env
	vi ~/.banshrc 
	"cd Desktop"
## 2.3 add sougo input type
	ref:http://blog.topspeedsnail.com/archives/6948
	sudo apt install -f fcitx-bin fcitx -y
	
	ref-file:http://202.118.253.12/files/31360000016306C4/cdn2.ime.sogou.com/dl/index/1509619794/sogoupinyin_2.2.0.0102_amd64.deb	
	sudo dpkg -i sogoupinyin_2.2.0.0102_amd64.deb

# 3. fanqiang
## 3.1 shadowsocks
	sudo apt install python-pip -y 
	sudo pip install shadowsocks
	nohup sslocal -s 104.225.156.218 -p 443 -l 1080 -k hOuvdSTb7n -t 600 -m AES-256-CFB &
	vi /etc/profile # add the last line 
## 3.2 google-chrome
	ref-file:http://www.google.cn/chrome/browser/desktop/index.html
	ref-doc: https://jingyan.baidu.com/article/46650658c18964f549e5f8c3.html
	sudo dpkg -i google-chrome-stable_current_amd64.deb
	sudo apt-get -f install
## 3.3 switchyOmega
	ref-file:
	ref-doc:https://www.switchyomega.com/download.html
## 3.4 privoxy
	ref:http://www.privoxy.org/user-manual/quickstart.html	
	apt-get install privoxy
# 4. install cuda
## 4.0 安装cuda
	ref:http://blog.csdn.net/masa_fish/article/details/51882183
	ref-file:https://developer.nvidia.com/cuda-80-ga2-download-archive
	ref-doc:http://developer2.download.nvidia.com/compute/cuda/8.0/secure/Prod2/docs/sidebar/CUDA_Installation_Guide_Linux.pdf?XsFZciNUIATezVL5kgMeNVlsoVaWExToCf02sGQ_6lMXR_QNvLufftgUy-_QD2K3yJL5bAIEJ8z0eAjoc_3yDBvQN_i3JpxqV_EFxAFI3DvevSUTy-xIoC342LbHgZULTZU8jD2FZLxzQMC8WkQYT0hoQYJdZeA_DWv1UuUOu70JVltiNuJviIUe6Q

## 4.2 安装 cuDNN
	ref:https://developer.nvidia.com/rdp/cudnn-download
	ref-doc:http://developer2.download.nvidia.com/compute/machine-learning/cudnn/secure/v6/prod/Doc/cudnn_install-2.txt?JE2p8dLJwV6NgESpgPGTt5-hyrwqWUIu4F3rlPd5OSf9e3DO2nzZlVaKNPpIT_HGPB_mohmWnLQVTwH0wiWBsIEP9RM3NlNFfyUXo7ffVAYSNfQpQMrR0HVz7blCtd4o9PP3pzf9TwoLvRqucIB5T3R0t4BlBHIuhQXaG9oBbmtOmzAY
	
## 4.3 安装 pycharm + virtualenv + 
	ref-file:https://www.jetbrains.com/pycharm/
	sudo apt-get install python-pip python-dev python-virtualenv
	virtualenv --system-site-packages
	source ~/tensorflow/bin/activate
	easy_install -U pip
	pip install --upgrade tensorflow-gpu 
	
## 4.4 参考tensorflow.org官网
	vi /etc/hosts
	
	#TensorFlow start  from https://github.com/tensorflow/tensorflow/issues/3834 
	64.233.188.121  www.tensorflow.org
	#TensorFlow end
	
	sudo /etc/init.d/networking restart
	
