# Model-Optimizations


## Torch-TensorRT

Making use of TensorRT optimization on Torchscripted modules, this has been moved under PyTroch repo and relatively easier to use.

In this PyTorch integration with TensorRT, there would be no need to convert the model to ONNX before conversion to TensorRT.

The resulted model should feel similar to Torchscripted model in temrs of saving and loading and passing the inputs. 

Old : PyTorch Model --> ONNX --> TensorRT
Now : Pytorch Model --> TensorRT

#### Steps

Pull the NGC docker container, starting with 21.11 version, pytorch:21.11-py3

```
docker run --gpus all -it --rm -v local_dir:container_dir nvcr.io/nvidia/pytorch:xx.xx-py3

```

Run the trt_test.py, this will benchmark resnet50 with eager mode and TensorRT of FP32 and FP16 versions. 

```
python trt_test.py

```
