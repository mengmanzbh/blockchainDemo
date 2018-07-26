## Bill Endorse Demo

A sample Node.js app to demonstrate **__fabric-client__** & **__fabric-ca-client__** Node.js SDK APIs

### Prerequisites and setup:

* [Docker](https://www.docker.com/products/overview) - v1.12 or higher
* [Docker Compose](https://docs.docker.com/compose/overview/) - v1.8 or higher
* [Git client](https://git-scm.com/downloads) - needed for clone commands
* **Node.js** v6.9.0 - 6.10.0 ( __Node v7+ is not supported__ )
* [Download Docker images](http://hyperledger-fabric.readthedocs.io/en/latest/samples.html#binaries)

```
ami-b49f64c9(Virginia)ubuntu官方镜像 密码:bitnami
sudo -i
wget -qO- https://get.docker.com/ | sh
sudo usermod -aG docker root
apt-get install jq


cd trainingProjects/billEndorse 
npm install
npm install -g bower

cd trainingProjects/billEndorse/public/ng
bower install

cd trainingProjects/billEndorse 
./setupFabricNetwork.sh
./createChannelAndInstallChaincode.sh
```

access http://localhost:4000/ng/src/
