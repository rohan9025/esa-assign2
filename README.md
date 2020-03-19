


# Esa-Assign2

The project basically is creating a simple online shopping cart platform int the form of microservices linked via apis made in Node.Js. The major roles are the products available and the user interacting with the microservices. 

This project has two microservices. The first microservice interacts with the user (assuming they have logged in and are valid users). The second microservice interacts with the people running the e-commerce site. They can add/update inventory as per the available stock.

## Getting Started

Download/fork+clone the folder esa-assign2. It will have a folder(api try) and two python scripts.

## Basic api structure

DATABASES:<br>
1) User<br>
2) Products<br>
3) Cart<br>

PROJECTS:<br>
1) controllers <br>
2) routes <br>
3) models <br>

a server.js file to set up and run the server

```
~esa-assign2>tree --filelimit 6
.
├── api try
│   ├── api
│   │   ├── controllers
│   │   │   ├── cartController.js
│   │   │   ├── productController.js
│   │   │   └── userController.js
│   │   ├── model
│   │   │   ├── cartModel.js
│   │   │   ├── productModel.js
│   │   │   └── userModel.js
│   │   └── routes
│   │       ├── cartRoutes.js
│   │       ├── productRoutes.js
│   │       └── userRoutes.js
│   ├── node_modules [214 entries exceeds filelimit, not opening dir]
│   ├── package-lock.json
│   ├── package.json
│   └── server.js
└── UserMicroservice.py

6 directories, 13 files
```


## Setting up

The node js code is designed to run on a mongodb atlas server. Please head to the server.js file and add a connection string to connect to a mongo database.


### Installing

A step by step series of examples that tell you how to get the server and client running

Running the server

```
~esa-assign2/api-try>npm start
```


Output :

```
> api-try@1.0.0 start ~\esa-assign2\api try
> nodemon server.js

[nodemon] 2.0.2
[nodemon] to restart at any time, enter `rs`
[nodemon] watching dir(s): *.*
[nodemon] watching extensions: js,mjs,json
[nodemon] starting `node server.js`
todo list RESTful API server started on: 4000

```

Running the userMicroservice code -essentially acts as a client to the api

```
~esa-assign2/>python userMicroservice.py
```
Note: the microservice files have their own instructions within the code. 

## Running the tests

The userMicroservice python script has a set of functions created and can be called by the user to view/add/ remove data at any instant. Modify the script to create flow of data and test the microservice. 

The python scripts are well documented with each function and their use.




## Built With

* [Node.Js](https://nodejs.org/en/) - The web framework used
* [MongoDb Atlas](https://www.mongodb.com/cloud/atlas) - Database Management
* [Python](https://www.python.org/) - Microservice script


## Authors

* **Rohan Russel Nedungadi** - *Initial work* 

See also the list of [contributors](https://github.com/rohan9025/esa-assign2/contributors) who participated in this project.


## Acknowledgments

* Proff Raghu Kishore Neeliseti

