# Improving ecological clustering with *UMAP* and *HDBSCAN*: an application to the *Reef Life Survey* dataset

## Introduction

Coastal reefs are complex and important habitats for marine species. These habitats, generally built by engineered species, allow a rich fauna to find shelter, food and nursery areas. These biogenic habitats also have many roles in biogeochemical cycles and have a strong influence on hydrodynamics. Thus, these coastal reefs provide a number of important ecosystem services to other species living there, as well as to human populations living near the coast. However, biogenic habitats are facing major challenges due to climate change, pollution, and overfishing, among other things.


## Materials & Methods

Thus, a standardized classification of marine habitats on a global scale is critical to monitor, protect, and restore them. However, in order to carry out such a program, it is necessary to document the different types of habitat present on the Earth. The realization of such a typology is not an easy task. Indeed, it is necessary to be able to take into account fine-scale variability of marine habitats, while also taking into account larger-scale biogeographic variability patterns. Here, we propose an innovative clustering pipeline to overcome these two obstacles.

To conduct our habitat typology, we used habitat data from the Reef Life Survey program. This participatory science program samples rocky reefs around the world. We recovered 18 benthic substrate coverage from 6642 sites around the globe.

Before unsupervised classification algorithms can be used, it is important to use a dimension reduction algorithm to improve the performance of the classification algorithm. In order to obtain a good classification, the choice of the dimension reduction method is important. However, on a global scale, ecological data present important non-linearities. We chose to use UMAP, a non-linear dimension reduction algorithm that preserves the local structure of the data, allowing for easier classification.

To edit an efficient classification, the choice of the classification method is also particularly important. This choice must be made in light of the properties of the data set. Ecological data, and even more so participatory science data, can include a certain amount of noise that interferes with the analyses. Moreover, due to the non-linearity of the ecological phenomena studied, the groups to be identified can present various shapes and densities in the data space. It is to overcome these two major problems often encountered in ecology that we turned to an unsupervised clustering algorithm that is able to identify clusters of various shapes, while excluding noisy observations from the clusters.


Such a complex clustering pipeline makes its interpretation complex for users. To interpret the discovered clusters, we used SHapley Additive exPlanations (SHAP).

## Results & Conclusion 

Our clustering pipeline allowed us to identify 24 different habitat types across the globe. Using SHAP values, we were able to identify habitat coverage thresholds to characterize each of the clusters.

These clusters capture both biogeographic patterns (e.g., coral-dominated versus kelp-dominated reefs) and smaller-scale variability in ecological states (e.g., the gradient of healthy coral cover or ecotones). This habitat typology distinguishes both iconic marine habitats and ecotones. Thus, our methodology presented here allows for the identification of global-scale coastal habitat types of a given complex set, while retaining regional particularities. This pipeline can be applied to any complex ecological dataset to perform effective unsupervised classifications.

# About me

Hi! My name is Clément VIOLET, I am a PhD candidat at IFREMER :dolphin:. I am interested in how do coastal reefs respond to global climate change. If you have any questions, suggestions or whant to discuss about this workp, please feel free to send me an e-mail! :smile:

:email: [clement.violet@ifremer.fr](mailto:clement.violet@ifremer.fr)
