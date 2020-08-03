## **Facial Expression Classification**

**Fastai Library or API**
- [Fastai](https://www.fast.ai/about/) is a deep learning library which provides practitioners with high-level components that can quickly and easily provide state-of-the-art results in standard deep learning domains, and provides researchers with low-level components that can be mixed and matched to build new approaches.

**Data Preparation**
- I have prepared the Data for this project from **Google Images**. Inorder to achieve more accurate classification, Dataset can be prepared from own Images because **Google Images** are not always accurate, it might contains Duplicate Images, Misplaced or Misclassified Images and many more which will utlimately affect the accuracy of the Model. Despite of those challenges, this Model can still classify Images with **High Accuracy.**
- To prepare the Data from **Google Images**, you should have to go [Google Images](https://images.google.com/) and search for the images you are interested in. The more specific you are in your Google Search, the better the results and the less manual pruning you will have to do. Then you should copy and paste the following Javascript.
```javascript
urls=Array.from(document.querySelectorAll('.rg_i')).map(el=> el.hasAttribute('data-src')?el.getAttribute('data-src'):el.getAttribute('data-iurl'));
window.open('data:text/csv;charset=utf-8,' + escape(urls.join('\n')));
```
**Objectives and Target**
- This Model can predict:
-- Happy Face

## **Snapshot of the Training Data**.
![Image](https://res.cloudinary.com/dge89aqpc/image/upload/v1595263839/1_duhky8.png)

## **Snapshot of the Predicted Image**.
![Image](https://res.cloudinary.com/dge89aqpc/image/upload/v1595263853/2_shyhkx.png)
