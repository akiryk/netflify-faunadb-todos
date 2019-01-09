# Todos App with Netlify and FaunaDB

This is a learning project for building a serverless Todos app using Netflify and Faunadb.

## Run Locally
```sh
# use latest node
nvm use 11.6

# Set FaunaDB key locally
export FAUNADB_SECRET=SECRETGOESHERE
```

## Key Resources

* [Netlify Tutorial Repo](https://github.com/netlify/netlify-faunadb-example)
* [Using Fauna Shell](https://github.com/fauna/fauna-shell)
* [CSS Tricks Video](https://css-tricks.com/video-screencasts/165-building-your-backend-with-serverless-functions/#respond)
* [Fauna DB Dashboard](https://dashboard.fauna.com/db)
* [Netlify Dashboard](https://app.netlify.com/)

## Using Fauna
``` sh
# Key Commands
fauna cloud-login
fauna create-database my-app
# Start Shell with my-app
fauna shell 'my-app'
# Create secret key for my-app
# fauna create-key [appname] [role, which is server or admin]
fauna create-key my-app server

# Database commands
fauna list-databases
fauna delete-database some-app
fauna list-keys
fauna delete-key 1232322323
```

### The Fauna Database Structure

Structure | Description
--------- | ---------------------
Database | A grouping of classes.
Class | A grouping of relatable instances. Analogous to tables in SQL.
Instance | A record, this is your actual data. These are structured documents and can include recursively nested objects, arrays, scalar types


