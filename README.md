#pixels

This project is run directly from the notebook.

What you need

You need the dataset folder to be replicated exactly the way the notebook expects.

Google Drive setup

Put the full folder in your Google Drive exactly like this:

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

Then open the notebook in Colab and run it from top to bottom.

The notebook mounts Google Drive and reads from:

/content/drive/MyDrive/pixels-to-predictions

So the folder structure must match exactly.

Local setup

You can also run locally, but you must replicate the same folder exactly on your machine:

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

If running locally, update the root path in the script or notebook so it points to your local pixels-to-predictions folder.

How to run

Colab

1. Upload or copy the dataset folder into Google Drive with the exact structure above.
2. Open the notebook in Colab.
3. Run all cells in order.

Local

1. Download the dataset.
2. Recreate the exact folder structure above.
3. Update the root path in the script or notebook if needed.
4. Run the notebook or Python script.

Important note

The folder structure matters. If the data is not laid out exactly the same way, image loading will fail.
