

# PoC-TruthChain

Proof of Concept: a blockchain-based truth base. Bigchain DB+Ethereum


### Dependencies

The examples can be [run via Docker](http://bigchaindb-examples.readthedocs.io/en/latest/install.html#the-docker-way)
(**recommended**), but, if you'd like, you can also [run them locally](http://bigchaindb-examples.readthedocs.io/en/latest/install.html#install-from-source)
with the following system dependencies:

 - OS dependencies: see [setup BigchainDB & RethinkDB](https://bigchaindb.readthedocs.io/en/latest/installing-server.html#install-and-run-rethinkdb-server)
 - python>=3.4
 - node>=5.3 using [nvm](https://github.com/creationix/nvm#installation) (**recommended**), or [manually](https://nodejs.org/en/download/)
 - [npm>=3.3](https://docs.npmjs.com/getting-started/installing-node) (should be installed with node)

## Quick start


### Docker

To run via Docker, set up your docker environment as necessary and:

```bash
$ make
```

**Note**: If using docker-machine, you'll have to run `make` with your docker-machine ip:

```bash
$ DOCKER_MACHINE_IP=$(docker-machine ip) make
```

The app will be available at <http://localhost:33000> (replace ``localhost`` with your
docker-machine ip as necessary).

### Locally

If you'd like to run this locally (preferably in a virtualenv), you can do so using
the handy CLI:

```bash
$ bigchaindb-examples --help

# Start everything
$ bigchaindb-examples start --init --all

# Reset everything
$ bigchaindb-examples reset-all
```

The app will be available at <http://localhost:3000>.


