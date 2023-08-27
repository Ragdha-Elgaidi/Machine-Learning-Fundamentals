# PreProcessing Data with PyTorch
## Data Representation
- Rarely can we use "out of the box" input. We need our input to be tensors, but often our raw data consists of images, text, or tabular data, and we can't easily input those directly into our model.
   - For image data, we need the data to be turned into tensors with entries of the tensors as bit values in color channels (usually red, green, and blue).
   - Text data needs to be tokenized, meaning, individual words or groups of letters need to be mapped to a token value.
   - For tabular data, we have categorical values (high, medium, low, colors, demographic information, etc...) that we need to transform into numbers for processing.

### One-Hot Encoding
- Categorical values can become numbers. For instance, if you have three colors, Red, Blue, and Yellow, you can assign binary values representing if the color is present or not. The model can then easily compute how far two points are from each other, rather than simply assigning arbitrary values (like 1, 2, and 3 to the colors).
- Note: One-Hot Encoding adds columns, which increases the dimensions of our tensors. If you have a lot of categorical features, this makes it even more complicated.

![screen-shot-2022-06-27-at-11 16 07-am](https://github.com/Ragdha-Elgaidi/Machine-Learning-Fundamentals/assets/76912120/d2c7449c-a927-4bb2-8f75-d271ff0b773b)

### Transforming Data for Neural Networks

- Often, we are faced with data that is not in a format conducive to use in neural networks in its raw form. Preprocessing is the act of turning data from that raw form into tensors that can be used as input to a neural network. This includes:
    - Encoding non-numerical features
    - Converting images to tensors of bit values in color channels
    - Tokenizing words

