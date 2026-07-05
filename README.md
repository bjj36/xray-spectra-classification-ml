# X-Ray Spectra Classification Using Machine Learning

## Overview
Softmax classification and K-means clustering applied to X-ray absorption spectra of chromium compounds, implemented from scratch in Python and NumPy. Completed as assessed coursework for MA22037 Machine Learning 1 at the University of Bath. This project builds a machine learning pipeline to classify X-ray absorption spectra of three chromium compounds, and applies the trained model to predict the composition of an unknown specimen pixel by pixel, producing a classification image. Two feature engineering approaches are compared: simple feature undersampling and K-means clustering of spectral features.

## Key Techniques
- Softmax classification implemented from first principles using NumPy
- Cross-entropy loss and gradient computation
- Adjusted gradient descent with early stopping
- Learning rate selection via systematic comparison of convergence behaviour
- K-means clustering for spectral feature engineering using scikit-learn
- End-to-end ML pipeline from raw spectroscopy data through feature engineering to classification image

## Structure

- CW_bjj36.ipynb — Main notebook containing all implementations and analysis
- CW_report_bjj36.docx — Written report summarising findings and model comparison
- CWData.npz — Not included due to file size. The notebook expects a file with the following variables: Xh (300x3959 matrix of spectra), Y (300x3 label matrix), Xhnew (332x3959 matrix of unknown specimen spectra), and Energies (vector of 3959 energy values)

## Requirements
- numpy
- matplotlib
- sklearn

## Note
This project was completed as assessed individual coursework. GenAI was used to debug a logic error in the early stopping condition and to assist with classification map visualisation code, as declared in the notebook in accordance with the university's academic integrity policy.
