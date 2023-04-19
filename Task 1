
## Onboarding

### Objective:

- Able to log in and navigate around the Tenable Cloud Security (Tenable.cs) dashboard
- Able to create a Tenable Cloud Security (Tenable.cs) project(s)
- Able to identify policies assigned to a project.
- Able to create and store API keys into AWS Secrets Manager
- Able to run a Cloud Formation Template



### Prerequisites
-  Skills:
  - [ ] Prior knowledge of AWS Dashboard
	- [ ] Basic Knowledge for Cloud Formation Stacks
  - [ ] Prior knowledge of networking, Remote Desktop Connection to Microsoft Windows. <sup>Note:  if not using local laptop</sup>

### Resources
- Tenable account (assigned by instructor)
- Access to https://cloud.tenable.com/
- Access to Tenable Documentation https://docs.tenable.com/Tenablecs.htm
- Credentials to Windows Desktop are in the Output Properties <sup>Note:  if not using the local laptop<sup>

### Tasks

#### Navigate to the environment
***Use if not using local laptop for connectivity, otherwise skip to the next section***

1. Remote Desktop Protocol (RDP) – use Remote Desktop connection to login into the external IP using your preferred client (i.e. Microsoft Remote Desktop)

    1.  You will need to navigate to the sign-in page

        1. Use the Google Chrome to navigate to Tenable sign-in page,
	        - There's bookmark in Chrome or shortcut on the Bastion host's Windows Desktop,
    	    - Use Tenable.cs credentials assigned by the class instructor,
        1. You're in *Tenable.io Workspace* page,
        1. `Click` the icon to open **Tenable.cs**,

#####  Create an API key 

The API key is used as an authetication key to verify validation questions using Tenable's REST API.  More information in using Tenable API keys can be found at https://developer.tenable.com/ (Search for the Cloud Security section for API examples)

1.  From Tenable Cloud Security (Tenable.cs) dashbord, `Click`on the **Integrations** icon from the left menu,
1.  `Click` on **API Tokens**,
1.  `Click` on the ***Click to generate an API Token,
1.  The new token will be added to the bottom of the list.  `Click` on the <u>copy</u> icon to `Save` the token to the clipboard.  

##### Store API key 
A cloud formation template will be used to store the API key in secrets manager.

1.  Navigate to AWS Console,
1.  Select the **CloudFormation** service,
1.  Click on **Create Stack->with New resources (standard)**,
	  - Select **Template is Ready** ,
    - Select **Amazon S3 URL**,
    - From **Output Properties**, `Copy` the link from the parameters,<u>**StoreAPI**</u>.
1.	Click on **Next**,
1.  In the window **Specify stack details:  
    1.  Enter the Stack name:  <u>**TenableStoreAPIkey**</u>,
    1.  Enter the **ApiKey** (found in the steps above),
    (ie Copy the key from **TenableCS Dashboard->Integrations->Create API Key**),
1.  `Click` **Next**,
1.  `Click` **Next**,
1.  `Click` **Submit**,
1.  `Click` the refresh button to verify the status **CREATE_COMPLETE**.


##### Create a Project
**A Project** is a group of any combination of connections, policies, cloud accounts:
1.  From the Tenable Cloud Security dashboard, click on the (+) button on the top-left menu  ,
1.  `Click` on **Create a Project**,
1.  Provide a ***Project Name*** (ie. **Lab01-Project**), then click ***Continue***,
1.  `Choose` **AWS** as the provider.

##### Verify the Assigned Policies
Project dialog box is used to view options and configurations assigned to a Project.  (ie, **Project ID**, repositories, cloud accounts, K8 clusters, Active Policy groups, Alerts, excluded resources, excluded drifts, change history)

From the Tenable Cloud Security Dashboard
- `Click` on the **Projects and Connections** tab,
- `Click` on the Project you created	,
- On the pop-up, look for the Active Policy Group,
- `Click` on the ***pencil*** icon.


#### VALIDATION QUESTION

1.  Enter the *Project ID* for the project created in this lesson?

#### END OF LAB