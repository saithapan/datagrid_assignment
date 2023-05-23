# DataGrid Assignment

## Prerequisites

- Before going further steps please Download the dataset from [here](https://catalog.data.gov/dataset/consumer-complaint-database). Extract the CSV File and place in it input folder. Since this is large dataset it not possible to share it in github

## Installation

- Clone the code from this repo
- Create new environment and requirements.txt file

```commandline
conda create --name <env_name> python=3.9
conda activate <env_name>
pip install -r requirements.txt
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu117
```

## Setup

- Run Project in New terminal

```shell
flask run
```
## Django App main files explanation
1. `ImageText/urls.py` - Main app script containing the API endpoints 
2. `ImageText/views.py` - Actual logic written here in class based views 
3. `config.py` - App configurations details like tesseract path

## Testing the api

### In Postman

- Once server started running
- Now Open Postman, select POST Method and provide this url(http://127.0.0.1:8000/img_upload)
- Now select Body -> form-data -> In key provide key name as `file` and select type as `file` and upload
  the `sample.png` file and click send button
-![image](https://github.com/saithapan/cognida_assignment/assets/36238978/7afe0504-1bda-47e7-84bc-f41d43aa0df7)
- **Output Sample Image:-**
- ![image](https://github.com/saithapan/cognida_assignment/assets/36238978/5f1c299a-4c31-4532-8b38-e4cc0b6a1e33)


