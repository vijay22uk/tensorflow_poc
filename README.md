# tensorflow POC
## Image classification
## In an given avengers poster it will find actors(RDJr:Iron man, captain america .... ) in it; 

tensorflow pocs with docker

# install tensorflow docker
### docker run -it gcr.io/tensorflow/tensorflow:latest-devel
### cd ~/tensorflow 
### this is a git repo of tensorflow source code
##### git pull 

### save docker image changes
#### docker commit <dockerId> <name: tensorflowdocker>
## Prepare images
#### link it to docker  docker run -it -v $HOME/tf_files:/avengers 
  
###### python tensorflow/examples/image_retraining/retrain.py \
###### --bottleneck_dir=/tf_files/bottlenecks \
###### --how_many_training_steps 4000 \
###### --model_dir=/tf_files/inception \
###### --output_graph=/avengers/retrained_graph.pb \
###### --output_labels=/avengers/retrained_labels.txt \
###### --image_dir /avengers

