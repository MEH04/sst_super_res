# Super-Resolution of Global Ocean Surface Temperature by Deep Learning
This is a summer research project carried out at the University of Reading Dept. of Meteorology.\
**Research by:** Matthew Howarth\
**Supervised by:** Prof. Chris Merchant, Dr. Niall McCarroll
## Research Overview
- Deep convolutional neural networks are designed in PyTorch and applied to super-resolve level 4 (L4) sea surface temperature (SST) data into gradient-restored (gR) data
- A gridding and blending algorithm is written to apply the model to large ocean regions, and transform from the gradient -> SST domain
- A pipeline is established for data pre-processing, ML training and model output analysis.

[A more comprehensive report and research poster](https://drive.google.com/drive/folders/1q6u0bg-89681OEiabz4U3XBC3hNv49DN?usp=sharing)
## Code Overview
The below descriptions of each notebook are written in the order of the pipeline: 
1. `data_analysis.ipynb`: A number of tools for analysing the SST data.
2. `cloud_classifier.ipynb`: An iPyWidget app for classifying images as cloudy or non-cloudy to establish the filtering threshold.
3. `data_extractor.ipynb`: Process data ready for machine learning.
4. `model.ipynb`: Load data into PyTorch, design and train architectures: the main machine learning file.
5. `reconstuction.ipynb`: An explanatory notebook for the gradient -> SST re-construction algorithm.
6. `region.ipynb`: Grid a large ocean region, apply the model, re-stitch, re-construct and find the power spectrum.
## Main References
- [L4 data product](doi.org/10.1038/s41597-024-03147-w)
- [Code for obtaining gR data](github.com/surftemp/sst-gradients)
- [Super-resolution architectures](doi.org/10.3390/rs14051159)


