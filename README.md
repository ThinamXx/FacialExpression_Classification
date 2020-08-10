## **Facial Expression Classification**


**Fastai Library or API**
- [Fast.ai](https://www.fast.ai/about/) is the first deep learning library to provide a single consistent interface to all the most commonly used deep learning applications for vision, text, tabular data, time series, and collaborative filtering.
- [Fast.ai](https://www.fast.ai/about/) is a deep learning library which provides practitioners with high-level components that can quickly and easily provide state-of-the-art results in standard deep learning domains, and provides researchers with low-level components that can be mixed and matched to build new approaches.

**Data Preparation**
- I have prepared the Data for this project from **Google Images**. Inorder to achieve more accurate classification, Dataset can be prepared from own Images because **Google Images** are not always accurate, it might contains Duplicate Images, Misplaced or Misclassified Images and many more which will utlimately affect the accuracy of the Model. Despite of those challenges, this Model can still classify Images with **High Accuracy.**
- To prepare the Data from **Google Images**, you should have to go [Google Images](https://images.google.com/) and search for the images you are interested in. The more specific you are in your Google Search, the better the results and the less manual pruning you will have to do. Then you should copy and paste the following Javascript.

```javascript
urls=Array.from(document.querySelectorAll('.rg_i')).map(el=> el.hasAttribute('data-src')?el.getAttribute('data-src'):el.getAttribute('data-iurl'));
window.open('data:text/csv;charset=utf-8,' + escape(urls.join('\n')));
```
**Objectives and Target**
* The Model can classify:
  * Happy Face
  * Sad Face
  * Surprise Face
  * Laughing Face

**Preparing the Model**
- I have used [Fastai](https://www.fast.ai/about/) API to train the Model. It seems quite challenging to understand the code if you have never encountered with Fast.ai API before.
One important note for anyone who has never used Fastai API before is to go through [Fastai Documentation](https://docs.fast.ai/). And if you are using Fastai in Jupyter Notebook then you can use doc(function_name) to get the documentation instantly.

**Snapshot of the Input Images**

![Image](https://res.cloudinary.com/dge89aqpc/image/upload/v1596440928/AA_wpjtcm.png)

**Training of the Data**
- Fastai Library requires very little bit of code to produce the high accuracy result.
- Snapshot of the Code:

![Image](https://res.cloudinary.com/dge89aqpc/image/upload/v1596718189/Accura_lxklzq.png)

**Interpretation**
- Fastai also provides fast Interpretation. Here, I have used Fastai API to draw the Confusion matrix.

![Image](https://res.cloudinary.com/dge89aqpc/image/upload/v1596441603/COnf_yqt7zg.png)

**Putting the Model in Production**
- I have tested the Model to classify the Laughing Face of a person.
- Snapshot of the Result:

![Image](https://res.cloudinary.com/dge89aqpc/image/upload/v1596441792/Resu_kxnxde.png)

