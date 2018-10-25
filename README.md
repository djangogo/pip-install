# pip-install
This repo demonstrate how to install pip's latest version


## 1.安装ubuntu系统自带的pip
（注意安装顺序，否则安装之后pip就会指向pip3，必须首先安装pip3然后安装pip2）

这里会安装到/usr/lib/python2.7/dist-packages/pip和/usr/lib/python2.7/dist-packages/pip3这个位置了

安装pip3
``` bash
    sudo apt install python3-pip
```
安装pip2
``` bash
    sudo apt install python-pip
```


## 2. 利用系统的pip更新pip自己
更新新的pip到/usr/local/lib/python2.7/dist-packages/pip和/usr/local/lib/python2.7/dist-packages/pip3这个位置了
更新pip3
``` bash
    sudo -H pip3 install -U
```

更新pip3
``` bash
    sudo -H pip install -U
```


## 3. 删除系统自带的pip，防止冲突
``` bash
    sudo apt remove python3-pip python-pip
```

## 4. 设置pip的源为清华的源
``` bash
    pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
    pip3 config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
```
