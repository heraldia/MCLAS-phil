# some incorrect parts
1. models/loss.js  -> should be loss.py,  correct?

# suggestion
1. Directly send me testConfig.ipynb, as I can not log in using his google username and credential.
2. Do we have a conda env.yaml or requirement.txt script?

# worklog
```
2022_1129_2321
unzip -t MCLAS.zip

unzip MCLAS.zip –d /home/phil/githubProject
unzip MCLAS.zip 
conda env update -f ./env/mclas.yml
conda activate mclas_env

2022_1130_2119 transfer to macpro
用了ubuntu, and mac os.
2022_1130_2232 conda env done

2022_1130_2232 I do not have cuda device. So it shows
[2022-11-30 22:31:46,186 INFO] Device cuda
Traceback (most recent call last):
  File "/Users/y0f00k5/Documents/b/githubProject/MCLAS/src/train.py", line 176, in <module>
    train_abs(args, device_id)
  File "/Users/y0f00k5/Documents/b/githubProject/MCLAS/src/train_abstractive.py", line 318, in train_abs
    train_abs_single(args, device_id)
  File "/Users/y0f00k5/Documents/b/githubProject/MCLAS/src/train_abstractive.py", line 332, in train_abs_single
    torch.cuda.set_device(device_id)
  File "/Users/y0f00k5/Library/miniconda3/envs/mclas_env/lib/python3.10/site-packages/torch/cuda/__init__.py", line 314, in set_device
    torch._C._cuda_setDevice(device)
AttributeError: module 'torch._C' has no attribute '_cuda_setDevice'
```
