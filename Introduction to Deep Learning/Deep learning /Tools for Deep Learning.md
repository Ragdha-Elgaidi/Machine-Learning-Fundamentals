# Tools for Deep Learning
## Deep Learning Lifecycle:

- We begin with a problem statement, then move to development (where code gets written). Next, we begin training, where our model learns our data. After training, we deploy, which is when our model goes out into the world for use. A lot of other people do front-end work at this stage. Then we go to monitoring. For our purposes, we'll focus on the development and training of models.
## Deep Learning Tools

### Development tools
   - Integrated Development Environment
        - Code Editor
       -  Interpreter/Compiler
  -   Jupyter Notebooks
       -  Note: Each cell is executed on its own, and it works well for environments to prototype or present code. However, there are limitations:
         -   Editing can make you lose state
          - Code deployed production should be in .py rather than notebooks

### Deep Learning Frameworks
  - PyTorch (aka Torch)
-  TensorFlow/Keras
  -   JAX

## Training Tools
- Experiment management like TensorBoard or Weights and Biases
    - Observe accuracy and loss at training time
- Model versioning like DVC, Neptune, and Pachyderm
   - Remedy issues within the model across different versions of the model
   - DVC is very similar to Git
