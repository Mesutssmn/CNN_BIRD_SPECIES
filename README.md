# CNN_BIRD_SPECIES

## About Dataset
![image](https://github.com/Mesutssmn/CNN_BIRD_SPECIES/assets/127686800/4b8b72e7-895b-4c81-8e8f-3a57eb491e5b)

**Dataset Size and Structure:** The dataset contains 525 bird species with 84,635 training images, 2,625 test images (5 images per species), and 2,625 validation images (5 images per species). Each species has its own subdirectory, making it convenient for use with tools like Keras' flow_from_directory.

**Dataset Files:** Along with the images, there's a CSV file named birds.csv. This file contains information about the images, including their file paths, labels (species names), scientific labels (Latin names), dataset (train, test, or valid), and class IDs.

**Image Properties:** All images are original and not augmented, with dimensions of 224 x 224 x 3 in JPG format. Each image contains only one bird, which occupies at least 50% of the pixels. The images were cropped and resized to ensure they contain sufficient information for classification.

**Data Cleaning:** Duplicate or near-duplicate images were removed to prevent leakage between train, test, and validation sets. Defective or low-information images were also filtered out.

**Training Recommendations:** Due to the dataset's size, using smaller image sizes (e.g., 150 x 150 x 3) is recommended to reduce training time.

**Data Imbalance:** The training set is not balanced, with a varying number of files per species. However, each species has at least 130 training image files. Additionally, there's a significant imbalance between male and female images, with about 80% of images being male and 20% female. This might affect the classifier's performance, especially if test and validation images are predominantly male.
