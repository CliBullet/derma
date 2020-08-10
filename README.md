# Dermatology Prediction Using Computer Vision<br>
## Getting Started
This AI project is an image classification problem in order to predict whether or not a patient has a particular skin disease.<br>
The disease labeled within the model consist of:<br>
  - Melanoma<br>
  - Basal Cell Carcinoma<br>
  - Benign Keratosis<br>
  - Dermatofibroma<br>
  - Melanocytic Nevi<br>
  - and Vascular Skin Lesion<br>
 
*This model currently preforms its best predictions on the melanocytic nevi class.<br>I would suggest to fine tune the hyperparameters and possibly train on more epochs to
produce better results for ALL of the classes.

### Prerequisites<br>
Step 1: Install Anaconda (or miniconda) depending on if your running this repo locally or via the cloud.<br>
Step 2: Install the Openvino Toolkit on your local machine or via the clous developed by Intel.<br> 
  *The OpenVino toolkit is the secret behind what's considered AI at the edge<br>

### Running the Program<br>
Step 1: Create a new environment using Anaconda<br> 
```
conda create --name [new environment name]<br>
```
  
Step 2: Activate this new environment<br>
```
conda activate [name of environment]<br>
``` 
Step 3: Go the the project directory and install all dependencies located in the requirement.txt file<br>
```
<local directory> conda install -r requirements.txt<br>
```
Step 4: Activate the OpenVino toolkit you downloaded earlier<br>
```
source [opt/intel/openvino/bin]setupvars.sh<br>*Make sure to use your own openvino installation directory where you downloaded the files<br>
```  
Step 5:CD into the project directory via terminal<br>

Step 6: Open the "edge_app.py" file and make sure to change the CPU_EXTENSION as per your installation directory of openvino<br>

### Model Deployment<br>

Run the "app.py" file using the command below:<br>
```
python app.py<br>
``` 
THE PROGRAM SHOULD BEGIN RUNNING SHORTLY WITHIN THE LOCAL TERMINAL.<br>

Now open your browser<br>
```
localhost:5000
```

Click on the yellow button which will direct you a page to upload an image of one of the skin disease listed earlier.<br>

Lastly, upload an image, click on the predicion and you should receive an accuracy score of the predicted disease and the amount of time it took to load the prediction.<br>

### Built With<br>
* [Anaconda](https://www.anaconda.com/products/individual) - Data science toolkit
* [OpenVino](https://software.intel.com/content/www/us/en/develop/tools/openvino-toolkit.html) - The CNN model framework
* [Google Colab](https://colab.research.google.com/notebooks/intro.ipynb) - AI model training on a free GPU and TPU
* [Microsoft Visual Code](https://code.visualstudio.com/) - programming editor for local testing and deployment

## Acknowledgements<br>
Thanks to anyone who has or does contribute to this Nebula project. We are very welcome!

