# Wiki RPG Masterproject

In the following, theory and work progress are documented.

## Issues and questions
Issues | Urgency | Comments
------------ | ------------- | -------------
Why are there gray pixels in the masks? | high | Maybe my python script does not exactly do what it should, but basically it does just setting the blue pixels to black and the non-blue pixel to white. [Simon] <br /> solved with new program (double for loop, so not very efficient)

How can we set thresholds for the binary classification? | | I have just used 0.5. However I’m sure this should be addressed in a later step again. I have read the following in my tutorial for the unet: “This is normally done by optimizing the threshold on a holdout set.” - <br /> This is sort of what I did by plotting different scores as a function of the threshold (just quite roughly, only for this test dataset of 10 pictures).

What’s the role of the test set in the network? Why does our current network (UNet) not use the test set? | | The code from the website we used does only consider the training data, thus the test set is not used for validation. The goal would be that the trained network is tested with the (unseen) test data. [Simon] <br /> The Testset is added to the old network and can be used to evaluate the trained model

Why is the network’s output (i. e. the prediction) a RGB picture (and not a 1-dimensional picture)? | | matplotlib's pyplot is implemented that it uses per default a colormap for the imshow() function. By adding cmap='gray' in the imshow() function, a black/white mask will be displayed. [Simon] <br /> I have added the cmap=’gray’ for the mask images. Hence now we have a grayscale output




## Theory
- make description about NN architecture
- make description about performance evaluation metrics (Intersection over Union (IoU))

## Log file
#### Task distribution of week 3 (March 3, 2020)
- [x] Wiki einrichten + Log (Simon)
- [ ] Git Repo (Roger)
-> hist, modell ordner
- [ ] Python Script für Google API Anfrage (Alex)
-> Welche Daten werden abgespeichert? (Roger)
- [ ] Koordinatenverschiebungen überlegen (Simon)
- [ ] Datenspeicher (Roger)
- [ ] Netzwerkt trainieren mit neuen Images (Roger, Alex)
- [ ] Performance anpassen intersection over union (Jaccard) pro Klasse (Simon, Alex)

