# Automated-paper-correction

End-to-end solution for hassle-free paper correction, for universities/teachers/students

## Usage

Clone the repo

    git clone https://github.com/KewalMishra/Automated-Paper-Correction.git
	cd paper-correction


## Installation
**We suggest you create a new environment**
```bash
pip install -r requirements.txt
```
## Run

```python
python app.py
```
The app will be available at  `127.0.0.1:5000/`

## Application description
The application is divided into 4 steps
### Step 1:
1. In step 1 the user is required to upload the student answers.
2. Only PDFs and Images are supported at the moment
3. All the student answers are saved locally in a folder called 'student_files' this folder is created in runtime and is temporary. We also provide an option to upload files to the cloud if required.

![picture](https://bitbucket.org/parthchudasama/paper-correction/raw/06a400646d30b9a416896e31f8af28911a64dc5b/static/screenshots/Step%201.png)

### Step 2:
1. In step 2 user is required to upload a master copy, the data provided in step 1 will be checked  against the master copy i.e the original answers.
![picture](https://bitbucket.org/parthchudasama/paper-correction/raw/06a400646d30b9a416896e31f8af28911a64dc5b/static/screenshots/Step%202.png)

### Step 3:
Handwriting recognition from Google Vision is not 100% accurate. We have ensured through tests that the accuracy remains acceptable using image preprocessing. To further ensure that the words and sentences are detected correctly, we recommend the user upload material that has been used to refer by students (Reference books, papers, etc)
![picture](https://bitbucket.org/parthchudasama/paper-correction/raw/06a400646d30b9a416896e31f8af28911a64dc5b/static/screenshots/step%203.png)

### Step 4:
The last step generates a zip file where each student's results are stored along with a detailed review of each paper.
Please be patient at this step because it might take a while depending upon the network connection.
![picture](https://bitbucket.org/parthchudasama/paper-correction/raw/06a400646d30b9a416896e31f8af28911a64dc5b/static/screenshots/step%204.png)

### Test run
In order to test the application, we have provided some test files which are present in the `test_files` folder.

1. Select any Image/PDF in step 1
2. Select `master_file.txt` in step 2
3. Select `correction_file.txt` in step 3


## License

[MIT](https://choosealicense.com/licenses/mit/)


## License

[MIT](https://choosealicense.com/licenses/mit/)
