
![GSoC mlpack image](./gsoc-mlpack.png)

**Organisation: [mlpack](https://github.com/mlpack)**

**Project: [Example Zoo](https://summerofcode.withgoogle.com/programs/2022/projects/1hgAURBM)**

**Mentors: [Ryan Curtin](https://github.com/rcurtin) and [Kartik Dutt](https://github.com/kartikdutt18)**

## Abstract
This summer, I was selected for Google Summer of Code to work on project `Example Zoo` for mlpack organization. Mlpack is a fast, flexible C++ machine learning library aiming to provide fast, extensible implementations of cutting-edge machine learning algorithms. mlpack is open source software, which means it is a community-led effort. 
Over the course of the last years, various machine-learning algorithms have been implemented as a part of mlpack. This project focused on applying some of the algorithms to interesting datasets to see how they fare. This allowed us to show (off!) the potential usage of mlpack through various real-world domains.


## Goal
- The main objective of the project was to deliver two or three medium sized notebooks in Python. One of them should be a regression notebook while another one should be a classification notebook.
- We discovered along the way that the imputer function in mlpack had no Python binding. So, after finishing the first part of the project, we worked on adding Python binding support for the imputer function.


## Results

A total of 3 Python notebooks were added to the examples repository. In each one of them, I performed:
- Data preliminary wrangling
- Data cleaning
- Exploration of data
- Visualizations to better understand the data
- Applying the machine learning models
- Evaluating the models and making prediction

## Contributions 

Here is the list of PRs (both open & closed) that I created during GSoC.

| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PULL &nbsp;&nbsp;REQUESTS                         | &nbsp;&nbsp;COMMITS                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;DESCRIPTION                                                                                     | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;STATUS |
|:------------------------------------------------------------------------------------- |:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |:------------------------------------------ |
| [#200](https://github.com/mlpack/examples/pull/200)                                   | <ul> <li> [c8059d9](c8059d93220c4d50d13822e1674eeea5eb105b06) </li> <li> [cb3300b](cb3300b5daee8288b7d0218fa7e11911e1a445e5) </li> <li> [10306d3](10306d357f96e1ae20b513ede7073f25bb6fd2ad) </li> <li> [e07e4cf](e07e4cf94a2cb1e2f7a9443d8799fd91dd62c2f0) </li> <li> [c83e12a](c83e12a7b058b29543833673bfc100d083aa8557) </li> <li> [c62c07c](c62c07cf7988cf88d9d16168308c2997411bb09f) </li> <li> [bfb0931](bfb0931bb6ad10e3e3aa9b53fe5e93ed715169bd) </li> <li> [c83a94b](c83a94b0fd2a37427b34517947775feca5ff3a63) </li> <li> [4397d71](4397d71eca10a9c5a4e22614d5057f29e4a788b1) </li> </ul>                                                                                                                                                                                              | **NYC Airbnb price prediction**<br>- Performed descriptive and exploratory analysis of the data in order to understand how the phenomena of each variable behave individually a	d transversely.<br>   - Used kernel density estimation (KDE) to estimate of the underlying distribution of the target variable.<br> - Applied One-Hot-Encoding to categorical variables.<br> - Used cross-validation to choose between several machine learning models (Linear regression - Ridge Regression - Bayesian Linear Regression) to accurately predict the price of the listing.                                                                    | :purple_square:Merged                      |
| [#202](https://github.com/mlpack/examples/pull/202)                            | <ul> <li> [ea7e833](ea7e833bf67f0ffe967ad179a16628de2f3a1a38) </li> <li> [e265ccf](e265ccfc943ee3bb891522ced071fb59449b1450) </li> <li> [a6a1280](a6a1280eec745071e3b7ed8df9eaa7c29b0a5e5e) </li> <li> [497ed93](497ed932890d3c3a5b83129a54b3f7b4a8092408) </li> <li> [f546a63](f546a632f007d6bec567c04e6680168df5f5bfcf) </li> <li> [05a74a9](05a74a93e874b7090cbea444ed4d8a050281ab3e) </li> <li> [dd7de1e](dd7de1e5f142d45ba108b32b835bfafc366e13d8) </li> <li> [9945371](9945371c1f6f0318ece354bffafe875e847be4d5) </li> <li> [5213253](52132531c6c691c38e4cfb5715402e7dee14e48d) </li> <li> [8520c49](8520c49d2381fc557ab8e642a06374ae99994fcd) </li> <li> [2811236](28112361e002cc2dd17f4911fa846f6692a2e1ab) </li> </ul>                                                                                                                                                                                              | **Rain in Australia prediction**<br>- Applied exploratory data analysis techniques to the data to better understand the underlying patterns. <br>- Applied feature engineering which included encoding date as it is a cyclic feature and handling class imbalance for classification. <br>- Used feature scaling and PCA for dimensionality reduction. <br>- Implemented 3 classification models (Naïve Bayes - Random Forest - Logistic Regression) to predict whether it rains the next day or not. </li> </ul>                                                                                                                                                                                                                       | :purple_square:Merged                      |
| [#205](https://github.com/mlpack/examples/pull/205)                            | <ul> <li> [1b44d08](1b44d08c6e71d4a1f3d95fbab10447faf41bbb3a) </li> <li> [924c779](924c779b50a4b8071a140a9614d4f1357cad1e94) </li> <li> [5678e7c](5678e7c3e86f3e56b35048ae553ed17e7e0c77d3) </li> </ul>                                                                                                                                                                                                                                                                                                                                                                                                                                                          | **Customer Personality Analysis** is a detailed analysis of a company’s ideal customers. It helps a business to better understand its customers. <br>The notebook includes:<br>- Exploratory data analysis. <br>- Feature engineering.<br>- Performing an unsupervised clustering of data using Kmeans to optimize the significance of each customer to the business.<br>                                                                                                                                                                                                                                                            | :purple_square:Merged                      |
| [#97](https://github.com/castor-software/depclean/pull/97)                            | <ul> <li> [ea7e833](ea7e833bf67f0ffe967ad179a16628de2f3a1a38) </li> <li> [e265ccf](e265ccfc943ee3bb891522ced071fb59449b1450) </li> <li> [a6a1280](a6a1280eec745071e3b7ed8df9eaa7c29b0a5e5e) </li> <li> [497ed93](497ed932890d3c3a5b83129a54b3f7b4a8092408) </li> <li> [f546a63](f546a632f007d6bec567c04e6680168df5f5bfcf) </li> <li> [05a74a9](05a74a93e874b7090cbea444ed4d8a050281ab3e) </li> <li> [dd7de1e](dd7de1e5f142d45ba108b32b835bfafc366e13d8) </li> <li> [9945371](9945371c1f6f0318ece354bffafe875e847be4d5) </li> <li> [5213253](52132531c6c691c38e4cfb5715402e7dee14e48d) </li> <li> [8520c49](8520c49d2381fc557ab8e642a06374ae99994fcd) </li> <li> [2811236](28112361e002cc2dd17f4911fa846f6692a2e1ab) </li> </ul>                                                                                                                                                                                              | In this PR, We are working on adding Python binding support for the imputer function                                                                                                                                                                                          | :green_square:Open                      |
## Evaluation metrics
1. NYC Airbnb price prediction


2. Rain in Australia prediction


3. Customer personality clustering
## Future plans 
## Acknowledgement 
## Ways to reach me

<p align="center">
  <a href="mailto:tareknaser360@gmail.com?subject = Hello from your GitHub README&body = Message"><img src="./gmail.svg" height="80px" width="80px" alt="Gmail" ></a>
  <a href="https://www.linkedin.com/in/tareknasser360/"><img src="./linkedIn.svg" height="80px" width="80px" alt="LinkedIn"></a>
</p>
