# Cheat_Sheets

## Building a Neural Network in PyTorch cheat-sheet / guide

### 1. Importing the data from kaggle

'''

from google.colab import files
files.upload()

'''

Then upload your kaggle api JSON and run the cell

### 2. Create the folders to store the data

'''
#Create the directories for it
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
'''
### 3. Download your selected dataset using the API command

'!kaggle datasets download -d {USER}/{Dataset}'

*E.g. !kaggle datasets download -d shaunthesheep/microsoft-catsvsdogs-dataset *

### 4. Unzip the downloaded dataset
'''
import zipfile
from zipfile import ZipFile
file_name=("microsoft-catsvsdogs-dataset.zip")
with ZipFile(file_name,'r') as zip:
             zip.extractall()
             print("done")
'''


