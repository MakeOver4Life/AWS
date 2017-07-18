# Cloudformation Structure

Other previous projects might have useful templates for reuse.

### AWS Managed Policies for Job Functions
http://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies_job-functions.html
Do not duplicate the above

### Per Environment

Production


NPE


### Policies required per environment



### Roles

BastionRole
ProductionAppRole
TestAppRole


### Role Policies

### Rollout Order:
Prod:
VPC - Name of stack: ProdVPC
Roles - Name of stack: Roles
SecurityGroups - Name of stack: SecurityGroups
Bastion - Name of stack: Bastion
JiraInstance - Name of stack: ProdJiraInstance
ConfluenceInstance - Name of stack ProdConfluenceInstance
ELB Name of stack: ProdELB (Choose Jira/Confl Targets)
RDS - Name of stack: ProdRDS
Route53 - Name of stack: Route53



### Resources


### Important Limits

Only Adminstrator or SystemAdministrator should be able to create/update/delete IAM policies
