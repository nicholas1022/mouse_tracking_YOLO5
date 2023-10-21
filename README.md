This is a mouse tracking application that track single or multiple mice in images or videos.

This application use [YOLOv5](https://github.com/ultralytics/yolov5) of <a href="https://ultralytics.com">Ultralytics</a> and Pytorch to train YOLOv5n with custom mouse dataset.
You can see the [YOLOv5 Docs](https://docs.ultralytics.com) for more understandings of YOLOv5. 
If you want to know how to use this application, you can skip this and see following section.

## <div align="center">Quick Start Examples</div>
Install and detect sections are similar to YOLOv5. You may refer to their example. 
<details open>
<summary>Install</summary>

Clone repo and install [requirements.txt](https://github.com/ultralytics/yolov5/blob/master/requirements.txt) in a
[**Python>=3.6.0**](https://www.python.org/) environment, including
[**PyTorch>=1.7**](https://pytorch.org/get-started/locally/).
<br>*This application is tested in Python==3.7 and PyTorch==1.8.0+cu111.

```bash
git clone https://github.com/nicholas1022/mouse_tracking  # clone
cd mouse_tracking
pip install -r requirements.txt  # install
```

</details>

<details>
<summary>Inference with detect.py</summary>

`detect.py` runs inference on a variety of sources and saving results to `runs/detect`.

```bash
python detect.py --source 0  # webcam
                          img.jpg  # image
                          vid.mp4  # video
                          path/  # directory
                          path/*.jpg  # glob
                          'https://youtu.be/Zgi9g1ksQHc'  # YouTube
                          'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream
```
<br><br>
`detect.py` accepts a series of parameters:
<br>--skip-frame: skip inference of video frames. 10 = infer one-tenth frames, 2 = infer half frames. 1 = no skip
<br>--real-time: real-time playback if --view-img parameter is set
<br>Refer YOLOv5 Doc for other parameters
</details>
