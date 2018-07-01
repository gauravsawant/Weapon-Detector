# Weapon Detector

## The Steps Invloved:

1. Train the tiny-yolo network in darknet library creating tiny-yolo-gun_6900.weights.
2. Convert the trained model using darkflow library into tensorflow tiny-yolo-gun.pb representation.
3. Reconstruct the network in tensorflow and import weights by loading tiny-yolo-gun.pb.
4. Optimize the loaded model for inference on mobile creating tiny-yolo-gun_inference.pb.
5. Load the optimized model into the Andriod App and compile.

## Dataset Notes:

The data set is a Combination of two dataset one unnamed and other Core50
The annotations for the dataset are generated manually.
Currently the dataset only consist of pistols and empty or everyday-object hands.
Futher improvement in dataset can be addition of weapons and knives.

## Inference App:

It uses camera of smartphone as input to the model and runs inference on it.
As it is a higly optimized model it has around 5-10% inconsistency.
The inconsistency can be eliminated in future on server side by running a fully accurate model on server.
