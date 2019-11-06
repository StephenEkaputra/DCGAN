# DCGAN

We use 1 GPU to train with batch size of 128 and epoch number of 50. It means that in 1 epoch we need to train with 1,583 (202,599 / 128 = 1,583) batches. We use 128 batch size to make the training faster converge. But, however we stopped at epoch 20 because out of memory. So, this is the longest and best GAN training, the author has ever done in terms of less memory GPU computer. The solution is we reduce the size of image data to 32x32 pixel to make the epoch longer.
We use Adam optimizer as optimization to both models (generator and discriminator) because when we use SGD, the loss function stop updating. We set the learning rate to 0.0002, beta 1 to 0.5, and beta 2 to 0.999, respectively. The updating loss function can be seen from the image below.


Training GAN is difficult because we should adjust the model architecture to avoid from collapsing. We want the loss function keeps updating in every epoch. To train GAN celebA, we should have huge GPU memory to have big number of epochs (for example 100). As long as the loss function keeps updating and having big number of epochs, the output should be better.
