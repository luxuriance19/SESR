# SESR
SESR: Single Image Super Resolution with Recursive Squeeze and Excitation Networks (Submitted to ICPR 2018)
---
![](https://github.com/opteroncx/SESR/raw/master/figures/f1.png)  
### Quality for scale x4
    Trained on yang91+bsd200, the default recursion depth for each branch is set to 4
---
| DataSet/Method        | PSNR/SSIM|
| ------------- | -----:|
| Set5      | 31.84/ 0.891      |
| Set14     | 28.32/ 0.784      | 
| BSD100    | 27.42/ 0.737      | 
| Urban100    | 25.42/ 0.771      | 
---
    Trained on div2k, r=4
---
| DataSet/Method        | PSNR/SSIM|
| ------------- | -----:|
| Set5      | 32.01/ 0.893      |
| Set14     | 28.41/ 0.786      | 
| BSD100    | 27.45/ 0.739      | 
| Urban100    | 25.72/ 0.781      | 
### Compare with other methods
![](https://github.com/opteroncx/SESR/raw/master/figures/f2.png)  
### Requirement
    Python 2.7
    Pytorch 0.2.0
    opencv-python
    numpy
### Train
    python train.py --cuda
### Evaluate
    python test.py --cuda
### Do Super resolution on your own images
    python test.py --cuda --mode sr --testdir path_to_your_image
