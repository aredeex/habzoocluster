# zoobin

Zookeeper binary wrapper with the intent to be called in a unit file

## Maintainers

Names of core plans maintainers (The Habitat Maintainers humans@habitat.sh is usually sufficient)

## Type of Package

binary package


## Usage
Call hab package withing a startup script or unit file

ex. hab pkg exec aredeex/zoobin zkServer.sh start /etc/zookeeper/conf/zoo.cfg
