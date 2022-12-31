<h1>Project Upload BackEnd: </h1>
<p align="center">

![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) ![Markdown](https://img.shields.io/badge/markdown-%23000000.svg?style=for-the-badge&logo=markdown&logoColor=white) ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white) ![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white) ![Insomnia](https://img.shields.io/badge/Insomnia-black?style=for-the-badge&logo=insomnia&logoColor=5849BE) ![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white) ![Yarn](https://img.shields.io/badge/yarn-%232C8EBB.svg?style=for-the-badge&logo=yarn&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)

> Status do Projeto: :heavy_check_mark: Finalizado

## Project description 

<p align="justify">
  This project aims to create an application capable of uploading files, either locally or directly to AWS S3.<br />
  The project is composed of two parts BackEnd and FrontEnd, you can clone the FrontEnd here.
</p>

 ## Prerequisites

  [Node](https://nodejs.org/en/download/)<br/>
  [MongoDB](https://hub.docker.com/_/mongo)<br/>
  [MongoDB Atlas](https://www.mongodb.com/try)<br/>
  [MongoDB Compass](https://www.mongodb.com/products/compass)<br/>
  [AWS S3](https://aws.amazon.com/pt/account/)<br/>
  [Yarn](https://classic.yarnpkg.com/lang/en/docs/install/#debian-stable)<br/>
  [Insomnia](https://insomnia.rest/download)<br/>

  ## Preparing local environment

  Before starting the App, you need to have MongoDB running on the machine, use Docker or MongoAltas.

  If you don't have MongoDB in your Docker, create a container using this command:

  ```
   docker run --name mongo -p 27017:27017 -d -t mongo
  ```
  To check if Mongo is running type the command:
  ```
   docker ps
  ```
  With the server running, access the URL: http://localhost:27017/ <br />
  If everything is correct, the following message will be displayed:
  ```
   It looks like you are trying to access MongoDB over HTTP on the native driver port.
  ```
  Open [MongoDB Compass](https://www.mongodb.com/products/compass), create the `upload` database and a `Post` collection.
  Create an .env file (you can use the .env-sample file as an example) and fill in the data according to the application.

  ```
  # If you host the application somewhere
  # enter host here:
  APP_URL=http://localhost:3000

  # s3: for production
  # local: for dev
  STORAGE_TYPE=local

  # Local machine address or Mongo Atlas
  MONGO_URL=mongodb://localhost:27017/upload

  # Data provided on the S3 AWS website
  BUCKET_NAME=
  AWS_ACCESS_KEY_ID=
  AWS_SECRET_ACCESS_KEY=
  AWS_DEFAULT_REGION=
  ```
  
  ## Starting the project:

  In the terminal, clone the project:
  ```
   git clone https://github.com/gilsonroberto/upload-backend.git
  ```
  Then enter the project directory:
  ```
   cd upload-backend
  ```
  Then install all project dependencies with:
  ```
   yarn install
  ```
  To run the project use the command:
  ```
   yarn dev
  ```
  ## Desenvolvedores/Contribuintes :octocat:

  [<img src="https://avatars.githubusercontent.com/u/30843584?v=4" width=115><br><sub>Gilson Roberto</sub>](https://github.com/gilsonroberto) 