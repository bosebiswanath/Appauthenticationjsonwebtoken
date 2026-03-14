# API Authentication using NodeJs

This is an Authentication API using JWT's that you can plug inside your current project or you can start with a new one. Email \& Password is used for authentication.

The API based on Node.js, Express, MongoDB \& Redis, following the **MVC pattern** i.e. Model ~~View~~ Controller.

**Mongoose** is used for storing Users in Database.
**Redis** is used for storing Refresh Tokens - to validate them as well at the same time Blacklisting them.

The application is **production ready**.

\---

## To start setting up the project

Step 1: Clone the repo

```bash
git clone https://github.com/bosebiswanath/Appauthenticationjsonwebtoken.git

Step 2: cd into the cloned repo and run:

```bash
npm install
```

Step 3: Put your credentials in the .env file.

```bash
PORT=3000
MONGODB\\\\\\\\\\\\\\\_URI=mongodb://localhost:27017
DB\\\\\\\\\\\\\\\_NAME=YOUR\\\\\\\\\\\\\\\_DB\\\\\\\\\\\\\\\_NAME
ACCESS\\\\\\\\\\\\\\\_TOKEN\\\\\\\\\\\\\\\_SECRET=GENERATE\\\\\\\\\\\\\\\_FROM\\\\\\\\\\\\\\\_GENERATE\\\\\\\\\\\\\\\_KEYS\\\\\\\\\\\\\\\_FILE\\\\\\\\\\\\\\\_IN\\\\\\\\\\\\\\\_HELPER
REFRESH\\\\\\\\\\\\\\\_TOKEN\\\\\\\\\\\\\\\_SECRET=GENERATE\\\\\\\\\\\\\\\_FROM\\\\\\\\\\\\\\\_GENERATE\\\\\\\\\\\\\\\_KEYS\\\\\\\\\\\\\\\_FILE\\\\\\\\\\\\\\\_IN\\\\\\\\\\\\\\\_HELPER
```

Step 4: To generate 256-bit keys for JWT

```bash
node ./helpers/generate\\\\\\\\\\\\\\\_keys.js
```

Step 5: Install Redis (Linux Ubuntu)

```bash
sudo apt-get install redis-server
```

Step 6: Run Redis Server (Linux Ubuntu)

```bash
redis-server
```

```

Step 7: Start the API by

```bash
npm start
Author

* ## Biswanath

## License

This project is licensed under the MIT License.

