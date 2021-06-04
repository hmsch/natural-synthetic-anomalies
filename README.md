# Self-Supervised Out-of-Distribution Detection and Localization with Natural Synthetic Anomalies (NSA)

## Data
The NIH chest X-ray data can be downloaded [here](https://nihcc.app.box.com/v/ChestXray-NIHCC/file/371647823217).
The MVTec AD dataset can be downloaded [here](https://www.mvtec.com/company/research/datasets/mvtec-ad).

## Training
Train chest X-ray or MVTec AD models using the `train_mvtec.py` and `train_chest_xray.py` scripts. E.g.
```
python3 train_chest_xray.py -s Shift-Intensity-M -d '/path/to/cxr/images/' -o '/where/to/save/models/' -l 'list_of_file_names.txt'
```
or 
```
python3 train_mvtec.py -o '/where/to/save/models/' -s Shift-Intensity-923874273 -n zipper
```

## Evaluation
Use `mvtec_evaluation.ipynb` and `chestxray_evaluation.ipynb`.
