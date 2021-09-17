# Steps:

Setup required at AWS Cloud
1. We need to create terraform code for IAM role with assume role category.
2. Create a policy to access cloudfront
3. Attach the policy with role
4. Generate the Role ARN

Setup required at Kubernetes end

1. The Kubernetes cluster will be hosted on premise network.
2. Services will be deployed on the Kubernetes cluster
3. In the annotations section of the application pod we need to provide the role ARN

How the connection will be establised between Kubernetes on-premise with AWS cloudfront
Using AWS direct connect.

Please check architecure diagram attached for end-to-end process.
