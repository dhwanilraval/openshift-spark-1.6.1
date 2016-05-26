# Apache Spark images for OpenShift

# Build

Builds the image with Openshift and pushes it to the internal registry:
```oc create -f bc-spark-1-6-1.json```

# Template
Specify the image name the you created above as a variable
```oc create -f template.yaml```
