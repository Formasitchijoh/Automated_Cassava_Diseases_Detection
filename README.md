# A Computer Vision Approach for Automated Identification of Cassava Diseases

Undergraduate project, University of Buea (B.Eng. Computer Engineering). Updated 2026.

This project uses computer vision and deep learning to identify cassava diseases from leaf images. The goal is to support early detection so farmers can act before disease spreads and yields are lost.

<img width="908" alt="Cassava disease detection overview" src="https://github.com/user-attachments/assets/3e6e7603-8331-4d7a-8fb1-426ccb104454">

## Why This Matters

Cassava is a staple food crop across Africa and a major source of income for smallholder farmers in Cameroon. In 2018, a cassava plague cut yields in my community, Bali-Nyonga, by about 80%. Disease outbreaks like this threaten both food security and family livelihoods, and fast, reliable diagnosis is the first step in managing them.

## What the Model Detects

The model classifies cassava leaf images into the following conditions:

- Cassava Mosaic Disease (CMD)
- Cassava Bacterial Blight (CBB)
- Cassava Brown Streak Disease (CBSD)

## Dataset

The model was trained on a labeled cassava leaf disease image dataset containing healthy and diseased leaves.

| Attribute | Description |
|---|---|
| `image_id` | Image file name |
| `label` | Numeric code for the disease |
| `label_num_to_disease_map.json` | Mapping between each disease code and its name |

<img width="1023" alt="Dataset sample" src="https://github.com/user-attachments/assets/c8c52873-60c0-441c-97c5-fabfad1c6142">
<img width="996" alt="Label distribution" src="https://github.com/user-attachments/assets/ae820d13-6a0d-492c-86a0-442ef9b45cdc">

## Approach

1. Loaded and explored the labeled images and the disease label mapping.
2. Split the data into training and validation sets and prepared the images for the model.
3. Fine-tuned a pretrained ResNet-152 convolutional neural network in PyTorch.
4. Evaluated the model on the validation set.

**Environment:** Kaggle
**Libraries:** PyTorch, pandas, NumPy, scikit-learn, Matplotlib, seaborn

## Results

| Metric | Value |
|---|---|
| Model | ResNet-152 (transfer learning) |
| Accuracy | 89% |

## What I Learned

During a field test at the University of Buea farm, a student asked: "After it detects the disease, what next?" That question showed the limit of this project. Detection comes after the damage is done. Farmers need crop varieties that resist disease under their pest and climate conditions. This led me toward predictive modeling that combines crop genetics, climate, and pest data to identify resistant varieties, which is the focus of my further studies in data science.

## Repository Contents

| File | Description |
|---|---|
| `Cassava Leaf Disease Detection - Pytorch Tutorial.ipynb` | Data exploration, training, and evaluation notebook |

## How to Run

1. Open the notebook on Kaggle or in Jupyter with a GPU runtime.
2. Attach the cassava leaf disease dataset.
3. Run the cells in order.
