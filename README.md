# GAN_stabilisation
AnoGAN dataset implementation
 Evaluation of the AnoGAN model proposed by Schlegl et al. (2017) on keras implementation of
 the model from tkwoo (2020) (which uses DCGAN models for generator and discriminator) is
 done on 3 different data sets. First, we use suggested data sets hand written digits mnist from
 keras data sets. Following that is Keras’ fashion mnist data set, which is slightly more complex
 than the handwritten digits mnist data set. However, because both of these data sets are in grey
 scale and have a size of 28X28, the latent vector dimension z was set to 10 and they were trained
 for only 10 epochs. Later, the model is evaluated on smoke free data set and because the model
 supports an input shape of (28,28,1), the images are resized and converted to grey scale using the
 openCV library, and the model is trained for 150 epochs.
 f or img in img_list :
 image = cv2. imread(os . path . join (path ,img) , 0)
 image = cv2. resize (image ,(28 ,28))
