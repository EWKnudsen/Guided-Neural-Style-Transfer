# Guided Neural Style Transfer
This project is a Keras implementation using Tensorflow as backend that performs an alternative style transfer method. Our implementation differs from the original ([Gatys et al., 2015](https://arxiv.org/abs/1508.06576)), in that the semantics of the content image is not iteratively being transferred onto the output by an optimization function. Instead, local information from the style image is being directly transferred over to the content image. This creates a different output image where the unwanted local features that comes with the content image transformation is being iteratively removed, making style image features more salient. The code is inspired by [hnarayanan](https://github.com/hnarayanan/artistic-style-transfer), who have implemented the original "Gatys et. al" style transfer method with keras and Tensorflow as backend.

### Dependencies
There are some necessary dependencies you have to install for the program to run.
run `pip install -r requirements.txt` in the terminal to install those. 

Create a file called ~/.keras/keras.json and write the following in it:
 
````
   {
       "image_dim_ordering": "tf",
       "epsilon": 1e-07,
       "floatx": "float32",
       "backend": "tensorflow"
   }
````
The code can then be execute by running `jupyter notebook` in the terminal

---

## Contributors

- Esben Winther Knudsen
- Malte Hølledig
- Sebastian Bach-Nielsen

---

## License & copyright

© Esben W. Knudsen, Aalborg University cph Medialogy

Licensed under the [MIT License](LICENSE).