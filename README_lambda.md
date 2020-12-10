# Install

```
git clone --recursive https://github.com/chuanli11/Zooming-Slow-Mo-CVPR-2020.git

virtualenv -p /usr/bin/python3.6 venv
. venv/bin/activate

pip install numpy opencv-python lmdb pyyaml pickle5 matplotlib seaborn

pip install torch==1.5.1
pip install torchvision==0.6.1

# Need to do the change here:
# https://github.com/CharlesShang/DCNv2/pull/58/files/9f4254babcd162a809d165fa2430a780d14761f4#diff-c49b9111a7857be19e44bbe3aacb89427c0d19009e1c27fbcbe51df9813c2d8a
cd codes/models/modules/DCNv2
bash make.sh
```

# Run

Set `test_dataset_folder` in `test.py` accordingly.


```
python test.py
```