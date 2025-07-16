# Machine Learning-Enhanced Near-Infrared Property Prediction for Improved Polyolefin Differentiation 

This repository is in support of a submitted manuscript: 
Shuaijun Li, Robert J.S. Ivancic, Bradley P. Sutliff, Derek Huang, Enrique Blázquez-Blázquez, Tyler B. Martin, Kalman B. Migler, Debra J. Audus*, Sara V. Orski*, "Machine learning-enhanced near-infrared property prediction for improved polyolefin differentiation"

This paper employs machine learning to predict key physical properties of polyolefins from NIR spectra, including density, crystallinity, and short chain branching. By integrating rapid NIR measurement with property prediction, we propose a property-based sorting methodology for polyolefins, addressing the current challenges recyclers face in differentiating polyolefin subclasses. This approach also enhances our understanding in spectra-property relationships. Our work represents a significant advancement toward enhancing sorting efficiency and promoting circularity in plastic recycling.

The repository is intended for the following use cases:

- Illustrate key results from the manuscript including machine learning property prediction, interpretability and figures.
- Allow for full reproducibility of the manuscript.

## Repository contents

The repository contains three folders:
-	Code: Four Jupyter notebooks, which are described in detail below.
-	Data: All of the NIR and property measurement data needed to train and test the models
-	ModelData: Three folders correspond to density, crystallinity, and short chain branching results for interpretability analysis. This information is generated from notebook and used in notebook.

The Code folder includes four Jupyter notebooks:
-	Property_Prediction.ipynb: Performs model training, computes the test root mean squared error and generates Figure 2 and Figure S2.
-	RMSE_Parity_Plot.ipynb: Reproduces the model prediction RMSE Figure 2 as well as PLSR prediction parity plot Figure 3.
-	Interpretability.ipynb: Reads the exported PLSR model information and performs an interpretability analysis including Figures 4, 5, and 6.

## Running the notebooks

Simply navigate to the notebook of interest and then click the `Open in Colab` badge to run in Google Colab [Google Colab](https://colab.research.google.com/). 
The notebooks are setup to walk the user through each of the preprocessing and analyzing steps, generating corresponding figures along the way. All code is written in Python and requires Python == 3.10. It can be used on any operating system. 

Alternatively, the code can be run locally by cloning the repository and using a conda [conda](https://www.anaconda.com) environment or a python virtual environment. Environment files are provided for both.

## Contact

Debra Audus, PhD  
Polymers and Complex Fluids Group
Materials Science and Engineering Division  
Material Measurement Laboratory  
National Institute of Standards and Technology  

Email: Debra.Audus@nist.gov  
GitHubID: @debraaudus  
Staff website: <https://www.nist.gov/people/debra-audus>  

# How to cite
Please cite our submitted manuscript once published:
Shuaijun Li, Robert J.S. Ivancic, Bradley P. Sutliff, Derek Huang, Enrique Blázquez-Blázquez, Tyler B. Martin, Kalman B. Migler, Debra J. Audus*, Sara V. Orski*, "Machine learning-enhanced near-infrared property prediction for improved polyolefin differentiation."

Additionally, please cite:
Shuaijun Li, Sara V. Orski, Debra J. Audus, Data in support of “Machine learning-enhanced near-infrared property prediction for improved polyolefin differentiation”, National Institute of Standards and Technology, https://datapub.nist.gov/od/id/mds2-3809

## Future updates and maintenance

There is no intent to update/maintain this repository once it is released to
the public, given that it is intended to reproduce published figures and
analysis that should not change over time.
