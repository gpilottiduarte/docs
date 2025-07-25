## Metadata_Start 
## code: en
## title: How to integrate DSM with Jenkins 
## slug: how-to-integrate-dsm-with-jenkins 
## seoTitle: How to integrate DSM with Jenkins 
## description:  
## contentType: Markdown 
## Metadata_End
## About Jenkins and integration with DSM CLI

Jenkins has a feature that allows environment variables to be set during job execution and stored safely for later use. However, administrators must ensure that these variables are rotated regularly without interrupting the DevOps pipeline.

Segura DSM has a Jenkins plugin that uses the platform's native architecture to set environment variables during pipeline runtime. This plugin also sends all the variables available in the working environment to Segura DSM to discover any sensitive data that is running unnoticed, helping system administrators to have greater control over their systems.

The image below shows a diagram of how DSM and Jenkins are integrated:

![Jenkins integration with Segura DSM](https://cdn.document360.io/5a1d58df-64ce-42a2-8b23-688477d32f33/Images/Documentation/image-FAFE2PUS.png)

## Integrate DSM with Jenkins

Segura DSM provides a native integration so that Jenkins jobs can fetch secrets directly from Segura, thus providing an easy way to configure secret injection.

To install the Segura Jenkins integration using the `.hpi` file, follow the steps below:

1. Access your Jenkins instance.
2. On the homepage, click the **Manage Jenkins** option in the side menu.
3. Click the **Manage Plugins** option.
4. On the **Advanced tab**, in the **Upload Plugin** section, click the **Upload button** and upload the `.hpi` file.
5. To complete the installation, restart Jenkins.

:::(error) (Attention)

* The integration of Segura with Jenkins is only available for Jenkins 2.235.1 or more recent versions.
* Ensure you select OAuth 2.0 as the authentication method in Segura DSM, as the plugin uses it to fetch information.

:::

## Configure integration with Jenkins

Once the plugin is installed, follow the instructions below:

1. Create a new job or select an existing one.
2. In the side menu, click on **Configure**.
3. Scroll to the **Build Environment** section and select the **Segura** **DSM Plugin** checkbox.
4. In the **Segura URL** field, enter the URL used to access the Segura instance.
5. Click the **Add** button to create a new Jenkins credential.
6. In the open window, select **Segura Auth Credential**.
7. Fill in the **Client ID** and **Client Secret** fields with the data provided by DSM.
8. Optionally, provide an ID and a description and click the **Add** button.
9. In the **Segura** **Auth Credential** field, select the credential created in the previous step.

## Inject secrets using Jenkins

After setting up the integration in the project, go to the **Build Now** menu to run the pipeline and use the secrets. When the job is finished, click **Job ID > Console** to display the execution result.

The execution result will look like the one below:

```bash
Started by user XXXX
Running as SYSTEM
Building in workspace /var/Lib/jenkins/workspace/DSM
Sending all enviroment variables to Seguras' server
API status code is 200
For sending vars: Segura returned à successfull responde with code 200
Getting all Seguras' secrets and storing it as environment variables
API status code is 200
For getting vars: Segura returned a successfull responde with code 200
Analyzing returned variables from Secret 13
Saving variable PASSWD with value ****
Saving variable additional_information with value ****
Saving variable aliases with value ****
Saving variable SECRET_ACCESS_KEY with value ****
Saving variable PORT with value ****
Saving variable ip with value ****
Saving variable HOST with value ****
Saving variable ACCESS_KEY_ID with value ****
Saving variable USER with value ****
Saving variable TTL with value ****
[DsM] $ /bin/sh -xe /tmp/jenkins14979126717851661906.sh

```

---

Do you still have questions? Reach out to the [Segura Community](https://community.Segura.io/).