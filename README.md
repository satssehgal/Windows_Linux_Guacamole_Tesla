# Windows_Linux_Guacamole_Tesla

In order to set this up i'm going to assume you have a kubernetes cluster either at home or on a remote server such as AWS/Azure/GCP etc, otherwise you can install apache guacamole directly on your computer with docker

In your kuberentes cluster we have to install a certificate issueing authority. Install all three le-* files in your cluster. This will put the lets encryptt certificate authority in your cluster.

You can test the certificate with the le-test scripts but since I know this works you can go directly to prod. Once done be sure to run the kubernetes file

Also ensure you port forward port 80 and 443 to your kubernetes load balancer
