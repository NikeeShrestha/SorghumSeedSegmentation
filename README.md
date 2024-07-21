# Sorghum Seed Segmentation using a previously published **pre-trained model**.

- Toda, Yosuke, Fumio Okura, Jun Ito, Satoshi Okada, Toshinori Kinoshita, Hiroyuki Tsuji, and Daisuke Saisho. "Training instance segmentation neural network with synthetic datasets for crop seed phenotyping." Communications biology 3, no. 1 (2020): 173.

## The main directory has three sub directories and compressed folder **Cropped_Scanned_Preprocessed.zip**:

- **Scripts**: This directory has two jupyter notebook scripts.
    -  **SorghumSeedInference.ipynb**: This notebook shows a demo about segmenting seed images and extracting data related to seed shape and color. The notebook has all the information regarding the files required to run this notebook.
    -  **ManualAnnotation.ipynb**: This notebook shows how to get the ground truth data related to seed shape and color from ten manually segmented images. The notebook has information regarding the files required to run the script.

- **Manual Annotation**: This directory has two sub directories. 
    - **Images**: Ten images with manual annotation performed at the online annotation tool; makesense.ai.
    - **JsonFiles**: Two metadata json files with annotation which includes mask and bounding box information for seeds within each scan. Metadata_1.json file has annotation information of five images (1101.jpg, 1102.jpg, 1103.jpg, 1107.jpg and 1109.jpg). Metadata_2.json file has annotation information of five images (4305.jpg, 4567.jpg, 4762.jpg, 4898.jpg and 5021.jpg). 
    
- **inference**: This directory has two sub-directories.
    - **rawimages**: This directory has three example images which is incorporated to be procssed in the **SorghumSeedInference.ipynb** script for preprocessing and extracting seed color phenotypes analysed in the study.
    - **processedimages**: This directroy will save the procssed images after images from **rawimages** runs through **SorghumSeedInference.ipynb**.

- **Cropped_Scanned_Preprocessed.zip** is a compressed folder that consists of 1664 pre-processed sorghum seed scans from experimental plots in the year of 2021. These images can be run through **SorghumSeedInference.ipynb** to extract seed shape and color phenotypes. 
