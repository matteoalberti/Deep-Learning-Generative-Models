# Deep generative models with TensorFlow 2

## Outline of the course

* [**Day 1: Overview of TF2**](day1/slides.ipynb)
    - Libraries and frameworks for Deep Learning
    - Build a model with tf.keras (the easy way)
    - Customise models, metrics and training loops
    - Visualise statistics with TensorBoard
    - DL programming paradigms: Symbolic vs. Imperative Programs
    - Backpropagation and AutoDiff


* [**Day 2: Improve performances**](day2/slides.ipynb)
    - TF execution modes
    - GPUs support
    - Improve performances with input data pipelines
    - Parallel execution across multiple devices
    - Distribution strategies


* [**Day 3: Hands-on generative deep learning**]()
    - Generative models
    - Autoencoders
    - Variatonal Autoencoders
    - Generative Adversarial Networks


## Install TensorFlow

Tensorflow and all the requirements for the notebooks can be easily installed using `conda` or `pip`:

- `pip` (make sure `python3` is installed)
```
python3 -m venv ~/envs/tf2
source ~/envs/tf2/bin/activate
pip install tensorflow==2.2.0
pip install tensorboard scikit-learn matplotlib jupyter pydot graphviz
```

- `conda` (usually the latest TensorFlow versions are not immediately available).
```
conda create -n tf2 python=3.7
conda activate tf2
conda install tensorflow
conda install tensorboard sklearn matplotlib jupyter pydot graphviz
```

## Instructions to access the cluster

To launch the interactive apps via the Open OnDemand portal follow the link:

[```https://login-web.hpc.cam.ac.uk/```](https://login-web.hpc.cam.ac.uk/)

If needed, you can access a login node via ssh:

```
ssh <username>@login-gpu.hpc.cam.ac.uk
```

### Obtain the credentials

1. **Make sure to have correctly installed Google Authenticator** (or any other OTP 
authentication app).

2. I will give each one of you an unique link via private message. To reveal the password
 use the passphrase given during the course. **The password is revealed only once!** Store
 it somewhere safe.

3. Login to the [OOD portal](https://login-web.hpc.cam.ac.uk/) using username / password.

4. Scan the QR code using Google Authenticator to pair your device as second factor
authenticator.

5. Insert the one time password provided by the authentication app.

### Launch an Interactive Session

From the Dashboard select the "Interactive Apps" tab, then "Jupyter Notebook" or 
"TensorBoard". Fill the fields as follows:

| Fields | Jupyter Notebook | TensorBoard |
|-----|-----|-----|
|Project Account| training-gpu | training-cpu |
| Partition | pascal | skylake |
| Reservation * | dltraining_day1 | |
| Number of hours ** | <=12 | |
| Number of ... | <=4 | 1 |

To launch TensorBoard on a specific folder fill the Logdir field accordingly. 

\* `dltraining_day1` for Tuesday, `dltraining_day2` for Wednesday, `dltraining_day3` for Thursday.

\** Remember that the reservation is from 10am - 10pm CEST


## Suggested readings

- Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow - 2nd Edition, 2019, O'Reilly, ISBN: 9781492032649
- TensorFlow official guide (https://www.tensorflow.org/guide)[https://www.tensorflow.org/guide]
- TensorFlow official documentation (https://www.tensorflow.org/api_docs)[https://www.tensorflow.org/api_docs]
- Keras official guides and docs (https://keras.io/)[https://keras.io/]


## Contacts

Piero Coronica - pc620@cam.ac.uk\
RSE @ Research Computing Services - University of Cambridge
