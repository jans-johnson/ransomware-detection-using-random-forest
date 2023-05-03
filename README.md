# Ransomware Detection Using Random Forest Method

Ransomware is a type of malware from cryptovirology that threatens to publish the victim's personal data or permanently block access to it unless a ransom is paid off. While some simple ransomware may lock the system without damaging any files, more advanced malware uses a technique called cryptoviral extortion.

Nowadays, the ransomware became a serious threat challenge the computing world that requires an immediate consideration to avoid financial and moral blackmail. So, there is a real need for a new method that can detect and stop this type of attack. Most of the previous detection methods followed a dynamic analysis technique which involves a complicated process. The present study proposes a novel method based on static analysis to detect ransomware. Specific features of an infected file can be extracted and trained using ML algorithms to predict if the file is ransomware or not.

The python libraries used are -
- pefile
- os
- hashlib
- array
- math
- pandas
- sklearn

## Steps for the Creation of Model and testing

1. Obtain the ransomware and goodware files from  different websites and group them in two seperate folders named as `malicious` and `legitimate`

2. Use `Data Collection.ipynb` to extract the required features from the obtained files

3. The data will be stored into `output.csv`

4. Use `Preprocessing and training.ipynb` for removing the duplicates and training the model using Random Forest Algorithm. The accuracy of the model can also be predicted here. Save the model afterwards as rf_model.pkl

5. Use `Predict File.ipynb` for testing the model on an external file.


The dataset consisted of about 1000 ransomware files and 1000 goodware files. The essential features were extraced and then stored into a CSV file and then trained using the random forest algorithm and an accuracy of 92% was obtained.