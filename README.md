# Data Analysis Project
This project is being developed for the Alcoding Club of PES University, Bangalore.
It is a Web Application that acts as a portal for all students belonging to the Computer Science Department, in which students can view their coding contest rankings and submit assignments for the courses they have enrolled.
This project is currently being developed using the MERN stack. 
Implementation details, features shall be enlisted in the near future. 


## Requirements

- [Node.js](https://nodejs.org/en/) 6+
- [MongoDB](https://docs.mongodb.com/manual/installation/)

```shell
npm install
```


## Instructions

Production mode:

```shell
npm start
```

Development (Webpack dev server) mode:

```shell
npm run start:dev
```

### Note
1. Make sure to add a `config.js` file in the `config` folder. See the `config.example.js` under `config/` directory for more details.
2. Genrate and add ssl files in the `server/` directory under a folder named `sslcert`.
```
openssl req -x509 -out localhost.crt -keyout localhost.key \
  -newkey rsa:2048 -nodes -sha256 \
  -subj '/CN=localhost' -extensions EXT -config <( \
   printf "[dn]\nCN=localhost\n[req]\ndistinguished_name = dn\n[EXT]\nsubjectAltName=DNS:localhost\nkeyUsage=digitalSignature\nextendedKeyUsage=serverAuth")
```
Rename the two generated files to `server.key` and `server.crt`.
