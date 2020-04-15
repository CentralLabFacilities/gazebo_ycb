# Gazebo YCB Objects 

SDF files of the [The YCB Object and Model Set](http://ycb-benchmarks.s3-website-us-east-1.amazonaws.com/)

## Usage

Add the model folder to `GAZEBO_MODEL_PATH` environment.

e.g. add the following to your gazebo launchfile:

```
<env name="GAZEBO_MODEL_PATH" value="$(find gazebo_ycb)/models:$(optenv GAZEBO_MODEL_PATH)"/>
```

## Attribution

All files under `models/*/[materials/meshes]` attributed to the
[The YCB Object and Model Set](http://ycb-benchmarks.s3-website-us-east-1.amazonaws.com/). Please see
`LICENSE_YCB` for more information.
