# Create an Ethereum cluster using containers

```yaml
by: иÐгü
email: ndru@chimpwizard.com
date: 02.28.2019
version: draft
```

****

The goal of this POC is to get the Ethereum framework working inside a container clustery.

The source code can be found [here](https://github.com/chimpwizard/playgound/tree/master/blockchain/ethereum).


## Proposed Architecture



(**SOME IMAGE TBD**)

## Preparing the environment

### Development tools

- Install metamask plugin: [link](https://chrome.google.com/webstore/search/metamask?hl=en-US&utm_source=chrome-ntp-launcher)
- Install truffle : npm install truffle --save-dev
- Install Test RPC: npm install ethereumjs-testrpc --save-dev

### Blockchain server


## The implementation


## Prerequisites to run the code

- install [npm](https://docs.npmjs.com/getting-started/what-is-npm)
- install [vagrant](https://www.vagrantup.com/intro/index.html)

### to start the cluster

```shell
npm run up      # To create the servers
npm run deploy  # To deploy the stack in the cluster
```

... then go to [http://172.10.10.20:8000](http://172.10.10.20:8000) and update the connection to
**172.10.10.20:8080** to point to the database api. The portainer console can be located at [http://172.10.10.20:9000](http://172.10.10.20:9000) for this use user **"admin"** and password **"password"**.

All server instances listen on port 8080, this takes advantage of the embeded load balancer that comes with docker swarm.

### to clean up your machine

```shell
npm run destroy
```

## Some references while doing this

- xxx
