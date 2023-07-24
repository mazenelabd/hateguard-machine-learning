# HateGuard Machine Learning Layer
This is the first layer of a three-layer product:
1. Machine learning layer or Data science layer, the current repository.
2. [Back-end layer](https://github.com/mazenelabd/hateguard-api).
3. [Front-end layer](https://github.com/mazenelabd/HateGuard/).

To run the product code, you do not have to rebuild the model in the first layer you can skip to [The Second Layer](https://github.com/mazenelabd/hateguard-api).

The second layer, the [API](https://github.com/mazenelabd/hateguard-api), and the third layer, the [front-end](https://github.com/mazenelabd/HateGuard/), should be running simultaneously to have a full functioning demonstration of the product.

- Machine learning / Data Science code
In this repository you can find three Python notebooks ".ipynb" and the dataset file used for the task "labeled_data.csv"
The three ".ipynb" files are:
1. "1-EDA.ipynb": in which we have conducted an exploratory data analysis for the dataset.
2. "2-transformer-fine-tuning.ipynb": in which we have managed to fine-tune the "microsoft/MiniLM" transformer to be able to detect hate speech. The output best model from this code is located at the path "./ML-layer/data/output/best_model"
3. "3-quantization.ipynb": in which we have managed to convert the transformer model, which is a PyTorch model, to an ONNX model which can be easily integrated inside the product. Also, we have managed to quantize the model reducing its size from 127MB to 32.2 MB. The output from this step was two models, the ONNX model and the quantized ONNX model, which can be found at "./ML-layer/onnx"
