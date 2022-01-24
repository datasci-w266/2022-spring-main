# Walkthrough Notebooks: BERT as a black box

The purpose of these notebooks is to show the use of BERT through some abstract APIs, in this case [HuggingFace Transformer Library](https://huggingface.co/transformers/), without getting in to what exactly is happening inside the model.  The goal is to be able to begin experimenting with that API and some models.

There are three notebooks each demonstarting a different API. These notebooks will work better with a GPU.  You can either create a new instance with a GPU or you can access these notebooks using Colab.  To use Colab, copy the notebook into your GoogleDrive and start the notebook from there.  To enable a GPU in your colab instance, start the colab notebook.  Then in the Edit menu go to Notebook Settings and select GPU as the hardware accelerator.

Note: GPUs are a shared resource.  The assumption is you will only use that shared resource when necessary.  When you are done using the GPU, terminate the session.  Do not use the GPU to run models that don't require a GPU e.g. a simple single dense layer.  Also note that you cannot run these notebooks for more than 12 hours at a time. If you hit the 12 hour mark your session will be terminated regardless of what you are doing at the time.  Therefore, be sure to close your sessions if you are not actively running some cells in the notebook.

* [Pipelines](HuggingFaceThreeWays_1_Pipelines.ipynb), the highest level most abstract API lets you run some simple experiments without access to many hyperparameters.
* [HuggingFace Trainer with PyTorch](HuggingFaceThreeWays_2_Trainer.ipynb), a lower level notebook that uses the trainer abstraction to train a model.  This notebook uses PyTorch (an alternative to TensorFlow) which is the default in HuggingFace.
* [HuggingFace TensorFlow ports with Keras](HuggingFaceThreeWays_3_Keras.ipynb), shows the HuggingFace port to TensorFlow.  Many of the HuggingFace models are ported even though they start life in PyTorch.

