# Indian Currency Detection using opencv

This code is based on opencv orb feature detection. SURF and SIFT features can also be used to extract the notes features. You can change the value of number of features detected by changing n_features in detect.py. Further brute force matching is used for matching the templates with existing notes.

## Getting Started

The following instructions will get this project up and running on your local machine for development and testing purposes. 

### Prerequisites

**Dataset**: https://drive.google.com/open?id=1W3xMiVxuCWw58PRCZ3p8IOqROrXe0Y66

Note: Download the __files__ folder on this drive


### Installing

1. Clone this repository:
2. Unzip the files folder downloaded from drive then Copy and Paste it in this cloned repository
    The "files" folder and the python file app.py should be in the same directory
3. Making a virtual environment (Open Terminal):
    
   `cd /path/to/this/repo/CurrencyDetectServer`
    
   `virtualenv env`
   
   `pip install -r requirements.txt`

4. Running the flask server:

    `python app.py`
    

### Running the tests

After running app.py, the flask server will be running at port 4555.

Make Request through Postman

  1. In the body section of Postman, write key as "image" and select type as file

  2. Select a currency image in the value section
    
  3. Send a post request to `localhost:4555/image`

<img src="https://github.com/shivamkumard107/CurrencyDetectServer/blob/master/assets/postman.png" width="700" height="160" />


## Built With

* [Flask](https://flask.palletsprojects.com/en/1.1.x/) - The server used
* [OpenCV](https://docs.opencv.org/3.4/d3/da1/classcv_1_1BFMatcher.html) - The ML implementation


