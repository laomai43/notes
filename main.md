#tmux
* 当前窗口全屏 ctl+b, z
* 开鼠标功能，以下几行配置加到 ~/.tmux.conf 中 
 
* ```
setw -g mouse-resize-pane on
setw -g mouse-select-pane on
setw -g mouse-select-window on
setw -g mode-mouse on
```

#dlib
* 安装

* ```  
sudo apt-get install build-essential cmake  
sudo apt-get install libgtk-3-dev  
sudo apt-get install build-essential cmake libgtk-3-dev libboost-all-dev  
sudo pip install dlib  
```

* [检测人脸](https://github.com/mit-nlp/MITIE/blob/master/dlib/python_examples/face_detector.py)

* ```python
import sys
import dlib
from skimage import io
detector = dlib.get_frontal_face_detector()
img = io.imread(f)
dets = detector(img, 1)
```

#python
* [call system commands](https://docs.python.org/2/library/subprocess.html)

* ```
subprocess.call(["ls", "-l"])
subprocess.call("exit 1", shell=True)
```

* sprintf like functionality in Python

* ```
print "This is the {}th tome of {}".format(5, "knowledge")
```
This is the 5th tome of knowledge  

* 支持非ASCII字符。

* ```
# -- coding: utf-8 --
```