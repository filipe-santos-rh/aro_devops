# aro_devops
This repo will be used to test automation from AzureDevOps to an ARO cluster  


### Create Project

#### Prerequisites:  

You will need to have a token from a User or Service Account that does have the capabilities to create Project, Groups, Assign permissions to users and groups.  

#### what will be created:  

This pipeline  will complete the following tasks:  
- Create a new project  
- Create 2 groups with the naming convention of **projectName-view** and **projectName-admin**  
- Grant permissions view to the group **projectName-view** to the project created  
- Grant permission admin to the group **projectName-admin** to the project created  
- Create a service account with the naming convention of **projectName-sa**
- Grant permission admin to the service account **projectName-sa** to the project created  


#### Variables:  

The following variables will be needed to execute the pipeline:  
- **apiUrl** 
This variable should be the api url to connect to you openshift cluster.   
- **sa_token** 
This variable should be the token used to connect to your openshift cluster.  
- **project_name** 
The name of the project that should be created.    

