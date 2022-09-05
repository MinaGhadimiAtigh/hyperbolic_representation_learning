.. notebook_test documentation master file, created by
   sphinx-quickstart on Sat Jul 25 11:56:56 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to the Hyperbolic Representation Learning for Computer Vision tutorial, ECCV2022!
=======================================================

| *Tutorial website*: https://sites.google.com/view/hyperbolic-tutorial-eccv22
| *Tutorial edition*: October, 2022
| *Repository*: To be updated
| *Author*: Mina Ghadimi Atigh


This website provides you access to the content that we will use for the tutorial session at the ECCV 2022,
"Hyperbolic Representation Learning for Computer Vision".

Learning in computer vision is all about deep networks and such networks operate on Euclidean manifolds by design.
But is Euclidean geometry the best choice for deep learning or simply a practical option?
Recent literature in machine learning and computer vision has shown that hyperbolic geometry provides a strong alternative,
with an improved ability to embed hierarchies, graphs, text, images, and videos.

In light of recent advancements in hyperbolic representation learning for computer vision, this tutorial seeks to advocate
hyperbolic geometry and its strong potential for computer vision to a broader audience. The tutorials provides a theoretical
and practical starting point for the field. At the conference, we will provide an easy-going introduction to hyperbolic
geometry for non-mathematicians, where we focus on intuition and high-level understanding. We then outline the current
state of hyperbolic geometry for vision from supervised and unsupervised perspectives. At the end, we dive into open
research problems and future potential for hyperbolic geometry and visual understanding.

Unique for this tutorial is that we do not stop at a theoretical foundation. The tutorial website will also host a
series of notebook-style code snippets with foundational works on hyperbolic geometry, to get a better understanding of
its workings and lower the barrier to start your dive into this exciting new research direction in computer vision.

For any remaining questions regarding the notebooks, please contact us at m.ghadimiatigh@uva.nl.

Schedule
--------

+------------------------------------------+---------------------------------------------------+
| **Date**                                 | **Practical**                                     |
+------------------------------------------+---------------------------------------------------+
| Monday, 9. May 2022                      | Practical 1: Multi-Layer Perceptrons              |
|                                          |                                                   |
| Tuesday, 10. May 2022                    | Practical 2: Convolutional Neural Networks        |
|                                          |                                                   |
|                                          | Practical 3: Vision Transformers                  |
+------------------------------------------+---------------------------------------------------+
| Wednesday, 11. May 2022                  | Practical 4: Regular Group Convolutions           |
+------------------------------------------+---------------------------------------------------+
| Thursday, 12. May 2022                   | Practical 5: Self-Supervised Contrastive Learning |
+------------------------------------------+---------------------------------------------------+

How to run the notebooks
------------------------

On this website, you will find the notebooks exported into a HTML format so that you can read them from whatever device you prefer.
Your task is to fill in the notebooks to solve the practicals.
There are three main ways of running the notebooks we recommend:

- **Locally on GPU**: If you have a laptop with a build-in NVIDIA GPU, we recommend that you run the notebooks on your own machine. All notebooks are stored on the github repository that also builds this website. You can find them here: to be updated.All notebooks require access to a GPU to keep the training times in a reasonable range. Nonetheless, if you prefer, you can code and test most of your code on a CPU-only system, i.e. your own laptop, and once your code is tested and ready, use one of the remaining options to train the model. To ensure that you have all the right python packages installed, we provide a conda environment in the `same repository <https://github.com/phlippe/asci_cbl_practicals>`_.

- **Google Colab**: If you do not have access to a GPU on your local machine, you can make use of `Google Colab <https://colab.research.google.com/notebooks/intro.ipynb#recent=true>`_. Google Colab provides you access to GPUs for free, and you can activate the GPU support by :code:`Runtime -> Change runtime type -> Hardware accelerator: GPU`. Each notebook on this documentation website has a badge with a link to directly open it on Google Colab. It is highly recommend to copy the notebook to your own Google Drive before starting, since when closing the session, changes might be lost if you don't save it to your local computer or have copied the notebook to your Google Drive beforehand. In addition, note that for free account, Google Colab is limited to one session at a time, and each session has a time limit.

- **Compute cluster**: If you have access to a compute cluster, we recommend to using it to do your final trainings. Depending on your preference, you can implement the practicals either locally or on Google Colab. Once your notebook is ready, you can first convert the notebooks to a script using :code:`jupyter nbconvert --to script ...ipynb`, and then start a job on the cluster for running the script. A few advices when running on clusters:

   - Disable the tqdm statements in the notebook. Otherwise your slurm output file might overflow and be several MB large.
   - Comment out the matplotlib plotting statements, or change :code:`plt.show()` to :code:`plt.savefig(...)`.


.. toctree::
   :caption: Tutorials
   :maxdepth: 2

   notebooks/Introduction_to_PyTorch.ipynb
   notebooks/2_Hyperbolic_Image_Embeddings.ipynb