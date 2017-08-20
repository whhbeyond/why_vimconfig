# whh_vimconfig
it is the vim config of the ubuntu PC and the server of company.
### vimconfig of ubuntu PC
1）####下载vundle 
git clone https://github.com/gmarik/vundle.git ~/.vim/bundle/vundle

2）打开一个vim, 运行:BundleInstall 
下载对应的bundle

3）安装ycm 
cd ~/.vim/bundle/YouCompleteMe 
./install.sh –clang-completer 
将ycm_extra_conf.py文件改为.ycm_extra_conf.py拷贝到~/.vim文件夹下 
安装ycm如何报错找不到python.h的头文件的解决方案是： 
sudo aptitude install python-dev 
如果还有问题，请访问https://github.com/Valloric/YouCompleteMe#ubuntu-linux-x64-super-quick-installation

将mktag脚本拷贝到/usr/bin路径下，然后chmod之后即可通过mktag自动生成 
ctags和cscope。具体用法参考mktag –help

将command.sh拷贝到.vim文件夹下

增加插件command-t 
需要当前环境已经安装ruby，如果使用报错，解决方案： 
sudo aptitude install ruby-dev 
cd ~/.vim/bundle/command-t/ruby/command-t/ 
ruby extconf.rb && make
### vimconfig of the server of company
将bashrc，vimrc和.vim拷贝到当前home路径下即可。
