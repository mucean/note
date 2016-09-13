## install

### reference

[first repackage](http://www.time-track.cn/install-youdaodict-in-xenial.html)
[install](http://blog.csdn.net/qianggezhishen/article/details/49208689)

### step

    dpkg -X ./youdao-dict_1.1.0-0-ubuntu_amd64.deb  youdao
    dpkg -e ./youdao-dict_1.1.0-0-ubuntu_amd64.deb youdao/DEBIAN
    dpkg-deb -b youdao youdaobuild/

    sudo dpkg -i youdao-dict_1.0.2~ubuntu_amd64.deb
    sudo apt-get install python3-pyqt5
    sudo apt-get -f install
    sudo dpkg -i youdao-dict_1.0.2~ubuntu_amd64.deb
