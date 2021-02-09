# Jumping into React, Node, MongoDB, and AWS S3

A simple web application that utilizes React, Node, and MongoDB that interacts with AWS S3 to store and create pre-signed URLs for uploaded objects. A simple proof-of-concept I worked up to introduce myself to the featured technologies.

The "nodeapi" directory contains the back-end API that interacts with MongoDB and S3 to store and retrieve objects. The "reactui" directory contains a React application that makes calls to the back-end to facilitate interactions with Mongo and S3.

This repo accompanies a blog post featured on my website.

https://www.ryanwendel.com/2021/02/09/jumping-into-react-node-mongodb-and-aws-s3/

The following is needed to prepare the API's environment.

```bash
mkdir nodeapi
cd nodeapi
npm init -y
npm install fastify --save
npm install fastify-multipart --save
npm install fastify-cors --save
npm install mongoose --save
npm install dotenv --save
npm install nodemon --save
npm install @aws-sdk/client-s3 --save
npm install @aws-sdk/s3-request-presigner --save
```

The following is needed to prepare the UI's environment.

```bash
npx create-react-app reactui
cd reactui
npm install axios --save
npm install dotenv --save
```
