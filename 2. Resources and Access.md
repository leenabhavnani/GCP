### Notes

##### Google Cloud’s resource hierarchy
- It contains four levels, and starting from the bottom up they are:
  - resources
  - projects
  - folders
  - an organization node
- Policies can be defined at the project, folder, and organization node levels. Some Google Cloud services allow policies to be applied to individual resources, too
- Policies are also inherited downward
- Projects are the basis for enabling and using Google Cloud services
  - Each project is a separate entity
  - Each resource belongs to exactly one project.
  - Projects can have different owners and users because they’re billed and managed separately
  - Project has three identifying attributes: a project ID(unique and immutable), a project name, and a project number ( used internally by Google Cloud).
- Google Cloud’s Resource Manager tool is designed to programmatically help you manage projects
- A folder can contain projects, other folders, or a combination of both.
- if you have two different projects that are administered by the same team, you can put policies into a common folder so they have the same permissions.

##### IAM
- The “who” part of an IAM policy can be a Google account, a Google group, a service account, or a Cloud Identity domain. A “who” is also called a “principal.”
- The “can do what” part of an IAM policy is defined by a role. An IAM role is a collection of permissions.
- You can define deny rules that prevent certain principals from using certain permissions, regardless of the roles they're granted.
- There are three kinds of roles in IAM: basic, predefined, and custom.
- Basic roles include owner, editor, viewer, and billing administrator.
- Specific Google Cloud services offer sets of predefined roles, and they even define where those roles can be applied.
- Custom roles will allow you to define “least-privilege” model permissions.
- Custom roles can only be applied to either the project level or organization level. They can’t be applied to the folder level.
  
##### Service Accounts
-  if you want to give permissions to a Compute Engine virtual machine, rather than to a person? Well, that’s what service accounts are for.
-  Service accounts are named with an email address, but instead of passwords they use cryptographic keys to access resources.
-  With a tool called Cloud Identity, organizations can define policies and manage their users and groups using the Google Admin Console.

##### Google Cloud
- There are four ways to access and interact with Google Cloud.
- The Cloud Console, the Cloud SDK and Cloud Shell, the APIs, and the Cloud Console Mobile App.
