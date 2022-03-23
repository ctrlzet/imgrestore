<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][https://github.com/scalyvladimir]

<!-- ABOUT THE PROJECT -->
## About The Project

This repo provides the replication of paper on image restoration. The goal is to restore high-quality images from low-quality images. We utilized SwinIR [(Liang et al., 2021)](https://arxiv.org/abs/2108.10257) model based on the Swin Transformer, which consisted of three main parts:
* Shallow feature extraction
* Deep feature extraction
  – Composed of many residual Swin Transformer blocks (RSTB), each has several Swin Transformers layers together with a residual connection
* High-quality image reconstruction.
We examined the performance of SwinIR with its default blind noises against our own synthetic noise. Moreover, we implemented the ISTA/FISTA algorithms with SwinIR as a de-noising model for non-blind deblurring problem.

<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/ctrlzet/imgrestore
   ```

<!-- ROADMAP -->
## Roadmap

Our repo follows steps mentioned in [2nd](https://drive.google.com/file/d/1QSgaFGV3dygyWZ2JUkI_GHgAytU5b-sI/view) project description

- [main branch](https://github.com/ctrlzet/imgrestore/tree/main) consists of two directories correspoding to [training](https://github.com/ctrlzet/imgrestore/tree/main/training) and [inference](https://github.com/ctrlzet/imgrestore/tree/main/inference) procedures each. This is all about replication of original paper + implication of projection layer. User required to follow a step-by-step intructions mentioned in `.ipynb` files located in same path.
- The first task covering research solved [here](https://github.com/ctrlzet/imgrestore/blob/main/Research_task1.pdf).
- Finally, ISTA/FISTA algorithms stored [here](https://github.com/ctrlzet/imgrestore/tree/ISTA_implementation).

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

<!-- CONTACT -->
## Contact

Vladimir Chernyy - Vladimir.Chernyy@skoltech.ru - author of README.md

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/github_username/repo_name.svg?style=for-the-badge
[contributors-url]: https://github.com/github_username/repo_name/graphs/contributors

<p align="right">(<a href="#top">back to top</a>)</p>
