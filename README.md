# DATAGATE

Data Gate by Ouchhh New Media Agency, proposes an aesthetic approach to Artificial Intelligence powered exploration of the Kepler Data.

The data of Kepler mission is a very large spreadsheet comprised of information dedicated to the detected exoplanets. Each table in these spreadsheets contains around a hundred columns. Each of these columns represent an aspect, a feature of these planets.

In addition to these spreadsheets, the publicly available data includes the raw light curve readings, which were used in the detection of the aforementioned planets. This data doesn’t readily make these planets detectable, but various AI methods have been used to analyze and extract planetary data from these light curves.
Due to its complexity and size, it is impossible to visualize these as is. So we propose an AI based approach to interpret and aestheticize this information. Our aim is to analyze this data through AI, strictly for an alternative, visual representation of this data. This project does not and cannot propose to detect new planets, which has been excellently done and publicly made available.

## ORIGINAL WALKTHROUGH

You can jump straight to the [AstroNet walkthrough](exoplanet-ml/astronet/README.md#walkthrough).

Otherwise, click through to the desired directory as outlined below.

## Original Directories

[astronet/](exoplanet-ml/astronet/)

* A neural network for identifying exoplanets in light curves. Contains code for:
  * Downloading and preprocessing Kepler light curves.
  * Building different types of neural network classification models.
  * Training and evaluating a new model.
  * Using a trained model to generate new predictions.

[astrowavenet/](exoplanet-ml/astrowavenet/)

* A generative model for light curves.

[light_curve/](exoplanet-ml/light_curve)

* Utilities for operating on light curves. These include:
  * Reading Kepler data from `.fits` files.
  * Applying a median filter to smooth and normalize a light curve.
  * Phase folding, splitting, removing periodic events, etc.
* [light_curve/fast_ops/](exoplanet-ml/light_curve/fast_ops) contains optimized
C++ light curve operations.

[tf_util/](exoplanet-ml/tf_util)

* Shared TensorFlow utilities.

[third_party/](exoplanet-ml/third_party/)

* Utilities derived from third party code.


## Additional tools for visualizations and custom pre-proprocessing.

These tools examplify the process we've gone through whilst preparing the data to be visualized in various procedural design software.

Also, we present minor Processing tools for visualizing various data.

# Setup

## Required Packages

* **TensorFlow** ([instructions](https://www.tensorflow.org/install/))
* **Pandas** ([instructions](http://pandas.pydata.org/pandas-docs/stable/install.html))
* **NumPy** ([instructions](https://docs.scipy.org/doc/numpy/user/install.html))
* **SciPy** ([instructions](https://scipy.org/install.html))
* **AstroPy** ([instructions](http://www.astropy.org/))
* **PyDl** ([instructions](https://pypi.python.org/pypi/pydl))
* **Bazel** ([instructions](https://docs.bazel.build/versions/master/install.html))
* **Abseil Python Common Libraries** ([instructions](https://github.com/abseil/abseil-py))

## Original Author

Chris Shallue: [@cshallue](https://github.com/cshallue)

## Creative 

Ouchhh Studio

# Citation

Please refer to the master branch for more information.

# Disclaimer

Ouchhh studio is not affiliated with Google, NASA or Kepler Project.
