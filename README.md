# Welcome to the image classification project using transfer learning

Once, my daughter and I decided to test how much easier it would be to implement the code we needed for the task as posted in the headline in TensorFlow compared to PyTorch 😊
We tried to maintain equal conditions for the project task in both frameworks, but it turned out to be not so simple. The pre-trained models we used, VGG16 and ResNet152, differ in PyTorch and TensorFlow in terms of input image sizes, pixel value ranges, and even the order of the channels. Relevant information has been provided in the notebooks along with comments.

The code in TensorFlow is shorter, and the dataset generators are very convenient, but to match PyTorch’s results, we had to make additions to the model's head and change the training parameters. PyTorch offers more flexibility and is more complex in code, but it has a useful feature like torchvision.utils.make_grid, for which we couldn't find a concise equivalent in TensorFlow, so we used it in both frameworks.

A few words about transfer learning strategies. Transfer learning with pretrained models is a brilliant idea, and great credit goes to its pioneers. With a relatively small number of labeled images, it enables achieving quite impressive classification accuracy. However, choosing the right training strategy (such as deciding how many pretrained layers to freeze) does not follow any universal rules and often required trial and error. Specific characteristics were evident both in the models and the frameworks used.

We’d appreciate any advice, but please, no throwing tomatoes at us 😊

