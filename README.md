# Brain Tumor Segmentation
Use pip to install all the dependencies
```bash
pip install -r requirements.txt
```
To open the notebook
```bash
jupyter lab
```
To see logs in Tensorboard
```bash
tensorboard --logdir logs --samples_per_plugin images=100
```
To setup the project dataset
```bash
python setup_scripts/download_dataset.py
python setup_scripts/unzip_dataset.py
python setup_scripts/extract_images.py
```

## Usage

```bash
python api.py --file <file_name> --ofp <optional_output_file_path>
python api.py --folder <folder_name> --odp <optional_output_folder_path>
python api.py -h
```

```
Available api.py Flags
--file  : A single image file name.
--ofp   : An optional folder location only where the output image will be stored. Used only with --file tag.

--folder: Path of a folder containing many image files.
--odp   : An optional folder location only where the output images will be stored. Used only with --folder tag.

-h, --help : Shows the help contents.
```
