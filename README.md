
### Documentation

See the [YOLOv5 Docs](https://docs.ultralytics.com/yolov5) for full documentation on training, testing and deployment. See below for quickstart examples.

<details open>
<summary>Install</summary>

Clone repo and install [requirements.txt](https://github.com/ultralytics/yolov5/blob/master/requirements.txt) in a
[**Python>=3.7.0**](https://www.python.org/) environment, including
[**PyTorch>=1.7**](https://pytorch.org/get-started/locally/).

```bash
git clone https://github.com/avlo2000/yolov5-aeromilitary.git
cd yolov5-aeromilitary
python3 -m pip install --user virtualenv
python3 -m venv env
source env/bin/activate
pip install -r requirements.txt
```

</details>


### Inference with detect.py

`detect.py` runs inference on a variety of sources, downloading [models](https://github.com/ultralytics/yolov5/tree/master/models) automatically from
the latest YOLOv5 [release](https://github.com/ultralytics/yolov5/releases) and saving results to `runs/detect`.

```bash
python detect.py --weights assets/best_baseline.pt --source 0                               # webcam
                                                   img.jpg                         # image
                                                   vid.mp4                         # video
                                                   screen                          # screenshot
                                                   path/                           # directory
                                                   list.txt                        # list of images
                                                   list.streams                    # list of streams
                                                   'path/*.jpg'                    # glob
                                                   'https://youtu.be/Zgi9g1ksQHc'  # YouTube
                                                   'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream
                                                   --conf-thres 0.25 # Confidence threshold more model
                                                                     # Bigger threshold -> less false positives
                                                                     # Smaller threshold -> less false negatives
```



