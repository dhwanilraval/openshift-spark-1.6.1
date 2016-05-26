# Apache Spark images for OpenShift

# Build

Builds the image with Openshift and pushes it to the internal registry:<br/>
```oc create -f bc-spark-1-6-1.json```

# Template
Specify the image name the you created above as a variable:<br/>
```oc create -f template.yaml```

# Deploy
Ether go via the webconsole or by shell using:<br/>
```oc new-app --template=spark --param=SPARK_IMAGE=<IMAGE NAME> --param=WORKER_NAME=<generated if empty> --param=MASTER_NAME=<generated if empty>```
