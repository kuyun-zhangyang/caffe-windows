Forked from https://www.github.com/BVLC/caffe master branch in 2015/6/5

Added [Batch Normalization](http://arxiv.org/abs/1502.03167), [Parametric ReLU](http://arxiv.org/abs/1502.01852), Locally Connected Layer, Normalize Layer, [Randomized ReLU](http://arxiv.org/abs/1505.00853).

Setup step:
======
1. Download third-party libraries from http://pan.baidu.com/s/1sjE5ER7 , and put the 3rdparty folder under the root of caffe-windows. If your VS version is not 2012, please refer to [this project](https://github.com/willyd/caffe-windows-dependencies) to create 3rdparty libraries.

2. Run ./src/caffe/proto/extract_proto.bat to create caffe.pb.h, caffe.pb.cc and caffe_pb2.py.

3. Double click ./build/MSVC/MainBuilder.sln to open the solution in Visual Studio 2012. Higher version of VS can also work, but you must create your own 3rdparty libraries.

4. Change the compile mode to Release and X64.

5. Change the CUDA include and library path to your own ones.

6. Compile.

TIPS: If you have MKL library, please add the preprocess macro "USE_MKL" defined in the setting of the project.

中文安装说明：http://blog.csdn.net/happynear/article/details/45372231

Matlab Wrapper
======
Just change the Matlab include and library path defined in the settings and compile.
Don't forget to add ./matlab to your Matlab path.

Python Wrapper
======
Similar with Matlab, just change the python include and library path defined in the settings and compile.

MNIST example
======
Please download the mnist leveldb database from http://pan.baidu.com/s/1mgl9ndu and extract it to ./examples/mnist. Then double click ./run_mnist.bat to run the MNIST demo.

Acknowlegement
======
We greatly thank [Yangqing Jia](https://github.com/Yangqing) and [BVLC group](https://www.github.com/BVLC/caffe) for developing Caffe,

[@niuzhiheng](https://github.com/niuzhiheng) for his contribution on the first generation of caffe-windows,

[@ChenglongChen](https://github.com/ChenglongChen/batch_normalization) for his implementation of Batch Normalization,

[@jackculpepper](https://github.com/jackculpepper/caffe) for his implementation of locally-connected layer,

and all people who have contributed to the caffe user group.
