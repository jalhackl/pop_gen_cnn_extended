# pop_gen_cnn_extended

This repository contains a pytorch and a tensorflow reimplementation of the introgression analysis in https://github.com/flag0010/pop_gen_cnn/tree/master/introgression.
The training and validation/test data were downloaded from https://conservancy.umn.edu/bitstream/handle/11299/198335/big_sim.npz

The  .npz-file must be extracted and the containing four .npy-files (xtrain, xtest, ytrain, ytest) be stored in the data folder (to be created within the main folder).

Both jupyter notebooks do the training, store the obtained model and evaluate the model on the test set (accuracy and confusion matrix).

In contrast to the original implementation, data is loaded via a dataloader so that it is not necessary that the complete files are loaded into memory.
