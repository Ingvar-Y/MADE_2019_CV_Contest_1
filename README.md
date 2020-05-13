# MADE_2019_CV_Contest_1

На первом шаге необходимо подготовить уменьшенный датасет при помощи cut_preparation.ipynb

Потом сабмит делается при помощи команд:
```
python hack_train_1_result.py -n predresnet151 -b 256 -d cut_data -e 20 -lr 3e-4 --gpu -nr
python hack_train_1_result.py -n predresnet151 -m predresnet151_best.pth -b 256 -d cut_data -e 10 -lr 3e-4 --gpu -nr
python hack_train_1_result.py -n resnet151 -m predresnet151_best.pth -b 256 -d . -e 5 -lr 3e-4 --gpu
```
![screenshot](https://github.com/Ingvar-Y/MADE_2019_CV_Contest_1/blob/master/screenshot.png)
