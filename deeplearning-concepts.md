# Deep learning concepts

### Fundamental equation

```txt
ŷ = log(x1w1 + x2w2)
```
`ŷ` is the predictive value of Y. `log` is a place holder for any non-linear function.`x1 and x2` are inputs, for example hours studied when calculating chance that student will pass. `w1 and w2` are weightings behind inputs, for example hours studied would have heavy weighting.

### (ANN) Artificial Neural Networks

`ANNs` essentially comprise of bricks of this fundamental equation. Think of each of the circles in the middle as the bricks and the ends, the input and output.

**Image grabbed from https://miro.medium.com/v2/resize:fit:1400/1*Gh5PS4R_A5drl5ebd_gNrg@2x.png**

![Image couldn't load](https://miro.medium.com/v2/resize:fit:1400/1*Gh5PS4R_A5drl5ebd_gNrg@2x.png "ANN Visualization")

### Forward propagation & Backwards propagation

Take this example equation:

```txt
ŷ = x1w1 + x2w2
```
Where `x1` is how many litres of water drank the day before exam, and `x2` is hours studied before exam(x1 and x2 both have their attached weighting, and lastly `y hat` is the predictive measure if the student passed. In `Forward Propagation`, we are telling the model to take the exam. In `Backwards Propagation OR backprop`, we are telling the model to change the weightings depending on the negative feedback which in this case is if the student passed or failed. For example look at the above graphic, in `backprop`, the red circle would tell the green circles that the output is wrong, the green circles fix what they can and then tell the blue circles that something is wrong we got the wrong output and so on and so fourth.
