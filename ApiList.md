# DevTinder API Documentation

auth Router

 -POST/signup
 -POST/login
 -POST/logout

Profile Router
 -GET/profile/view
 -PATCH/profile/edit
 -PATCH/profile/forgot-password
 -DELETE/profile/delete

Connection Request Router
 Status: ignore,interested,accepted,rejected
 # Send Connections
 -POST/request/send/:status/:userId         // Status is dynamic    [interested,ignored]
 
 # Review Connections           
 -POST/request/review/:status/:requestId        // Status is dynamic [accepted,rejected]


User Router
 -GET/user/connections
 -GET/user/request/received
 # Feed
 -GET/user/feed - get all the profiles of others for you