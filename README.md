**Emilio Yanez** <img align="right" width="220" height="220" src="/assets/IMG/template_logo.png">

## C111 Final Project: Emilio Yanez

### Dataset

See the two .txt files above (in `assets`)

### Report
Atmospheric Rivers (ARs) are elongated and narrow filaments of water vapor transport in the atmosphere. Convergence of these water vapor plumes is often associated with heavy precipitation events (e.g., US West Coast). As part of my research in Dr. Gang Chen’s group, we have quantified the relationship between an AR’s moisture, wind, integrated vapor transport (IVT), and associated precipitation in two main ways. The first is by developing a global, percentile-based classification of wet and windy ARs in satellite observations (similar to [2]). The second (and the focus of this project) is using a binned scatter approach to understand better the sensitivity of mean AR precipitation to changes in other AR variables (e.g., moisture, wind, and IVT). Binned scatter plots [1] divide the independent variable into dynamically-sized bins and find the conditional means of a dependent variable, similar to the convective onset statistics for tropical convective precipitation against changes in water vapor [3]. In previous work, we found a strong conditional relationship between mean AR IVT and mean AR precipitation, regardless of the ocean basin and season. These conditional statistics in satellite observations may provide a benchmark for quantifying the relationship between ARs and precipitation in other data sets (such as reanalysis and climate models). As such, understanding and building an accurate “base” AR IVT-precipitation relationship is important for subsequent studies.

Deriving a conditional relationship between AR IVT and AR precipitation from raw data is challenging since there is considerable noise when plotting a simple scatterplot. This motivates using a machine learning (ML) approach to simplify the scatter in the data. Supervised algorithms, such as linear regression, support vector regression, and random forest regression can be used to predict mean AR precipitation from other AR variables. Once the ML model is trained, we can plot new scatter plots of mean AR IVT versus the predicted mean AR precipitation. The hope is that the predicted data, modeled from real satellite data, can reproduce the conditional AR IVT-precipitation relationship found in the original, non-ML method (my previous research). Overall, I find that all three ML models (linear, SVR, and random forest) predict the original conditional relationship with good accuracy.

For the full report, see [link](assets/AOS_C111_Final_Project_Report_EY.pdf) or the above PDF file (in `assets`).

### Code

On BruinLearn, or [link](https://colab.research.google.com/drive/1M-5st5HlL7MYsYQ3k0VK4jblUYzewdqg?usp=sharing).
