# Text-to-ImageGAN

This project is a part of the AAI-521 course in the Applied Artifical Intelligence Program at the University of San Diego (USD).

-- Project Status: Completed

## Installation

To use this project, go to https://huggingface.co/sglasher/van-gogh-stable-diffusion, or use the script "Text-to-ImageFinalProject_Final.ipynb". It is the main script, which requires the other files already saved in this repository. 

## Project Intro/Objective

The main purpose of this project is to create AI generated artwork. The capability of text-to-image generation to emulate specific artistic styles, such as those of iconic figures like Vincent Van Gogh, provides a remarkable avenue for promoting and marketing the works of deceased artists.

## Partners/Contributors

* Caterina Gallo, Jeremy Krick, Se’Lina Lasher

## Methods Used

* Computer Vision
* Machine Learning
* Deep Learning

## Technologies

* Python
* Hugging Face
* Stable Diffusion

## Project Description

For this project, we developed a text-to-image model able to generate Van Gogh style pictures based on text prompts provided by users. To this purpose, we exploited a pre-trained model of Stable Diffusion available in Hugging Face, which also hosts the “WikiArt” dataset we used for fine-tuning. This dataset includes 103,250 pieces of art, for which different features such as “title”, “artist”, and “style” are provided. However, in order to fine-tune our model, we considered a smaller dataset consisting of images and descriptions of more than 400 Van Gogh’s masterpieces only. For this reason, the synthetic images produced by the trained model are expected to recall the hand of the artist. To quantitatively evaluate our final model, we tested two different metrics for diffusion models: the CLIP score (28.89) and the Fréchet Inception Distance or FID (677.19). Also, we collected the opinion of 16 users, who were asked to test the model and assess the quality of the output images by assigning a score from 1 to 5 to the following criteria: relevance to the initial prompt (4.56 ± 0.7), Van Gogh style (3.94 ± 1.34), complexity (4.0 ± 0.87), creativity (4.0 ± 1.12), and general satisfaction (4.38 ± 0.78). These results confirm that our model behaves generally well although there is still space for further improvements.

## License

[MIT](https://choosealicense.com/licenses/mit/)
