**Problem statement:** 
To build a CNN based model which can accurately detect melanoma. 
Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. 
A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

**Important Libraries Used:**
tensorflow
matplotlib.pyplot
keras.preprocessing - load_img
seaborn
numpy
pandas
Augmentor
keras
models - Sequential
Optimizers - Adam
callbacks - EarlyStopping
googlecolab - drive

**Approach Followed:**
Step 1: Data Loading to drive, reading images from respective folders for Test and train
Step 2: Setting Parameters: batch size as 32, image heights and width as 180
Step 3: Visualizing the data: Sample image from each class, check size for each class
Step 4: Data Augmentation: As there is class imbalance we will use Augmentor to add additional samples to each class
Step 5: Creating Train and Validation dataset with 80:20 split
Step 6: CNN Model: 3 CV layers >> 1 Drop out >> Flatten >> Dense >> Dropout >> Dense layer with softmax activation func.
Step 7: Model Compilation: Optimizer: Adam, loss: crossentropy
Step 8: Model Training with epochs set at 20

**Model Accuracy Visualization**
Generate Training and Validation accuracy & Loss trend with epochs. Accuracy should gradually increase for both

**Run Model on Test Samples**
Check random samples from test group to see if Actual class and Predictive class match
