# Welcome to the image classification project using transfer learning!

One day, my daughter and I decided to test how much easier it would be to implement our code for the task (as mentioned in the title) using TensorFlow compared to PyTorch 😊. We aimed to keep the project conditions as consistent as possible across both frameworks, but it turned out to be not so simple. The pre-trained models we used, VGG16 and ResNet152, have differences in PyTorch and TensorFlow, including variations in input image sizes, pixel value ranges, and even the channel order. Relevant information has been provided in the notebooks, along with comments.

The code in TensorFlow is shorter, and the dataset generators are quite convenient. However, to match PyTorch’s results, we had to modify the model's head and adjust the training parameters. PyTorch, on the other hand, offers more flexibility and is more complex to code, yet it includes a useful feature, torchvision.utils.make_grid, for which we couldn't find a concise equivalent in TensorFlow—so we ended up using it in both frameworks.

A few words about transfer learning strategies: Transfer learning with pretrained models is a brilliant concept, and much credit goes to its pioneers. With a relatively small number of labeled images, it enables impressive classification accuracy. However, choosing the right training strategy (such as deciding how many pretrained layers to freeze) doesn’t follow any universal rules and often requires trial and error. Both the models and the frameworks have unique characteristics that influenced our choices.

We’d appreciate any advice, but please, no tomato-throwing 😊.
