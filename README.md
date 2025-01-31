# BantuMasak App

BantuMasak is an application designed to assist users, particularly housewives, in creating a well-organized plan for the meals they want to prepare over several days. Our team has developed various features to simplify the process of meal planning. 
On the machine learning side, we have built two types of models: a recommendation system and an image classification system. 
Our recommendation system includes two types. First, it provides recipe recommendations by calculating ratings. Second, it suggests menus based on the user's input, specifically the ingredients they have on hand. 
For food classification, users can either upload or scan existing food images from their phones. The application will then predict the name of the food and provide detailed information such as ingredients and complete recipes.

## Project Structure (ML)
For Mid Checkpoint
```bash
.
├── README.md
├── Mid Checkpoint
│   ├── datasets
│   │   ├── Image Classification
│   │   │   └── dataset-food-selected
│   │   │       ├── asinan-jakarta
│   │   │       ├── ayam-bumbu-rujak
│   │   │       ├── ayam-goreng-lengkuas
│   │   │       ├── bika-ambon
│   │   │       ├── cendol
│   │   │       ├── es-dawet
│   │   │       ├── gado-gado
│   │   │       ├── gulai-ikan-asin
│   │   │       ├── kerak-telor
│   │   │       ├── klapertart
│   │   │       ├── kolak
│   │   │       ├── kue-lumpur
│   │   │       ├── kunyit-asam
│   │   │       ├── laksa-bogor
│   │   │       ├── lumpia-semarang
│   │   │       ├── mie-aceh
│   │   │       ├── nagasari
│   │   │       ├── papeda
│   │   │       ├── rendang
│   │   │       ├── rujak-cingur
│   │   │       ├── sate-ayam-madura
│   │   │       ├── sate-meranggi
│   │   │       ├── serabi
│   │   │       ├── soto-ayam-lamongan
│   │   │       └── soto-banjar 
│   │   └── Recommandation System
│   │       ├── preprocessed_dataset.csv (Clean Dataset For RS Based on Input)
│   │       ├── Preprocessing_Dataset_BasedonInput.ipnyb (Code For Preprocessing Data)
│   │       └── recipes_dataset.csv (Dirty Dataset For RS Based on Input)
│   └── Model
│       ├── Image Classification
│       │   └── FirstTF.ipnyb
│       └── Recommendation System
│           ├── RecommendationSystem_Opsi1_ForYou.ipnyb
│           ├── RecommendationSystem_Opsi2_ForYou.ipnyb
│           └── RecommendationSystem_Opsi3_BasedonInput.ipnyb
└── Final Deliverables
    ├── ...
    ...
```

For Final Deliverables
```bash
.
├── README.md
├── Mid Checkpoint
│   ├── ...
│   ...
└── Final Deliverables
    ├── datasets
    │   ├── Image Classification
    │   │   └── dataset-food-selected
    │   │       ├── asinan-jakarta
    │   │       ├── ayam-goreng-lengkuas
    │   │       ├── es-dawet
    │   │       ├── gado-gado
    │   │       ├── gulai-ikan-asin
    │   │       ├── kolak
    │   │       ├── lumpia-semarang
    │   │       ├── mie-aceh
    │   │       ├── rendang
    │   │       ├── rujak-cingur
    │   │       ├── sate-ayam-madura
    │   │       ├── sate-meranggi
    │   │       ├── serabi
    │   │       ├── soto-ayam-lamongan
    │   │       └── soto-banjar 
    │   └── Recommandation System
    │       ├── preprocessed_dataset.csv (Clean Dataset For RS Based on Input)
    │       ├── Preprocessing_Dataset_BasedonInput.ipnyb (Code For Preprocessing Data)
    │       └── recipes_dataset.csv (Dirty Dataset For RS Based on Input)
    └── Model
        ├── Image Classification
        │   └── FirstTF.ipnyb
        └── Recommendation System
            ├── RecommendationSystem_Opsi1_ForYou.ipnyb
            ├── RecommendationSystem_Opsi2_ForYou.ipnyb
            └── RecommendationSystem_Opsi3_BasedonInput.ipnyb
```
## Datasets
We collected the datasets for both the recommendation system and food classification by scraping. For food classification, we scraped images from Google Images, resulting in a dataset with 25 food labels, each containing 50 images. 
On the other hand, for the recommendation system, we scraped data from the cookpad.com website. The dataset includes 800 different recipes, each with the food's title, ingredients, step-by-step instructions for making the dish, and the corresponding image URL.


## Network
For the food classification model, we utilized transfer learning with the ResNet50 architecture. We also incorporated Convolutional Neural Networks (CNNs) into the model, specifically modified for the 25 food labels.
In the case of the recommendation system, we developed two types. The first type, "Recommendation for You," involves calculating ratings and creating an embedding layer to provide suitable recipes for the user. 
The second type of recommendation system is based on user input. We tokenize the ingredients and create an embedding layer to suggest appropriate recipes based on the available ingredients provided by the user.

## Built With
* [Tensorflow Keras](https://www.tensorflow.org) - The AI framework,
* And Other Related Libraries.

## Authors
|          Nama         | Bangkit-ID |       Path       |       Contact       |
|:---------------------:|:----------:|:----------------:|:-------------------:|
|  [Jihan Kamilah](https://github.com/jihanKamilah)  |  M304DSY2993  | Machine Learning | <a href="https://www.linkedin.com/in/jihan-kamilah/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" /></a> |
|  [Santiana](https://github.com/Santiana1922)  |  M304DSY2487  | Machine Learning | <a href="https://www.linkedin.com/in/santiana/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" /></a> |
