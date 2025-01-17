# Updated code for GWC YOLOv5
## Step 0: 
Open your Anaconda Prompt/Powershell/Linux Terminal and put your hands on keyboard. If you still don't have it installed on your PC, click [here](https://www.anaconda.com/download)

## Step 1: 
```shell
git clone https://github.com/0YJ/GWC_YOLOv5.git
cd GWC_YOLOv5
mkdir weights
```
## Step 2: 
Download weight from [link](https://drive.google.com/file/d/1msfpBFOTe_g0Jp3c-DITUglHJaFOSHmk/view?usp=sharing) and put the weight file in "weights" folder.

## Step 3: 
Keep in project folder and do: 
```
conda create -n GWC python=3.8
conda activate GWC
pip install -r requirements.txt
pip install ensemble_boxes
```

## Step 4: 
You can get one test data from [here](https://drive.google.com/file/d/1V5k1wamDO7UmcMn-LIa3HEhf_iDz_EfP/view?usp=drive_link)

## Step 5: 
```
python detect.py --img-size 8000 --name best --weights weights/wheatHead.pt --source /where-you-save-the-test-data --nosave  --max-det 10000 --conf-thres 0.5
```
