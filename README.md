# welcome on the kubewatch.io deployment repository

You will find here the different ways you have to deploy our pod.
The main advantage to scan from your cluster vs from the platform are:

1. No secrets or access token from your cloud provider are required.
2. Only inventory information is sent to the platform
3. You can access internal services for fingerprint, SSL/TLS checks and App scanning.

To deploy your pod, you will find here the following templates:

1. kubectl command in k8s-deployment
2. helm deployment charts in the versionned directories

Feel free to send your feedback on our support at kubewatch.io email or join us on our slack workspace kubewatchio

-- The kubewatch.io team