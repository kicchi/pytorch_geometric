# pytorch geometric
## インストール手順
pytorchのインストール  
conda経由でインストールする事  
```
conda install pytorch torchvision -c pytorch
```
出たエラー
```
ImportError: numpy.core.multiarray failed to import
```
対処法:Numpyが古いのでアップデート
```
pip install numpy --upgrade
```
