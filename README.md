<a name="readme-top"></a>

<!-- PROJECT LOGO -->
<br />

<div align="center">
  <a href="https://github.com/alaaNfissi/Unlocking-the-Emotional-States-of-High-Risk-Suicide-Callers-through-Speech-Analysis">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center"> Unlocking the Emotional States of High-Risk Suicide Callers through Speech Analysis </h3>

  <p align="center">
    This paper has been submitted for publication in the 35th IEEE International Conference on Tools with Artificial Intelligence (ICTAI).
    <br />
   </p>
   <!-- <a href="https://github.com/alaaNfissi/Unlocking-the-Emotional-States-of-High-Risk-Suicide-Callers-through-Speech-Analysis"><strong>Explore the docs »</strong></a> -->
</div>
   

  
<div align="center">

[![view - Documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](https://github.com/alaaNfissi/Unlocking-the-Emotional-States-of-High-Risk-Suicide-Callers-through-Speech-Analysis/#readme "Go to project documentation")

</div>  


<div align="center">
    <p align="center">
    ·
    <a href="https://github.com/alaaNfissi/Unlocking-the-Emotional-States-of-High-Risk-Suicide-Callers-through-Speech-Analysis/issues">Report Bug</a>
    ·
    <a href="https://github.com/alaaNfissi/Unlocking-the-Emotional-States-of-High-Risk-Suicide-Callers-through-Speech-Analysis/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#abstract">Abstract</a></li>
    <li><a href="#built-with">Built With</a></li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#getting-the-code">Getting the code</a></li>
        <li><a href="#dependencies">Dependencies</a></li>
      </ul>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

<!-- ABSTRACT -->
## Abstract

<p align="justify"> Suicide remains a major public health concern worldwide, and early detection of suicidal ideation is crucial for prevention. One promising approach to monitoring symptoms is through the prediction of suicidal speech, as speech can be passively collected and may provide insight into changes in risk. However, directly identifying suicidal speech is difficult due to the rapid variability in speech characteristics and the association of suicidal ideation with emotion dysregulation.
In light of these challenges, we present a novel end-to-end (E2E) method for speech emotion recognition (SER) as a mean of detecting changes in emotional state that may indicate an increased risk for suicide. Our method incorporates the use of Convolutional Neural Networks (CNNs) and Gated Recurrent Units (GRUs) to analyze raw waveform signals. Firstly, our model is designed to train the CNN component to identify higher-level speech representations directly from raw waveform data, rather than relying on manually crafted features or spectrograms. This approach enables the network to effectively capture specific emotion-related features within a narrow frequency range, while also handling speech of varying lengths without the need for segmentation. Secondly, the GRU component is capable of learning temporal patterns, enhancing the network's ability to capture time-dependent features of the signal. 
Furthermore, we introduce our NSPL-CRISE emotion dataset for our research, which contains phone call recordings from individuals who are lifeline frequent callers with serious physical and psychological problems and a history of suicidal ideation, planning, and previous attempts. This dataset provides valuable insights into the emotional states of individuals at high risk for suicide.
The goal of this research is to provide a promising approach to symptom monitoring and, ultimately, suicide prevention through early detection of suicidal ideation. Our experimental results show that our method outperforms other state-of-the-art techniques for SER. </p>

<div align="center">
  
![model-architecture][model-architecture]
  
*Proposed model architecture*
  
</div>

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With
* ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
* ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
* ![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
* ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
* ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
* ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started
<p align="justify">
  
All source code used to generate the results and figures in the paper are in
the `CNN-n-GRU` folder.
The calculations and figure generation are all run inside
[Jupyter notebooks](http://jupyter.org/).
  
</p>

### Getting the code

You can download a copy of all the files in this repository by cloning the
[git](https://git-scm.com/) repository:

    git clone https://github.com/alaaNfissi/Unlocking-the-Emotional-States-of-High-Risk-Suicide-Callers-through-Speech-Analysis.git

or [download a zip archive](https://github.com/alaaNfissi/Unlocking-the-Emotional-States-of-High-Risk-Suicide-Callers-through-Speech-Analysis/archive/refs/heads/main.zip).

### Dependencies

<p align="center">

You'll need a working Python environment to run the code.
The recommended way to set up your environment is through the
[Anaconda Python distribution](https://www.anaconda.com/download/) which
provides the `conda` package manager.
Anaconda can be installed in your user directory and does not interfere with
the system Python installation.
The required dependencies are specified in the file `requirements.txt`.

We use `conda` virtual environments to manage the project dependencies in
isolation.
Thus, you can install our dependencies without causing conflicts with your
setup (even with different Python versions).

Run the following command to create an `ser-env` environment to create a separate environment:
```sh 
    conda create --name ser-env
```
Activate the environment, this will enable the it for your current terminal session. Any subsequent commands will use software that is installed in the environment:
```sh 
    conda activate ser-env
 ``` 
Use Pip to install packages to Anaconda Environment:
```sh 
    conda install pip
```
Install all required dependencies in it:
```sh
    pip install -r requirements.txt
```

</p>

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

All source code is made available under a BSD 3-clause license. You can freely
use and modify the code, without warranty, so long as you provide attribution
to the authors. See `LICENSE.md` for the full license text.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Alaa Nfissi - [@LinkedIn](https://www.linkedin.com/in/alaa-nfissi/) - alaa.nfissi@mail.concordia.ca

Github Link: [https://github.com/alaaNfissi/Unlocking-the-Emotional-States-of-High-Risk-Suicide-Callers-through-Speech-Analysis](https://github.com/alaaNfissi/Unlocking-the-Emotional-States-of-High-Risk-Suicide-Callers-through-Speech-Analysis)

<p align="right">(<a href="#readme-top">back to top</a>)</p>




<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[model-architecture]: images/cnn-n-gru-smc.png


[anaconda.com]: https://anaconda.org/conda-forge/mlconjug/badges/version.svg
[anaconda-url]: https://anaconda.org/conda-forge/mlconjug

[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
