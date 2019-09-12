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
path通す
```
export PATH=/usr/local/cuda/bin:$PATH
export CPATH=/usr/local/cuda/include:$CPATH
```
CUDAある場合
```
export LD_LIBRARY_PATH=/usr/local/cuda/lib64:$LD_LIBRARY_PATH
export DYLD_LIBRARY_PATH=/usr/local/cuda/lib:$DYLD_LIBRARY_PATH
```

必要なパッケージのインストール
```
pip install --verbose --no-cache-dir torch-scatter
pip install --verbose --no-cache-dir torch-sparse
pip install --verbose --no-cache-dir torch-cluster
pip install --verbose --no-cache-dir torch-spline-conv
pip install torch-geometric
```
