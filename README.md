
# NTUT 4K Drone Photo Dataset Preprocessing

This repository hosts Python scripts for converting the "NTUT 4K Drone Photo Dataset for Human Detection" into YOLOv5-compatible format. The aim is to prepare high-resolution drone imagery from the dataset for use in YOLOv5 models, facilitating machine learning tasks related to human detection.

## Dataset

Download the dataset directly from [Kaggle](https://www.kaggle.com/datasets/kuantinglai/ntut-4k-drone-photo-dataset-for-human-detection/data). Additional information about the dataset can be accessed on its [official website](https://datasetninja.com/ntut-4k-drone-photo).

## Installation

Ensure Python is installed on your system. Clone this repository to get started:

```bash
git clone https://github.com/amitpydev/NTUT-Preprocessing.git
cd NTUT-Preprocessing
```

No external `requirements.txt` is necessary as the script handles dependency checks and installations.

## Usage

Ensure that the downloaded `archive.zip` file from Kaggle is either in the same directory as the script or specify its path using the `--zip_path` argument.

### Running the Script

To process the dataset and prepare it for YOLOv5, execute the following command, specifying the path to the ZIP file if it is not in the same directory:

```bash
python main.py --zip_path="archive.zip" --yolov5_data_path="path_to_yolov5_output_directory"
```

This will convert the dataset annotations to YOLOv5 format and save them to the specified directory.

### Optional Arguments

- `--use_recognizable`: This flag can be included to categorize all tracking labels (e.g., ID_***) as 'Recognizable' within the YOLOv5 annotations.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

- GitHub Repository: [NTUT-Preprocessing](https://github.com/amitpydev/NTUT-Preprocessing)
- For more details or queries, feel free to contact me through my [GitHub Profile](https://github.com/amitpydev).
