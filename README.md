# sprint-branch-create
Azure Pipeline YAML for creating a new sprint branch, set it as the default branch and apply branch policies

## Requirements
Before running the code you will need to do the following:
1. The 'Project Collection Build Service' service account in the Azure DevOps project where the code will run needs to have certain permissions. Otherwise when the code is run in a pipeline it will throw a permissions error. In project settings -> Repository -> Security set 'Create branch', 'Edit policies' and 'Contribute' to Allow for Project Collection Build Service. 
2. Create a Azure Resource Manager service connection. Go to project settings -> Service connections. Click on New service connection. Choose Azure Resource Manager and click Next. Choose service principal (automatic). Give the service connection a name. Select subscription. Leave resource group field blank. Make sure the 'Grant access permissions to all pipelines' checkbox is selected. Click Save.
