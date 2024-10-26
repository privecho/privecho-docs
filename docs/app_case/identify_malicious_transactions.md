## Requirements

Financial institutions monitor trading activities to identify and prevent fraudulent behavior. These transaction data often contain sensitive personal information, such as account numbers, transaction amounts, and user identities.

## Prerequisites

- Anomaly transaction monitoring AI model component has been registered with the verifiable AI model execution layer.

- FHE (Fully Homomorphic Encryption) component has been registered with the privacy computing execution layer.

- Idle computing resources are available for scheduling by the computing power scheduling layer.

## PrivEcho

### Input

FHE encrypted transaction information

### Output

Anomalous trading activities

### Execution Process

1. Financial institutions prepay tokens for computation and storage fees.

2. Financial institutions use the FHE component to create a public-private key pair and encrypt sensitive data using the public key.

3. The gateway layer forwards the received ciphertext and task information from FHE.

4. The preprocessing layer performs some preliminary operations, such as authentication, intent analysis, and information forwarding; among these, intent analysis converts requirements into a demand structure recognizable by the scheduling layer.

5. The scheduling execution layer begins work:

   - The computing power scheduling layer selects scheduled computing resources based on computational costs and allocates resources to this task.

   - The privacy computing module verifies data legality, such as whether it meets privacy-computputing data requirements.

   - The verifiable AI model layer executes computations and outputs results along with corresponding proofs.

6. The post-processing layer conducts preprocessing before returning results, such as analyzing whether results are legitimate or if there is any sensitive data that needs verification.

7. Results and proofs are returned to financial institutions for use or further analysis.