# Cloud-Native-Cassandra-Building-CRUD-applications-with-Python-and-NodeJS
Apache Cassandra is a free and open-source, distributed, wide column store, NoSQL database management system designed to handle large amounts of data across many commodity servers, providing high availability with no single point of failure.  This is a curated list of awesome Apache Cassandra packages and resources. Maintained by Rahul Singh of Anant. Feel free contact me if you'd like to collaborate on this and other awesome lists. Awesome Cassandra , Awesome Solr, Awesome Lucene. This powers the Resources section of Cassandra.Link, a rich collection of blog feeds, and curated links as a searchable knowledge base.
Node-Express-Cassandra CRUD sample Application
This is a simple Node-Express CRUD application using Cassandra.

Configuration
Cassandra connection configuration requires CASSANDRA_IP environment variable or cassandra link alias:

const client = new cassandra.Client({contactPoints: [process.env.CASSANDRA_IP || 'cassandra']});
Express configuration requires PORT environment variable. The default port is 3000:

app.listen(process.env.PORT || 3000);
Wercker environment properties to push image to repository:

DOCKER_USERNAME = username for Docker account
DOCKER_PASSWORD = password for Docker account
DOCKER_TAG = tag of the docker image
DOCKER_REPOSITORY = name of the new repository (includes image name)
How to run
In Docker environment use Docker link and define alias: cassandra for Cassandra service.

Or set Cassandra IP address as environment variable:

export CASSANDRA_IP=129.150.70.97
To start the Node application:

npm install
node app.js
History
1.0.0
Initial version
License
The Universal Permissive License (UPL), Version 1.0

Credits
The user interface layout is based on DARREN-2000/nodecrud.
