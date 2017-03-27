This project is meant to be snippets for understanding the TFRecord and Pipeline concepts in Tensorflow.

1) FifoQueue.ipnb - create a fifo queue and read in

2) shuffle_batch.ipynb - same thing, but reading with shuffling

3) TFRecordReading.ipynb - same thing, but instead of generating "fake data," we read it from a file of TFRecords representing spectrograms (2D grayscale images)
	It imports the spectreader module also found in this directory.
    Note: before running this, the TFRecord files must be created in the data directory using the runcmd found there.

===========

/data

train and validate are directories with labeled subdirectories, each containing a collection of data files (spectrograms in the tif image format)

spect2TFRecords.py reads the data files and creates two files of TFRecords, one for the training data, one for the validate data. 

tiffspect.py isn't currently used.

Copy the runcmd text to the command line to create the TFRecord files from data
