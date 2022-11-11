# Monkeypox-Classification

Monkeypox is a viral disease affecting both humans and animals. It is casued by the Monkeypox Virus which is zoonotic and is of the family Orthopoxviruses The ongoing outbreak was confrimed in May of 2022 with a cluster of cases in United Kingdom on a patient with travel history to Nigeria where the virus is endemic. The disease has since spread to ther countries in the world predominantly Europe. It has since been declared an evolving concern as opposed to a public health emergency of worldwide/international concern.

To counter its rapid spread, early diagnosis and identification is key. However,the confirmatory PCR and other biochemical tests are not easily available,are very costly and not available in sufficient quantities.

To this end there was need to develop a computer-aided tool that will help identify and act as a means of triaging the suspected patients before they are subjected to confirmatory tests. There being limited data on the same, we leveraged the https://www.kaggle.com/datasets/nafin59/monkeypox-skin-lesion-dataset that was created by scrapping the web for images reported and publicly available case reports.

![Image classification workflow](https://user-images.githubusercontent.com/73839280/201317012-355c304c-b99b-42f9-a775-ac8f35ba0a27.png)


# Dataset and Dataset Description
The dataset used here was created withe the primary focus of telling apart monkepox leisons from other cases that might clinically resemble monkeypox i.e the rash and pustules in measles and chicken pox caused by Measles virus and Varicella Zooster Virus respectively resemble monkeypox in ther initial/earlier stages. For purposes of this task the dataset was grouped into two: Monkeypox cases and non-monkeypox cases also called 'others' so that this task is performed as a binary classification task.

The dataset was arranged in 3 distinct folders

This folder had the original images. 228 in number divided as follows: 102 of the Monkeypox class and 126 of the Other/Non-monkeypox class
This folder has augmented images to aid in this task. A number of augmentation techniques were employed.
To reduce bias a fthis folder was created to do a cross-validation; with the original images being split into training test and validation sets in the ratios 70:20:10 all this while maintaining patient independence.
The training and validation sets were the augmented images while the test images were the original ones

A CSV file containing the image metadata was also included.
