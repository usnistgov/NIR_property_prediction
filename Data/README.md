# Background

The data here is in support of a submitted manuscript: Shuaijun Li, Robert J.S. Ivancic, Bradley P. Sutliff, Derek Huang, Enrique Blázquez-Blázquez, Tyler B. Martin, Kalman B. Migler, Debra J. Audus*, Sara V. Orski*, "Machine learning-enhanced near-infrared property prediction for improved polyolefin differentiation."

This paper employs machine learning to predict key physical properties of polyolefins from NIR spectra, including density, crystallinity, and short chain branching. By integrating rapid NIR measurement with property prediction, we propose a property-based sorting methodology for polyolefins, addressing the current challenges recyclers face in differentiating polyolefin subclasses. This approach also enhances our understanding in spectra-property relationships. Our work represents a significant advancement toward enhancing sorting efficiency and promoting circularity in plastic recycling.

Data is provided to support the validation of the results and to facilitate prototyping of the methodologies presented in the manuscript. A corresponding code repository is accessible at https://github.com/usnistgov/nir_property_prediction, which includes Jupyter notebooks that demonstrate the machine learning training and testing approach discussed in the manuscript, along with scripts for reproducing the figures presented in the manuscript. This resource promotes transparency, reusability, and further development and adaptation of the presented work.

# Data Description

## Sample Information
The `SampleInformation.csv` file provides the original resin code from the manufacturer (where appropriate), the source, the sample code used to identify materials in this work, the major and minor polyolefin class as reported by the source, the physical form/shape of the sample, and additional notes such as BigSMILES, alternative names, reference links, etc.

## NIR
The NIR folder contains NIR spectroscopy data. Background has been automatically subtracted by the instrument when the spectra were taken. The data files are named as `<SampleCode>_<Replicate>.csv`, where each sample was measured six times, with the sample being shaken between each replicate. The measurements cover the wavenumber range from `4000 cm-1` to `12000 cm-1`. The first column is the wavenumber in `cm-1` and the second column is the intensity value in percent reflectance.

## Property Measurements
The `PropertyMeasurements.csv` file provides the measured values for density, crystallinity, and short chain branching. These property measurements were used for training and testing machine learning models. Density was calculated using Archimedes principal; crystallinity was determined using the enthalpy of melting from differential scanning calorimetry. A `10 °C/min` temperature ramp was used, and values were extracted from heating. Heat of fusion $\Delta H_m^0$ was taken as `293.6 J/g` and `207.1 J/g` for PE and PP samples, respectively. Short chain branching was taken from an IR detector on a high-temperature size exclusion chromatography instrument. For all these three properties, averaged measurement values are provided.

More details on how these measurements were obtained can be found in the corresponding submitted paper.

## Contact

Sara V. Orski, PhD  
Polymers and Complex Fluids Group
Materials Science and Engineering Division  
Material Measurement Laboratory  
National Institute of Standards and Technology  

Email: sara.orski@nist.gov  
Staff website: https://www.nist.gov/people/sara-orski  

# How to cite
If you use the data, please cite:
Shuaijun Li, Robert J.S. Ivancic, Bradley P. Sutliff, Derek Huang, Enrique Blázquez-Blázquez, Tyler B. Martin, Kalman B. Migler, Debra J. Audus*, Sara V. Orski*, Data in support of “Machine learning-enhanced near-infrared property prediction for improved polyolefin differentiation”, National Institute of Standards and Technology, https://datapub.nist.gov/od/id/mds2-3809

If you use the code, please cite our submitted manuscript once published:
Shuaijun Li, Robert J.S. Ivancic, Bradley P. Sutliff, Derek Huang, Enrique Blázquez-Blázquez, Tyler B. Martin, Kalman B. Migler, Debra J. Audus*, Sara V. Orski*, "Machine learning-enhanced near-infrared property prediction for improved polyolefin differentiation " to be submitted.




