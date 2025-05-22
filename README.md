# Galaxy Classification with Machine Learning

A machine learning project that classifies galaxies as either elliptical or spiral based on their physical characteristics. This was made to practice and learn machine learning skills.

## Overview

This project demonstrates building a machine learning model to distinguish between two main types of galaxies:
- **Elliptical galaxies**: Smooth, blob-like galaxies with older stars
- **Spiral galaxies**: Galaxies with distinctive spiral arms and active star formation

The model uses numerical features that astronomers extract from galaxy observations, such as concentration of light, asymmetry, and smoothness.

## What I Learned

- Data exploration and visualization
- Feature analysis and importance
- Random Forest classification
- Model evaluation with confusion matrices
- Making predictions on new data

## Dataset Features

| Feature | Description | Elliptical | Spiral |
|---------|-------------|------------|--------|
| Concentration | Light concentrated in center | High | Low |
| Asymmetry | How symmetric the galaxy appears | Low | High |
| Smoothness | How smooth the light distribution is | High | Low |
| Ellipticity | How elongated the galaxy appears | Low | High |

## Usage

Classify new galaxies using the `classify_galaxy()` function:

```python
galaxy_type, confidence = classify_galaxy(
    concentration=0.85,
    asymmetry=0.15,
    smoothness=0.75,
    ellipticity=0.25
)

print(f"Prediction: {galaxy_type} galaxy")
print(f"Confidence: {confidence:.2%}")
```

## Results

- **Accuracy**: 85-95% on test data
- **Key Features**: Smoothness and concentration are most important
- **Output Files**: Feature distribution plots, importance charts, galaxy images from ESA Hubble

## Next Steps

1. Use real galaxy datasets from Galaxy Zoo or SDSS
2. Try different ML algorithms (SVM, Neural Networks)
3. Add more galaxy types (irregular, lenticular)
4. Move to image-based classification with deep learning

## Resources

- [ESA Hubble Gallery](https://esahubble.org/images/) - Source for galaxy images used in this project
