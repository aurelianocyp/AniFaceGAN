## Enviroment
The code is tested in the docker environment: yuewuust/pytorch1.11.0_nviffrast:v11
Please refer to [Link](https://hub.docker.com/r/yuewuust/pytorch1.11.0_nviffrast/tags).

We use the Pytorch 1.11.0 version.

3090 py3.8 ubuntu20.04 cuda11.3

## Test
The expression coefficients are extracted by [Deep3DFaceRecon](https://github.com/microsoft/Deep3DFaceReconstruction). And we provide the smile expression ./mat/01626.mat as an example. Zero expression is defined as a neutral face. 

Run the 
```
./render.sh
``` 
and the rendered multiview images and videos will be sorted in ./multiview_imgs/.

## To do

- [X] Release inference code
- [X] Release pretrained checkpoints
- [ ] Clean up code.
- [ ] Add detailed instrunctions.


## Citation

Please cite the following paper if this work helps your research:

    @inproceedings{yue2022anifacegan,
    title={AniFaceGAN: Animatable 3D-Aware Face Image Generation for Video Avatars},
    author={Wu, Yue and Deng, Yu and Yang, Jiaolong and Wei, Fangyun and Chen Qifeng and Tong, Xin},
    booktitle={Advances in Neural Information Processing Systems},
    year={2022}
}
