# pixels-to-predictions

Fine-tuning SmolVLM-500M for multimodal science multiple-choice reasoning.

---

## Requirements

- A Google account with Drive access (for Colab), or a local Python environment
- The competition dataset with the exact folder structure below

---

## Dataset Setup

### Google Drive (Colab)

Place the dataset folder in your Drive exactly like this:

```
MyDrive/
└── pixels-to-predictions/
    ├── train.csv
    ├── val.csv
    ├── test.csv
    ├── sample_submission.csv
    └── images/
        └── images/
            ├── train/
            ├── val/
            └── test/
```

The notebook mounts Drive and reads from:

```
/content/drive/MyDrive/pixels-to-predictions
```

### Local

Replicate the same structure on your machine:

```
pixels-to-predictions/
├── train.csv
├── val.csv
├── test.csv
├── sample_submission.csv
└── images/
    └── images/
        ├── train/
        ├── val/
        └── test/
```

Then update the root path variable in the notebook to point to your local folder.

---

## How to Run

### Colab

1. Copy the dataset folder into Google Drive with the exact structure above
2. Open the notebook in Colab
3. Run all cells top to bottom

### Local

1. Download the dataset
2. Recreate the folder structure above
3. Update the root path in the notebook
4. Run the notebook or script

---

## Note

The folder structure must match exactly. If the paths are off, image loading will fail. Please find all related project files and weights in google drive: https://drive.google.com/drive/folders/15tq3ca1YRA6y9EzprRRAn5E85UbRSPXt?usp=sharing
