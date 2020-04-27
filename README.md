# YOLOv3

Keras(Tensorflow v2 backend) implementation of yolo v3 objects detection. 

## Requirement
- OpenCV 4.2.0
- Python 3.8.2  
- Tensorflow-gpu 2.2.0  
- Keras 2.3.1
- Numpy

### Installation
```bash
git clone https://github.com/waasnipun/object-detection-YOLOv3.git
cd object-detection-YOLOv3

install python3
install opencv

# using pip3
pip3 install numpy 
pip3 install tensorflow-gpu 
pip3 install keras 
```


## Quick start

- Download official [yolov3.weights](https://pjreddie.com/media/files/yolov3.weights) and put it on top folder of the project.

- Run the follow command to convert darknet weight file to keras .h5 file. The `yad2k.py` was modified from [allanzelener/YAD2K](https://github.com/allanzelener/YAD2K) to support for v3.
```
python3 yad2k.py cfg/yolo.cfg yolov3.weights
```

- run follow command to show the demo. The result can be found in `images\res\` folder and `videos\res\`.
```
python3 demo.py
```

## Results

<img width="400" height="350" src="/images/res/person.jpg"/><img width="400" height="350" src="/images/res/dog.jpg"/>
<img width="400" height="350" src="/images/res/rd2-2.png"/><img width="400" height="350" src="/images/res/giraffe.jpg"/>

## Original Work

- [allanzelener](https://github.com/allanzelener/YAD2K)
 
## Reference

- [official YOLO website](https://pjreddie.com/darknet/yolo/)	
- [allanzelener](https://github.com/allanzelener/YAD2K)


## Copyright
See [LICENSE](LICENSE) for details.
