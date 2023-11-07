# SEAT-OD
This is the code for the paper "SEAT-OD: Semantic-aware Testing for Object Detection Systems".

Document Organization：
```
SEAT-OD/
        README.md
        TestCaseGeneration/
        Metrics/
        PGD_Attack/
```
where TestCaseGeneration/ is the test sample generation module, Metrics/ is the SEAT framework and the pgd attack method is in PGD_Attack/.

## Test Case Generation
We use styleGAN2 as the basis for test case generation. That is, we first train a GAN with the Kitti dataset for feature visualization. 
### 1.0  Install
This implementation is tested with Anaconda Python  3.8(ubuntu18.04), PyTorch  1.8.1 and Cuda  11.1

### 2.0  Generation
Test case generation using styleGAN2, by run
```
    python case.py
```
The results are saved in out/

![Test case generation](https://github.com/dummySeatOD/SEAT-OD/blob/main/Figure/generation.png)
