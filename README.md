# Mv
project 1 Datasets

A bunch of some 200 datasets. You can call it mini-kaggle :)

Download multiple data in csv file from here Want to download any csv file for local use? Follow the steps mentioned below: 👇

Go to a csv file in a repository of your choice
From the top right bar just above the file section, select and click on "Raw" button
A page will appear with comma separated data with no styling
Copy the page url
Make a folder in your desktop
Open that folder in your favourite code editor and make a simple python file inside the folder. Name it as you please.
Copy this code [From the section below]
Run the python file
The csv file will get downloaded within sometime, depending upon file size
Now you are ready the use it locally!!

import requests import pandas as pd url = '{(copied url here)}' res = requests.get(url, allow_redirects=True) with open('download_file_name.csv','wb') as file: file.write(res.content) download_file_name = pd.read_csv('download_file_name.csv')
