## Week 6: Logging and Monitoring

The intention of this week's mini-project was to add logging and tracing to a lambda function.

To begin this week's project, I began with the application I created in week 5. This application is relatively simple: to add an item to a database, add /{##} to the prod url.

See the following git repository for more information on the creation of the app.


## Configurations
First, I set up configurations on the lambda function.

![image1](img/log1.png)
![image2](img/setup1.png)

Navigating to the configuration tab under the lambda function, we can see that the monitoring configurations are set up. 

![image3](img/setup2.png)

## Logging

Navigating to cloudwatch -> log groups -> log group of interest, we can see that the logging for this lambda function is set up.   

![image3](img/log2.png)

Selecting the log stream of interest, we can see the logging of the different actions performed.

![image3](img/log3.png)

## Tracing with AWS X-Ray

First, confirm that permissions are set. 

![image4](img/xray1.png)

AWS X-Ray produces traces. The following are screenshots from these traces.

![image5](img/xray2.png)

![image6](img/xray3.png)

![image6](img/xray4.png)

## Cloudwatch

After connecting logging and AWS X-Ray to cloudwatch, I was able to produce a dashboard that outlines the logging and monitoring that I set up.

![image7](img/Cloudwatch1.png)
