<h1>Examining the Role of Color in Predicting Fruit Freshness Using Convolutional Neural Networks</h1>

<h2>Abstract</h2>
Color is a commonly used visual cue for assessing fruit freshness, which is a concern that remains critical in food supply chain management. Computer vision techniques offer a way to reduce the subjectivity and improve the consistency of freshness evaluation. This study uses an image dataset containing eight fruit types, with balanced samples of fresh and rotten images, to investigate how different color transformations influence the behavior of a convolutional neural network. The model is trained on the original images and on five color-based variants, namely grayscale, red-blue channel swap, and isolated red-only, green-only, and blue-only channels, to examine how color information affects classification performance. The model trained on the original images has training and validation accuracies of 91% and 81%, only exceeded by the swap variant with training accuracy 93%. Confusion matrix analyses were primarily utilized to identify performance differences across the variants and highlight fruit-specific trends. This revealed that the swapped variant outperforms the original variant for apples, bananas, guavas, and pomegranates; the red variant beats the original for grapes and oranges; the blue variant surpasses the original for jujubes, while the grayscale variant is an equally-performing alternative for strawberries.

<h2>File Directory</h2>
{VariantName} represents the originnal dataset and five variants used in our study, i.e., Grayscale, Red-Blue Channel Swap, Red-only, Green-only, and Blue-only. 

{ClassName} represents the 16 classes used in our study, composed of eight fruits (apple, banana, grape, guava, jujube, orange, pomegranate, strawberry), each of which has two freshness levels (fresh and rotten).

```text
fruit-cnn/
├── ColorVariants/
│   └── {VariantName}/ (x 6)
│       └── {ClassName}/ (x 16)
│           └── {ClassName} ({Index}).jpg (x 50)
├── Models/
│   └── cnn_{VariantName}.keras (x 6)
├── Results/
│   ├── accuracies.png
│   ├── confusion_matrices.png
│   ├── variants.png
│   ├── SelectedImages/
│   │   └── {ClassName}.png (x 16)
│   └── SelectedSeamCarvedImages/
│       └── {ClassName}.png (x 16)
├── SeamCarvedImages/
│   └── {ClassName}/ (x 16)
│       └── {ClassName} ({Index}).jpg (x 50)
├── MATH 282.1 Project (Cheng, Montemayor).pdf
├── p2.ipynb
├── README.txt
└── requirements.txt
```
    
<h2>Credits</h2>
This project was created by Sted Cheng and Annika Montemayor, and submitted as a requirement for the course <b>MATH 282.1: Computer Vision</b> taken in the first semester of AY 2025-2026 in Ateneo de Manila University. 