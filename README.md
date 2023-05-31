# BantuMasak App

We create a Tensorflow model to predict the fresh and rotten fruits. By doing so, we hope we can easily separate fresh and rotten fruits from fruit images. (INI BELUM DIJELASIN)

## Project Structure
```bash
.
├── README.md
├── datasets
│   ├── Image Classification
│   │   └── dataset-food-selected
│   │       ├── asinan-jakarta
│   │       ├── ayam-bumbu-rujak
│   │       ├── ayam-goreng-lengkuas
│   │       ├── bika-ambon
│   │       ├── cendol
│   │       ├── es-dawet
│   │       ├── gado-gado
│   │       ├── gulai-ikan-asin
│   │       ├── kerak-telor
│   │       ├── klapertart
│   │       ├── kolak
│   │       ├── kue-lumpur
│   │       ├── kunyit-asam
│   │       ├── laksa-bogor
│   │       ├── lumpia-semarang
│   │       ├── mie-aceh
│   │       ├── nagasari
│   │       ├── papeda
│   │       ├── rendang
│   │       ├── rujak-cingur
│   │       ├── sate-ayam-madura
│   │       ├── sate-meranggi
│   │       ├── serabi
│   │       ├── soto-ayam-lamongan
│   │       └── soto-banjar 
│   └── Recommandation System
│       ├── filekotor.csv
│       └── filebersih.csv
└── Model
    ├── Image Classification
    │   └── fileclassification.ipnyb
    └── Recommendation System
        ├── filerecommendation_opsi1.ipnyb
        └── filerecommendation_opsi2.ipnyb
```

## Datasets
For the Food Classification dataset (image) I got it by scraping data on Google Image, each class has 50 images, so total is 1250 (split into 80:20 for train:test). And, for system recommendations I get from scraping data on the cookpad.com website.



## Network
For this model, we use Convolutional Neural Networks. Our model used transfer learning InceptionV3 for the baseline model with 6 classes (Fresh and Rotten banana, apple, and orange). We also using VGG16 for the improved model with 2 classes (Fresh and Rotten Fruit) as our final model. (INI MASIH BINGUNG)

## Prequisites
You don't need to install anything since its written in Google Colab which is a cloud service
- Copy this repository link into the collab https://github.com/Bangkit-JKT2-D/fruits-fresh-rotten-classification/blob/master/fresh-rotten-fruits-improve.ipynb
- After succesfully open the notebook, create cookies.txt for downloading the dataset from kaggle
- First of all, With the assumption of using Google Chrome, download extension [cookies.txt](https://chrome.google.com/webstore/detail/cookiestxt/njabckikapfpffapmjgojcnbfjonfjfg)
- Open the kaggle link dataset [fruit-rotten-dataset](https://www.kaggle.com/sriramr/fruits-fresh-and-rotten-for-classification) then on your right top corner of browser, choose the cookies.txt.
- download the cookies.txt.
- upload the cookies.txt on the notebook as what required

## Built With
* [Tensorflow Keras](https://www.tensrflow.org) - The AI framework used

## Authors
* **Jihan Kamilah**  - [jihanKamilah](https://github.com/jihanKamilah)
* **Santiana**       - [santiana](https://github.com/...)
