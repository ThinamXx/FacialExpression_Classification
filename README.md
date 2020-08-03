## **Facial Expression Classification**

**Fastai Library or API**
- [Fastai](https://www.fast.ai/about/) is a deep learning library which provides practitioners with high-level components that can quickly and easily provide state-of-the-art results in standard deep learning domains, and provides researchers with low-level components that can be mixed and matched to build new approaches.

**Data Preparation**
- I have prepared the Data for this project from Google Images. Inorder to achieve the high accuracy, preparing Dataset using own Images is prefered because Google Images are not always accurate. Inspite of those challenges this Model can classify the **Facial Expression**.
- For the Data, you should have to go [Google Images](https://images.google.com/)
```javascript
urls=Array.from(document.querySelectorAll('.rg_i')).map(el=> el.hasAttribute('data-src')?el.getAttribute('data-src'):el.getAttribute('data-iurl'));
window.open('data:text/csv;charset=utf-8,' + escape(urls.join('\n')));
```

## **Snapshot of the Training Data**.
![Image](https://res.cloudinary.com/dge89aqpc/image/upload/v1595263839/1_duhky8.png)

## **Snapshot of the Predicted Image**.
![Image](https://res.cloudinary.com/dge89aqpc/image/upload/v1595263853/2_shyhkx.png)
