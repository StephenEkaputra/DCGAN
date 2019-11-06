# DCGAN

Training GAN is difficult because we should adjust the model architecture to avoid from collapsing. We want the loss function keeps updating in every epoch. To train GAN celebA, we should have huge GPU memory to have big number of epochs (for example 100). As long as the loss function keeps updating and having big number of epochs, the output should be better.
