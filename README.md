# zoobin

Zookeeper binary wrapper with the intent to be called in a unit file

## Maintainers

Names of core plans maintainers (The Habitat Maintainers humans@habitat.sh is usually sufficient)

## Type of Package

binary package


## Usage
Call hab package withing a startup script or unit file

ex. hab pkg exec aredeex/zoobin zkServer.sh start /etc/zookeeper/conf/zoo.cfg

when used this way you will need to export the needed env in the unitfile/startup script used

example unitfile entires:  
  Environment=ZOOMAIN=org.apache.zookeeper.server.quorum.QuorumPeerMain
  Environment=ZOOCFGDIR=/etc/zookeeper/conf
  Environment=ZOOCFG=/etc/zookeeper/conf/zoo.cfg
  Environment=ZOO_LOG_DIR=/var/log/zookeeper
  Environment=ZOO_LOG4J_PROP=INFO,ROLLINGFILE
  Environment=JMXLOCALONLY=true
