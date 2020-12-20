https://www.brachiograph.art/index.html

#### Prerequisite:
Raspberry Pi OS is installed and upgraded.

#### Build the plotter

References:

- https://www.brachiograph.art/get-started/build.html
- https://www.brachiograph.art/get-started/wiring.html
- https://www.raspberrypi.org/documentation/usage/gpio/
- https://pinout.xyz/

#### Install the software
Install system packages:
```
sudo apt install -y python3-venv pigpiod libjbig0 libjpeg-dev liblcms2-2 libopenjp2-7 libtiff5 libwebp6 libwebpdemux2 libwebpmux3 libzstd1 libatlas3-base libgfortran5 git
```
Set up a virtual environment
```
python3 -m venv env
source env/bin/activate
```
Clone the BrachioGraph repository
```
cd
git clone https://github.com/evildmp/BrachioGraph.git
```
Install Python packages
```
cd BrachiGraph
pip install -r requirements.txt
```

#### Start up the BrachioGraph
Power up the Raspberry Pi and test from Python Shell.
https://www.brachiograph.art/get-started/drive.html

#### Run example code
- Take photo and Draw
```
cd ~/BrachiGraph
wget -O - https://raw.githubusercontent.com/Shumingx/hello-pi/main/projects/brachio-graph/cam_draw.py > cam_draw.py
python3 cam_draw.py
```

- Draw a map
```
cd ~/BrachiGraph
wget -O - https://raw.githubusercontent.com/Shumingx/hello-pi/main/projects/brachio-graph/map_draw.py > map_draw.py
python3 map_draw.py
```










#### some good libraries
https://gpiozero.readthedocs.io/en/stable/index.html
