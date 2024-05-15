## Enviroment
The code is tested in the docker environment: yuewuust/pytorch1.11.0_nviffrast:v11
Please refer to [Link](https://hub.docker.com/r/yuewuust/pytorch1.11.0_nviffrast/tags).

We use the Pytorch 1.11.0 version.

3090 py3.8 ubuntu20.04 cuda11.3

其他库自己配就是了，版本没多大问题。别用那个docker。

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

## 记录
要生成自己的mat对应的头部姿态和表情参数时将render.sh里面的render.py改为render_mine.py就是了
