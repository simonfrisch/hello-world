# Wiki RPG Masterproject

In the following, theory and work progress are documented.

## Issues and questions
Issues | Urgency | Comments
------------ | ------------- | -------------
Why are there gray pixels in the masks? | high | Maybe my python script does not exactly do what it should, but basically it does just setting the blue pixels to black and the non-blue pixel to white. [Simon] \n solved with new program (double for loop, so not very efficient)
How can we set thresholds for the binary classification? | | I have just used 0.5. However I’m sure this should be addressed in a later step again. I have read the following in my tutorial for the unet: “This is normally done by optimizing the threshold on a holdout set.” - This is sort of what I did by plotting different scores as a function of the threshold (just quite roughly, only for this test dataset of 10 pictures).

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

