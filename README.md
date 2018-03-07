# kick_tip
Trying to predict the outcome for a given football matchup using (statistical) learning methods.

##### Problem definition:
A set of football clubs defined as
![equation](http://latex.codecogs.com/gif.latex?C%3A%3D%5Cleft%20%5C%7B%20x%5Cin%20%5Cmathbb%7BR%7D%5E%7BN%7D%20%7C%5C%20x%20%5C%20%5Ctext%7Bgiven%20some%20specific%20time%7D%5C%20t%20%5C%20%5Ctext%7Brepresents%20the%20state%20of%20a%20club%20in%20respective%20football%20league%20%7D%20%5Cright%20%5C%7D) is given. 
For any tuple ![equation](http://latex.codecogs.com/gif.latex?%28x%2Cy%29%5Cin%20C%5E2) the outcome is encoded as ![equation](http://latex.codecogs.com/gif.latex?f%28x%2Cy%29%5Cin%20%5B0%2C1%5D) where 0 indicates a strong tendency
in favor of x and vice versa.
The mapping that is to be learned is defined as
![equation](http://latex.codecogs.com/gif.latex?f_%5Ctheta%3A%20C%5E2%20%5Crightarrow%20%5B0%2C1%5D%20%2C%20%28x%2Cy%29%20%5Cmapsto%20o), where theta is the parameter of the function that is being "learned" and o is the outcome as described above.
Goal is then to optimize the function f so that the error on the training data is minimized and the model is able to generalize to unseen data.

###### Possible strong features that may be interesting to extract:
Clubprestige (e.g. a value that represents the 'prestige' of a club based on (performance) history in the respective league),
relative Clubstrength (e.g. a value that represents a conclusion on past encounters within a certain matchup),
Playerstrength (e.g. a value that represents the current squad), etc.

## To-Do's:
List of things that need to be done:
* Check on available literature i.e., related work
    * [Ulmer et al. on Premier League Predictions using AI & ML](http://cs229.stanford.edu/proj2014/Ben%20Ulmer,%20Matt%20Fernandez,%20Predicting%20Soccer%20Results%20in%20the%20English%20Premier%20League.pdf)
    * [Pettersson on using RNN for Football Match Prediction](http://publications.lib.chalmers.se/records/fulltext/250411/250411.pdf)  
    * [Silfwer on his attempt of doing the same and collecting data over 2 years](https://doctorspin.me/digital-strategy/machine-learning/)
    * [Raval YT Video on Football Match Prediction with Deep Learning](https://www.youtube.com/watch?v=6tQhoUuQrOw)
* Collect data (write some script to automatically extract information from specific sites to some form of database)
* Future: Feature-Extraction & Preprocessing, Devlop/Train/Evaluate some model

#### Additional remarks
This repo is created simply out of fun, trying to take the things one has learned in the past by taking classes and
getting to know and love learning methods and apply them on some real life application that is cool (rather
than in the context of academia-only). My friend Bilal came up with the idea, so I created this repo for us to 
manage things in one place cleanly. Robin is also involved though sceptical, I hope that we may find/take the time
to try this out (at least if we don't get rich we gain some experiences and insights by doing it anyways haha).