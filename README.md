# Document Classification
Classificate documents on categories


### Requirements
Please see requirements.txt.
<br />
To install these packages, use
```bash
$ pip install -r requirements.txt
```

### Training data
Based on Reuters-21578 files.
<br />
Available in sgm format on 
```bash
classification/data/ 
```
Trained data's topics can be found in
```bash
classification/data/all-topics-strings.lc.txt
```
To train/test, run the following scripts 
from classification/
### Train 
```bash
$ python train_and_classify_reuters_data.py 
```

### Classify 
```bash
$ python test_classifier.py 
```
Will predict the topic for the testing articles from 
```bash
classification/data/reuters_test_json/reuters_test1.json 
```
If all the <i>json</i> testing articles are provided with 
the specific topics field mentioned, 
<br />
it will show the 
<b> [Hit-rate score](http://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html#sklearn.svm.SVC.score) </b> and the <b> [Confusion matrix](http://scikit-learn.org/stable/modules/generated/sklearn.metrics.confusion_matrix.html) </b>. 

### Example
```bash
$ python train_and_classify_reuters_data 
$ python test_classifier.py
```
