# Document_Classification
Classificate documents on categories


### Requirements
Please see requirements.txt.
<br />
To install those packages, use
$ pip install -r requirements.txt

### Training data
Based on Reuters-21578 files.
<br />
Available in sgm format on 
classification/data/ 
<br />
Trained data's topics can be found in
classification/data/all-topics-strings.lc.txt

### Train 
$ python train_and_classify_reuters_data.py 

### Classify 
$ python test_classifier.py 
<br />
    Will predict the topic for the articles from 
classification/data/reuters_test_json/reuters_test1.json 
<br />
    If all the json testing articles are provided with 
the specific topic/topics, it will show the 
<b> Hit-rate score </b> and the <b> Confusion matrix </b>. 

### Example
$ python train_and_classify_reuters_data 
$ python test_classifier.py
