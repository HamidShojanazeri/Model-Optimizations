# Model-Optimizations


## Torch-TensorRT

Making use of TensorRT optimization on Torchscripted modules, this has been moved under PyTroch repo and relatively easier to use.

In this PyTorch integration with TensorRT, there would be no need to convert the model to ONNX before conversion to TensorRT.

The resulted model should feel similar to Torchscripted model in temrs of saving and loading and passing the inputs. 

Old : PyTorch Model --> ONNX --> TensorRT
Now : Pytorch Model --> TensorRT
