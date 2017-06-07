# Guided-Neural-Style-Transfer
This project is a keras implementation using Tensorflow as backend that performs an alternative style transfer method. 
Our implementation differs from the original [(Gatys et al., 2015)](https://arxiv.org/abs/1508.06576), in that the semantics of the content image is not iterately being transfered onto the output by an optimization function. Instead, local information from the style image is being directly transfered over to the content image. This creates an more abstract output image where the local features from a the style image is more prominent. The code is inspired by [hnarayanan](https://github.com/hnarayanan/artistic-style-transfer), who have implemented the the original "Gatys et. al" style transfer method with keras with a Tensorflow backend. 

### Dependencies
There are some necessary dependencies you have to install for the program to run.
run `pip install -r requirements.txt` to install those through the terminal. 

Create a file called ~/.keras/keras.json and write the following in it:
 ``
   {
       "image_dim_ordering": "tf",
       "epsilon": 1e-07,
       "floatx": "float32",
       "backend": "tensorflow"
   }
   
`` The code can then be execute by typing `jupyter notebook` into the terminal

---

## Contributors

- Esben Winther Knudsen
- Malte Hølledig
- Sebastian Bach-Nielsen

---

## License & copyright

© Esben W. Knudsen, Aalborg University cph Medialogy

Licensed under the [MIT License](LICENSE).