# Image Filtering Microservice API Endpoint using AWS Elastic Beanstalk - A Cloud DevOps Project

Image filtering microservice that deploys with `Elastic Beanstalk`  on `AWS` to deploy a restful API endpoint that takes an image url as a query parameter and returns the filtered image.

## How the endpoint works
- The endpoint:
    - Validates the image_url query
    - Filters the image and applies grayscale transformation.
    - Sends the resulting file in the response
    - Deletes any files on the server on finish of the response.

This is part of a larger project that uses a `Node-Express` server to serve the API endpoint and a `Ionic` client to consume the API.

Backend application deployed on `AWS Elastic Beanstalk` using `EB CLI` (`eb init`, `eb create`, `eb deploy` ) and  `AWS CLI`.

API developed alongside Postman collection for testing and to prevent requests without valid authentication headers.

## Technologies used

- `Node.js`
- `Express`
- `Typescript`
- `AWS Elastic Beanstalk`
- `AWS CLI`
- `Postman`

### Endpoint URL (At the time of deployment)

<http://udagramfilterimage-env.eba-u5wp28wp.us-east-1.elasticbeanstalk.com>

## Deployment Screenshots
### Successful API Response of filtered image
![Successful API Response of filtered image](https://github.com/WafulaLukorito/Udagram/blob/master/deployment_screenshots/successful%20api%20response.png?raw=true "Successful API Response of filtered image")

### Succesful Deployment on AWS Elastic Beanstalk
![Succesful Deployment on AWS Elastic Beanstalk](https://github.com/WafulaLukorito/Udagram/blob/master/deployment_screenshots/udagram.png?raw=true "Succesful Deployment on AWS Elastic Beanstalk")
