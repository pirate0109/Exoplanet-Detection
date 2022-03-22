## Exoplanet Detection Using Machine Learning


### Project Description
The kepler mission was lauched to figure out earthlike planets revolving along stars. There have been more than 1000 confirmed stars with exoplanets thanks to this mission and more than 3000 stars with potential planets around it. The methodology used is Transit Photometry Method where a distant planet is detected by measuring the change in flux  of a star as it passes between a planet and the earth. Thus if the planet is present around the star, there would be miniscule reduction in the flux intensity of star during transit. 

### Dataset

The dataset was made available as a part of Annual Inter-IIT competition held in IIT Madras. This dataset contains flux of over 5000 stars in a time series form. Its a binary classification problem with label 1 represent that the star no confirmed exoplanet and 2 represented that the star has atleast one exoplanet.


### Data Preprocessing

**Noise Removal**
The random bunching of photons introduces the noise in the measured flux. These are also known as shot noise. We applied Gaussian filter to  attenuate the high frequency flux thus smoothing some random shot noises in the data.

**Standardization**
The flux of the exoplanet depends in how big it is. It also depends on the type of the exoplanet, distance etc. Thus it becomes very important to put the data on the same scale. We scaled the flux data between 0 to 1.

![Denoising and Standardization](images/denoise.png)

