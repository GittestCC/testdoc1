---
title: Deployment
---

## What is Deployment?
 Deployments are tailored back-end features packages, ready to be consumed by your clients.

They are composed of KintoBlocks with unique configuration parameters, and either a client or a protocol to allow your
clients to talk to the deployment. You can deploy your app in a specific environment and have several environment for 
one deployment to apply different custom configuration.

## How to Create a Deployment?

1. Select deployment from the sidebar.

2. Click on **Create new deployment**.

    ![Screenshot](/docs/assets/01.png)

3. Enter the reqired details `Deployment Name` , `Description(optional)` and `Environment name`.

    ![Screenshot](/docs/assets/02.png)

    > Note: Give a unique name for the **Deployment name**.

4. Enable **Automatically deploy toggle** and add kintoblocks.

5. Click on **Create New Deployment**.

    ![Screenshot](/docs/assets/03.png)

6. Check for the status & history.

7. Copy the secret key to get a token.
    
     ```
    curl -H "Content-Type: application/json" -X POST -d
    '{"clientId":"466026ce01964537ad0627b953356ce8","clientSecret":"YveH2V0KycIk"}' 
        https://api.staging.kintohub.com/authorize
    ```

8. Open git bash and paste the api code.

    ![Screenshot](/docs/assets/10.png)

9. Copy the **Access your api** and Replace 
- `token`
- `kintoblock` 
- `endpoint`
    
     ```
        curl -H "Kinto-Authorization: Bearer <token>" https://api.staging.kintohub.com/<KintoBlock>/<endpoint>
    ```

### Refer [click here](https://docs.kintohub.com/docs/kintoapps)
 
[About Deployment status](deployment-status-history.md)
