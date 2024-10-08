- # Alzheimer's Disease Detection

- ## `dataset link` : https://www.kaggle.com/datasets/tourist55/alzheimers-dataset-4-class-of-images/code?datasetId=457093&sortBy=voteCount

## Steps to Load the Dataset in Google Colab

   ```bash
    !pip install opendatasets --upgrade
    import opendatasets as od
    dataset_url = 'https://www.kaggle.com/datasets/tourist55/alzheimers-dataset-4-class-of-images'
    od.download(dataset_url)
   ```
Go to your Kaggle account settings and click on `Create New API Token`. This will download a kaggle.json file. You can open the json file and see your API key.

- `MildDemented` : Individuals in this category show no signs of dementia. This is the control group used for comparison. **Not severe**.
- `ModerateDemented` : This stage corresponds to what is often referred to as early-stage dementia or mild cognitive impairment (MCI).**Mild**, but starting to impact daily functioning.
- `NonDemented` : At this stage, dementia is becoming more noticeable, and individuals may start requiring some assistance in their daily lives. **Moderate** (but still in the earlier stages of dementia).
- `VeryMildDemented` : This stage is more advanced than the previous stages. Individuals experience significant memory loss, confusion, and reduced ability to function independently. It corresponds to mid-stage Alzheimer’s. **Severe** (often requires full-time care and supervision).

Initial train data Count:
- `MildDemented` : 717
- `ModerateDemented` : 52
- `NonDemented` : 2560
- `VeryMildDemented` : 1792

Initial Test data Count:
- `MildDemented` : 179
- `ModerateDemented` : 12
- `NonDemented` : 640
- `VeryMildDemented` : 448