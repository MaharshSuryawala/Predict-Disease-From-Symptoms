# Predict-Disease-From-Symptoms

<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]][contributors-url]
[![Stargazers](https://img.shields.io/github/stars/MaharshSuryawala/Predict-Disease-From-Symptoms?style=flat-square)]()
[![Followers](https://img.shields.io/github/followers/MaharshSuryawala?style=flat-square)](https://github.com/MaharshSuryawala)
[![MIT License][license-shield]][license-url]
[![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/MaharshSuryawala/Predict-Disease-From-Symptoms)

<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the Project](#about-the-project)
  * [Overview](#overview)
  * [Built With](#built-with)
  * [Dataset](#dataset)
* [Results](#results)
* [Contributing](#contributing)
* [License](#license)
* [Contact](#contact)
* [References](#references) 
* [Acknowledgements](#acknowledgements)

## About the Project

![Food](.images/doc.jpg)

<span>Photo by <a href="https://unsplash.com/@nci?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">National Cancer Institute</a> on <a href="https://unsplash.com/s/photos/medical?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Unsplash</a></span>


### Overview

* According to a recent study carried out by [BMJ quality and safety](https://qualitysafety.bmj.com/), 12 million adults who seek medical care are misdiagnosed each year in the United States. 
* The accumulation of large case loads and incomplete medical histories lead to rise in human-errors. 
* An Artificial Intelligent system can predict and diagnose a disease at a faster and more efficient way as compared to medical professionals. 
* In the following project we will be predicting diseases from symptoms using machine learning algorithms like decision tree and random forests. 
* Moreover, we will try to plot the diseases and symptoms and create a network graph to analyse the common symptoms between diseases, most common symtoms, most common diseases etc.  

### Built With

* [Python](https://www.python.org/)
* [Jupyter Notebook](https://jupyter.org/)

### Dataset

Source: [Disease-Symptom Knowledge Database](http://people.dbmi.columbia.edu/~friedma/Projects/DiseaseSymptomKB/index.html)
  
  * The data set consists of 148 diseases with their corresponding symptoms. 
  * The data set also included the count of disease occurences.  
  
## Results

### Disease-Symptoms Network 

![Disease-Symptoms Network](disease_symptom_network.png)

### Decision Tree

* Model Accuracy - 90.54%

* Text Representation 

|--- atypia <= 0.50

|   |--- pleuritic pain <= 0.50

|   |   |--- low back pain <= 0.50

|   |   |   |--- hypertonicity <= 0.50

|   |   |   |   |--- hyperkalemia <= 0.50

|   |   |   |   |   |--- dysarthria <= 0.50

|   |   |   |   |   |   |--- abnormally hard consistency <= 0.50

|   |   |   |   |   |   |   |--- feeling  suicidal <= 0.50

|   |   |   |   |   |   |   |   |--- debilitation <= 0.50

|   |   |   |   |   |   |   |   |   |--- hepatomegaly <= 0.50

|   |   |   |   |   |   |   |   |   |   |--- enuresis <= 0.50

|   |   |   |   |   |   |   |   |   |   |   |--- truncated branch of depth 50

|   |   |   |   |   |   |   |   |   |   |--- enuresis >  0.50

|   |   |   |   |   |   |   |   |   |   |   |--- truncated branch of depth 3

|   |   |   |   |   |   |   |   |   |--- hepatomegaly >  0.50

|   |   |   |   |   |   |   |   |   |   |--- swelling <= 0.50

|   |   |   |   |   |   |   |   |   |   |   |--- class: primary  carcinoma of the liver cells

|   |   |   |   |   |   |   |   |   |   |--- swelling >  0.50

|   |   |   |   |   |   |   |   |   |   |   |--- class: lymphatic  diseases

|   |   |   |   |   |   |   |   |--- debilitation >  0.50

|   |   |   |   |   |   |   |   |   |--- aura <= 0.50

|   |   |   |   |   |   |   |   |   |   |--- class: carcinoma of lung

|   |   |   |   |   |   |   |   |   |--- aura >  0.50

|   |   |   |   |   |   |   |   |   |   |--- class: encephalopathy

|   |   |   |   |   |   |   |--- feeling  suicidal >  0.50

|   |   |   |   |   |   |   |   |--- class: depression  mental

|   |   |   |   |   |   |--- abnormally hard consistency >  0.50

|   |   |   |   |   |   |   |--- class: cholecystitis

|   |   |   |   |   |--- dysarthria >  0.50

|   |   |   |   |   |   |--- enuresis <= 0.50

|   |   |   |   |   |   |   |--- difficulty <= 0.50

|   |   |   |   |   |   |   |   |--- paresis <= 0.50

|   |   |   |   |   |   |   |   |   |--- numbness <= 0.50

|   |   |   |   |   |   |   |   |   |   |--- stridor <= 0.50

|   |   |   |   |   |   |   |   |   |   |   |--- class: benign  prostatic hypertrophy

|   |   |   |   |   |   |   |   |   |   |--- stridor >  0.50

|   |   |   |   |   |   |   |   |   |   |   |--- class: deglutition  disorder

|   |   |   |   |   |   |   |   |   |--- numbness >  0.50

|   |   |   |   |   |   |   |   |   |   |--- class: accident  cerebrovascular

|   |   |   |   |   |   |   |   |--- paresis >  0.50

|   |   |   |   |   |   |   |   |   |--- class: hemiparesis

|   |   |   |   |   |   |   |--- difficulty >  0.50

|   |   |   |   |   |   |   |   |--- class: transient  ischemic attack

|   |   |   |   |   |   |--- enuresis >  0.50

|   |   |   |   |   |   |   |--- class: confusion

|   |   |   |   |--- hyperkalemia >  0.50

|   |   |   |   |   |--- patient non compliance <= 0.50

|   |   |   |   |   |   |--- hypotension <= 0.50

|   |   |   |   |   |   |   |--- rhonchus <= 0.50

|   |   |   |   |   |   |   |   |--- pain chest <= 0.50

|   |   |   |   |   |   |   |   |   |--- rest pain <= 0.50

|   |   |   |   |   |   |   |   |   |   |--- class: respiratory  failure

|   |   |   |   |   |   |   |   |   |--- rest pain >  0.50

|   |   |   |   |   |   |   |   |   |   |--- class: peripheral  vascular disease

|   |   |   |   |   |   |   |   |--- pain chest >  0.50

|   |   |   |   |   |   |   |   |   |--- class: kidney  disease

|   |   |   |   |   |   |   |--- rhonchus >  0.50

|   |   |   |   |   |   |   |   |--- class: Alzheimer's  disease

|   |   |   |   |   |   |--- hypotension >  0.50

|   |   |   |   |   |   |   |--- hypokalemia <= 0.50

|   |   |   |   |   |   |   |   |--- orthopnea <= 0.50

|   |   |   |   |   |   |   |   |   |--- class: kidney  failure acute

|   |   |   |   |   |   |   |   |--- orthopnea >  0.50

|   |   |   |   |   |   |   |   |   |--- class: insufficiency  renal

|   |   |   |   |   |   |   |--- hypokalemia >  0.50

|   |   |   |   |   |   |   |   |--- class: overload  fluid

|   |   |   |   |   |--- patient non compliance >  0.50

|   |   |   |   |   |   |--- class: edema  pulmonary

|   |   |   |--- hypertonicity >  0.50

|   |   |   |   |--- class: thrombus

|   |   |--- low back pain >  0.50

|   |   |   |--- class: aphasia

|   |--- pleuritic pain >  0.50

|   |   |--- diarrhea <= 0.50

|   |   |   |--- cicatrisation <= 0.50

|   |   |   |   |--- metastatic lesion <= 0.50

|   |   |   |   |   |--- egophony <= 0.50

|   |   |   |   |   |   |--- class: influenza

|   |   |   |   |   |--- egophony >  0.50

|   |   |   |   |   |   |--- class: upper  respiratory infection

|   |   |   |   |--- metastatic lesion >  0.50

|   |   |   |   |   |--- class: endocarditis

|   |   |   |--- cicatrisation >  0.50

|   |   |   |   |--- class: embolism  pulmonary

|   |   |--- diarrhea >  0.50

|   |   |   |--- jugular venous distention <= 0.50

|   |   |   |   |--- hemodynamically stable <= 0.50

|   |   |   |   |   |--- productive cough <= 0.50

|   |   |   |   |   |   |--- class: bacteremia

|   |   |   |   |   |--- productive cough >  0.50

|   |   |   |   |   |   |--- class: HIV

|   |   |   |   |--- hemodynamically stable >  0.50

|   |   |   |   |   |--- class: carcinoma prostate

|   |   |   |--- jugular venous distention >  0.50

|   |   |   |   |--- class: chronic  kidney failure

|--- atypia >  0.50

|   |--- lung nodule <= 0.50

|   |   |--- class: arthritis

|   |--- lung nodule >  0.50

|   |   |--- class: neoplasm  metastasis


* Decision Tree

![Decision Tree](decision_tree_graphivz.png)

<!-- CONTRIBUTING -->
## Contributing  

Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/amazing-feature`)
3. Commit your Changes (`git commit -m 'feat: some amazing feature'`)
4. Push to the Branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.

<!-- CONTACT -->
## Contact
[![Linkedin](https://api.iconify.design/openmoji:linkedin.svg?width=40&height=40)](https://www.linkedin.com/in/maharsh-suryawala-05410312b/) 

Maharsh Suryawala - [Portfolio](https://maharshsuryawala.github.io/maharshsuryawala/)

Project Link: [https://github.com/MaharshSuryawala/Predict-Disease-From-Symptoms](https://github.com/MaharshSuryawala/Predict-Disease-From-Symptoms)

## References

* [https://builtin.com/artificial-intelligence/artificial-intelligence-healthcare](https://builtin.com/artificial-intelligence/artificial-intelligence-healthcare)

<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements
* [Img Shields](https://shields.io)
* [Iconify](https://iconify.design/)
* [MIT License](https://opensource.org/licenses/MIT)
* [Unsplash](https://unsplash.com/)
* [Badgen](https://badgen.net/)
* [For The Badge](https://forthebadge.com/)


[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)


[![ForTheBadge built-with-love](http://ForTheBadge.com/images/badges/built-with-love.svg)](https://github.com/MaharshSuryawala)


<!-- MARKDOWN LINKS -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/MaharshSuryawala/Predict-Disease-From-Symptoms?style=flat-square 
[contributors-url]: https://github.com/MaharshSuryawala/Predict-Disease-From-Symptoms/graphs/contributors
[license-shield]: https://img.shields.io/github/license/MaharshSuryawala/Predict-Disease-From-Symptoms?style=flat-square?style=flat-square
[license-url]: https://github.com/MaharshSuryawala/Predict-Disease-From-Symptoms?style=flat-square/blob/master/LICENSE.txt
