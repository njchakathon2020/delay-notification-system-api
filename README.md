# delay-notification-system-api

## About the project 

delay-notification-system-api is implemented using Mule 4.
This system api is used to add and retrieve data from/to database related to Train delay services.
It is used by Notification process api for sending service information to users via email.

## List of Endpoints:

- Get Locations

    http://delay-notification-system-api.us-e2.cloudhub.io/api/users/locations?notificationRangeMins=100

      This method is used to retreive qualifying source and destination locations that need to be checked for delay at the moment
      
- Get Users

    http://delay-notification-system-api.us-e2.cloudhub.io/api/users?sourceLocationCode=BSK&destinationLocationCode=WAT

      This is a get request and endpoint will fetch the list of users from the database
      
- Get subscription by UserID  

    http://delay-notification-system-api.us-e2.cloudhub.io/users/{userId}/subscriptions?sourceLocationCode=BSK&destinationLocationCode=WAT

      This is a get request and this endpoint fetch the users who have subscriptions based on userID
    
