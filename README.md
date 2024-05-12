deploy cluster role ,binding and datadog-rbac after that
Deploy both of them

Secure communication between node-based Agents and the Cluster Agent
The next step is to ensure that the Cluster Agent and node-based Agents can securely communicate with each other. The best way to do this is by creating a Kubernetes secret. To generate a token to include in the secret, run the following:

echo -n '<32_CHARACTER_LONG_STRING>' | base64




Copy the resulting string. Then, create a file, dca-secret.yaml, with the following:
After completeing all the dashboard will look like this
![image](https://github.com/Zenisis/datadog-eks/assets/119743135/6b834292-d3ee-4ba5-a087-dec92ae7a031)


https://www.datadoghq.com/blog/eks-monitoring-datadog/     #view this document for more refrence
