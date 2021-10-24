# Udagram Image Filtering Microservice
The project consists of:
A microservice to filter images.
A url image has to be provided in the query params image_url

### Code repository
### Run in local
1. Initialize a new project: `npm i`
2. run the development server with `npm run dev`
### Project deployed to AWS Beanstalk following the next commands:
1. eb init
2. npm run build
3. eb create
4. eb deploy (In order to push changes to the application)
### System deployed
Please visit http://image-filter-jared-zena.us-east-1.elasticbeanstalk.com/filteredimage/?image_url=https://i.postimg.cc/C12BqfZC/Screen-Shot-2021-10-24-at-6-11-37-PM.png
To see a example of image filtered (Cat image to another URL in order to make it work).

Please note that not passing a url will return a 400 (Bad request) http code
http://image-filter-jared-zena.us-east-1.elasticbeanstalk.com/filteredimage?image_url=