# LAB 17 - Class 401d48

## Project:  AWS: S3 and Lambda (images)

### Author: Junyoung Son

### Problem Domain  

- Create an S3 Bucket with “open” read permissions, so that anyone can see the images/files in their browser
- A user should be able to upload an image at any size, and update a dictionary of all images that have been uploaded so far
- When an image is uploaded to your S3 bucket, it should trigger a Lambda function which must:
    - Download a file called “images.json” from the S3 Bucket if it exists
    - The images.json should be an array of objects, each representing an image. Create an empty array if this file is not present
    - Create a metadata object describing the image
        - Name, Size, Type, etc.
- Append the data for this image to the array
- Note: If the image is a duplicate name, update the object in the array, don’t just add it
- Upload the images.json file back to the S3 bucket

### Links and Resources

- [GUI DEPLOY](http://lab16-env.eba-fz3iirss.us-west-2.elasticbeanstalk.com/) (http://lab16-env.eba-fz3iirss.us-west-2.elasticbeanstalk.com/)
- [CLI DEPLOY](http://lab16-env.eba-fz3iirss.us-west-2.elasticbeanstalk.com/) (http://lab16-env.eba-fz3iirss.us-west-2.elasticbeanstalk.com/)
<!-- - [front-end application](http://xyz.com) (when applicable) -->

### Setup

  npm i express
  AWS - Elastic Beanstalk - New Application
  ZIP index & package.json file

#### `.env` requirements (where applicable)

- `PORT` - 3002
- `DATABASE_URL` - URL to the running Postgres instance/db

#### How to initialize/run your application (where applicable)

npm commands:
- `npm start`
- `npm i express`

eb commands:
- eb init
- eb create
- eb deploy
- eb open

#### How to use your library (where applicable)

#### Features / Routes

- Feature One: Details of feature
- GET : `/hello` - specific route to hit

#### Tests

- How do you run tests?
- Any tests of note?
- Describe any tests that you did not complete, skipped, etc

#### ![UML]()
