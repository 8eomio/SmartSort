# AI 분리수거 도우미 똑똑수거
## SmartSort: AI Trash Sorting System
![smartsort_teaser](https://github.com/8eomio/SmartSort/assets/61742009/ca238791-1d4f-4fa0-b93b-84f725b23760)

### Installation 


Clone this repository 
```bash
git clone https://github.com/media-project-2021/media-project.git
cd media-project/
```
Create environment 
```bash
conda env create -n waste_clf
```

Activate environment 
```bash
conda activate waste_clf
```

Install dependencies 
```bash
pip install -r requirements.txt
pip install flask
pip install flask_socketio 
```

### Datasets & Training  
Datasets are collected by human effort, downloaded from several internet sites (kaggle, google, naver)
you can acquire our collected data from https://drive.google.com/drive/u/1/folders/1rsNvi2tOihz8pTIm1zLYmVx6Eiwd_4XN

To train our model, run the below code:
```bash
python train.py
```
after train finished _pth. formatted file will located in same directory. 

### Download trained network
our trained model file can be downloaded from https://drive.google.com/file/d/1PVe8MJyvTcWFaAXhzJn6n7rBhVwbx5nq/view?usp=sharing
make sure downloaded model file in same directory with video_stream.py


### WebUI
Open 2 terminals
First terminal, execute video_stream.py
```bash
python video_stream.py
```
if code doesn't work, try to change load_checkpoint('FINAL.pth') into load_checkpoint('your directory path+FINAL.pth')

Second terminal, go to project directory
run the below code. 
```
npm install
npm install react-router-dom
npm install socket.io-client
npm start
```
once you executed above code, you can just run below code for next time.  
```
npm start
```

### UI illustration 

![image](https://user-images.githubusercontent.com/61742009/146537336-1309d9a2-9a3d-4e8c-ac1e-fcbd05eef9fa.png)
![image](https://user-images.githubusercontent.com/61742009/146537356-7014b7c5-228e-44d2-ac9f-c8d348d5efb1.png)
 

### Acknowledgements 
This work was done for 2021-2 mediaproject. If you have questions, contact aidbeomjo@ajou.ac.kr
