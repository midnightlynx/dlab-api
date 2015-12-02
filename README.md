## running
You need to have python's `virtualenv` installed and on your path.
You will also need to configure the NEO4J_URI variable to access
a Neo4j instance. This can be done in `config.py` or by setting
it as a system environment variable.

The NEO4J_URI string for accessing capstone's instance can be found
on the Servers Trello board on Neo4j -> NEO4J_URI.

```
# create python virtual environment and fetch dependencies
./setup.sh

# set environment variable to a running Neo4j instance
export NEO4J_URI=<uri access string>

# run all tests
./env/bin/nosetests

# start local api server
./env/bin/python run.py
```

You should now have the api server running at 127.0.0.1:9000
