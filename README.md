# AI-Image-Caption-Bot
A deep learning based web app to predict the caption of an image. The features of images were extracted using Transfer Learning with help of Resnet-50 model and the features of text were extracted using embedded matrix (from glove.6B.50d). The text was fed to embedded layer and then LSTM model(RNN) . Both the images and text model were fed to a decoder i.e. feed forwarding neural network(ANN) with softmax activation to predict probability of each word in embedded matrix and the highest probability word could be fed again to LSTM as sequential partial caption (although in training set we fed the ground truth always to predict the next word).

The dataset used for training was Flickr 8k dataset : https://www.kaggle.com/shadabhussain/flickr8k

The bot is useful -

For blind people (Visual aid) - As it could help them by converting the text into audio and give them a representation about their surroundings.
Google Lens - This concept can be seen in Google lens too.
Automatic surveillance (CCTVs) - Notify when a suspicious activity is caught.
