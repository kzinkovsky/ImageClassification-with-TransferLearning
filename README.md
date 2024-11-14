#Welcome to the image classification project using transfer learning

Once, my daughter and I decided to test how much easier it would be to implement the code we needed in TensorFlow compared to PyTorch 😊
We tried to maintain equal conditions for the project task in both frameworks, but it turned out to be not so simple. The pre-trained models we used, VGG16 and ResNet152, differ in PyTorch and TensorFlow in terms of input image sizes, pixel value ranges, and even the order of the channels. Relevant information has been provided in the notebooks along with comments.

The code in TensorFlow is shorter, and the dataset generators are very convenient, but to match PyTorch’s results, we had to make additions to the model's head and change the training parameters. PyTorch offers more flexibility and is more complex in code, but it has a useful feature like torchvision.utils.make_grid, for which we couldn't find a concise equivalent in TensorFlow, so we used it in both frameworks.

We’d appreciate any advice, but please, no throwing tomatoes at us 😊

