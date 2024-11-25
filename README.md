<div align="center">
  <p>
        <img src="images/LCZprocess.png" width="600">
</p>
</div>

# Introduction
Local Climate Zone (LCZ) classification system offers the standardization of urban heat island studies and addresses the shortcomings of the urban-rural division (Stewart & Oke 2012). Given the increasing attention in LCZ, this project aims to illustrate an efficient and adaptable GIS-based LCZ mapping framework within the Uunited States. A modified standard rule-based approach was used to map 100m resolution LCZs in Denton County. All data proessing was performed in ArcGIS.


| Band Value | LCZ | Label |
|----------|----------|----------|
| 5 | 5 | Scattered trees |
| 6 | 6 | Low plants |
| 8 | 8 | Large lowrise |
| 9 | 9 | Sparsely built |
| 11 | A | Dense trees |
| 12 | B | Scattered trees |
| 14 | D | Low plants |
| 15 | E | Bare rock or paved |
| 16 | F | Bare soil or sand  |
| 17 | G | Water |
| 18 | 6D | Open lowrise & low plants |

# Urban Canopy Parameters
* Maxmium building footprint (m²)
* Number of building
* Mean building height (m)
* Building surface fraction (%)
* Majority landcover
* Tree canopy surface fraction (%)
* Pervious surface fraction (%)


# Evaluation
150 samples were generated using stratified random sampling. Each of the LCZ has at least 10 samples. High resolution satellite imagery was used to build the groundtruth.

The overall accuracy is 82% and the kappa coefficient is 0.78. Below is the confusion matrix:

| LCZ | B | D | 8 | 9 | G | A | F | E | 6 | 5 | Total | User Accuracy |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:----:|:---:|
|  B  | 7 | 1 | 0 | 0 | 1 | 0 | 0 | 0 | 1 | 0 |  10   |     0.7       |
|  D  | 4 | 46| 1 | 2 | 0 | 2 | 0 | 0 | 0 | 0 |  55   |     0.84      |
|  8  | 0 | 0 | 9 | 0 | 0 | 0 | 0 | 0 | 1 | 0 |  10   |     0.9       |
|  9  | 1 | 0 | 0 | 9 | 0 | 0 | 0 | 0 | 0 | 0 |  10   |     0.9       | 
|  G  | 0 | 0 | 0 | 0 | 10| 0 | 0 | 0 | 0 | 0 |  55   |     1         |
|  A  | 1 | 0 | 0 | 0 | 0 | 9 | 0 | 0 | 0 | 0 |  10   |     0.9       |
|  F  | 0 | 1 | 2 | 1 | 0 | 0 | 3 | 0 | 3 | 0 |  10   |     0.3       | 
|  E  | 0 | 1 | 0 | 0 | 0 | 0 | 0 | 9 | 0 | 0 |  10   |     0.9       |
|  6  | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 15| 0 |  15   |     1         |
|  5  | 0 | 1 | 3 | 0 | 0 | 0 | 0 | 0 | 0 | 6 |  10   |     0.6       |
|Total| 13| 50| 15| 12| 11| 11| 3 | 9 | 20| 6 |  150  |               |
|Producer Accuracy| 0.54 | 0.92 | 0.6 | 0.75 | 0.91 | 0.82 | 1 | 1 | 0.75 | 1 |     |     0.82       |
