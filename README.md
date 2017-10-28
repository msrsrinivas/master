# master
Existing functionality:

 The As Is functionality of the application is to query the Google directory API, in order to recursively fetch all group members mail id's as well as subgroup members for a given group email. 

In order to consume the Google directory API, service account is used to fetch the member details with the highest privileges but, it is touching the sensitive information.

2. New Requirement:

To be functionality is not to use the service account for pulling the group member information is not recommended because it is touching the all sensitive information of the group members as it will have the super admin rights. So this is not ideal.
The new approach will not open up any sensitive information of users within google group. Service account has more access than only API access. It has access to other resources and APIs. Using this approach, we can restrict the access of user limited to single API.

