# Provisioning Custom Samples Jahia 8.2
Inspired and forked from https://github.com/Jahia/provisioning-tutorials
Those are for saving **8.2.0** samples **(after the introduction of GraalVM and NPM modules in 8.2)**

Those are customisations of the initial Provisioning Tutorials
| Sample | Description |
| --- | --- |
| [01-jahia-mariadb-digitall](./01-jahia-mariadb-digitall/) | Jahia 8.2 with Maria DB and Digitall |
| [02-jahia-mariadb-digitall-local-provisioning-files](./02-jahia-mariadb-digitall-local-provisioning-files/) | the previous but with local provisioning files instead of online (with custom module installation)
| [03-jahia-mariadb-digitall-override-folder](./03-jahia-mariadb-digitall-override-folder/) | Example on how to override patches provisioning folder by a local folder [localMount](./03-jahia-mariadb-digitall-override-folder/localMount)
| [04-jahia-mariadb-luxe](./04-jahia-mariadb-luxe/) | This will create an environment with a website based on an NPM module
| [05-jahia-mariadb-empty](./05-jahia-mariadb-empty/) | This will create a Jahia 8.2 environment with no website


**Passwords and Tokens here are just for fun.**
- Here we use `9000` as exposed port and `WeLiveInATwilightWorld` as a root password
- Variables are set in every folder in the `.env` file of each case. Make sure to use different ones if you want to make a real world exposed use case.

## K8S custom local manifests
Kubernetes custom configuration manifests (to run those examples above) can be found in https://github.com/GladTek/jahia-k8s-provisioning