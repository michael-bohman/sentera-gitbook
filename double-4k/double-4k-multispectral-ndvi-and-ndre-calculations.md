---
description: >-
  This document describes the NDVI and NDRE calculations for the Double 4K (D4K)
  Multispectral camera.
---

# Double 4K Multispectral - NDVI and NDRE Calculations

## Multispectral

The D4K Multispectral camera is a bit different than other cameras, since each band must be normalized to each other before indices that use both cameras are calculated.

For the RGB side of the camera, the stacked filters result in the following spectral response, as shown in Figure 1:&#x20;

<div align="left"><figure><img src="../../.gitbook/assets/image (324).png" alt=""><figcaption><p><mark style="color:blue;">Figure 1: Stacked Filters</mark></p></figcaption></figure></div>

In Figure 1, red/green/blue correspond to channels of the resulting jpeg image. Note that there is some cross talk between the channels. That is, the blue channel has primarily blue wavelengths, but also has small contributions from the green and red wavelengths as well.

If it is necessary to separate the channels further, we can use a system of equations to subtract out the effect of the out of band channels on each band. This calculation assumes that the incoming light is approximately uniform (which is the case with daylight). We also add the constraint that the power across each of the filtered bands is equal. This allows us to perform calculations across each of the color bands, even if the filter widths vary.

This results in the following:&#x20;

DN \[color] = digital number of that band (from the jpeg)&#x20;

\[color] = Corrected color after subtracting out of band colors&#x20;



Blue = 1.37&#x37;_&#x44;Nblue - 0.18&#x32;_&#x44;NGreen - 0.06&#x31;_&#x44;NRed_&#x20;

_Green = -0.19&#x39;_&#x44;Nblue + 1.42&#x30;_&#x44;NGreen - 0.32&#x39;_&#x44;NRed&#x20;

Red = -0.03&#x34;_&#x44;Nblue - 0.11&#x30;_&#x44;NGreen + 1.150\*DNRed



&#x20;For the NIR/Red Edge camera, we have the following combined spectral response, as shown in Figure 2:

<div align="left"><figure><img src="../../.gitbook/assets/image (326).png" alt=""><figcaption><p><mark style="color:blue;">Figure 2: Combined Spectral</mark></p></figcaption></figure></div>

Note that from this imager, we only use the Blue channel for NIR and the Red channel for Red Edge. The green channel is discarded when performing index and band calculations. This is because there is not any additional useful information in the green band that isn't already captured by the blue and red bands.

Like the RGB method above (and subject to the same restrictions), we can subtract the out of band channels in the NIR and Red Edge portions via the following:



RedEdge = -0.95&#x36;_&#x44;Nblue + 1.00&#x30;_&#x44;Nred NIR = 2.42&#x36;_&#x44;Nblue - 0.34&#x31;_&#x44;Nred



When attempting to calculate indices that use both cameras, both the camera settings and the normalization factors used in the band math equations need to be considered during any index computations you may make.&#x20;

You will first have to normalize each of your images for the total exposure opportunity. This will allow images with differing ISO and exposure times to be compared properly.&#x20;

DN = Digital Number&#x20;

Gain = ISO / 100 \[Exif Tag]&#x20;

Shutter = Shutter time in seconds \[ Exif Tag]



ExposureOpportunity = DN / ( Gain \* Shutter )



The normalization values for each band separation matrix were chosen independently for each camera to keep 8-bit values in their proper ranges (typically 0-255). A normalization value of 1/750 was used for RGB, and 1/277.7 was used for RedEdge. This means that a step increase in RGB values implies a 2.7x step in the RedEdge values. So, if you want to compute indices that use both cameras you must consider our band math gains. This is done after the bands are separated using the above system of equations.

So, you end up with the following:



NDVI = (2.700 \* NIR\_2 - Red\_1) / (2.700 \* NIR\_2 + Red\_1)&#x20;

NDRE = (NIR\_2 - RedEdge\_2) / (NIR\_2 + RedEdge\_2)
