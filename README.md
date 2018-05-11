# Inci_i1a

Launched Application Links:
   -InciManager: http://cf-azuc-docker-node-0037.az.codefresh.io:33161/
   -InciDashboard: http://cf-azuc-docker-node-0037.az.codefresh.io:33162/
The application is an incidence analysis system composed by 4 submodules:  

#### - Module 1.- Information Loader: [Loader](https://github.com/Arquisoft/Loader_i1a)  
   
   Parses the agents from an excel file and loads them unto the Agents database.  

#### - Module 2.- Agent management and querying: [Agents](https://github.com/Arquisoft/Agents_i1a)  

   This module consists of a REST web service that allows to query and obtain information about the agents that participate in the system.   
   
#### - Module 3.- Incidence Management: [InciManager](https://github.com/Arquisoft/InciManager_i1a)

   This module will process the incidents that are delivered by the different agents. The module will request information to agents module to check if the agents are registered in the system and are allowed to submit incidents. If the agent info is correct, he will be able to submit new incidents through Apache Kafka.  
   
#### - Module 4.- Analysis and dashboard: [InciDashboard](https://github.com/Arquisoft/InciDashboard_i1a)  

   The incidence dashboard will be used by the incident management staff for visualizing and managing the incidents that appear in the system. This module will receive incidents submitted by module 3 (InciManagement) through Apache Kafka.

## Graphic representation of the system

![Diagram of Inci_i1a](https://i.imgur.com/BPy28pi.png "Diagram of Inci_i1a")

## Spring Boot  

The application has been developed using [Spring Boot 1.5.](https://projects.spring.io/spring-boot/)  

## MongoDB  
The submodules share a common MongoDB database on the cloud storage of the [mLab webpage.](https://mlab.com/)  

## Apache Kafka  
The last two submodules communicate sending the incidents through Apache Kafka. A quick tutorial on how to set the zookeeper and the kafka server needed may be found on the [Apache Kafka webpage](https://kafka.apache.org/quickstart)  

## Docker  
To ship and distribute the application we use [Docker](https://www.docker.com/what-docker), each module, Kafka and Zookeeper are indepentent Docker containers. To download and install Docker for Windows, you can use the following [link](https://docs.docker.com/toolbox/toolbox_install_windows/).  

## Gatling  
Agents, InciManager and InciDashboard have been put through a battery of load/stress tests, done using the automated testing tool [Gatling](https://gatling.io/download/), more information about Gatling can be found on the [Gatling documentation](https://gatling.io/documentation/) or in the [InciDashboard readme](https://github.com/Arquisoft/InciDashboard_i1a).  

## Cucumber
[Cucumber](https://cucumber.io/) is an open-source tool for executable specifications, it's been used on the InciDashboard to create user tests based on specifications. You can perform the installation following the instructions on the [Cucumber documentation](https://docs.cucumber.io/installation/).  

## Team members:  
- [Pedro Blanco Suárez (UO251935)](https://github.com/pedrytus)  
- [David Ferreiro Fernández (UO250757)](https://github.com/rimorD)  
- [Manuel García Fernández (UO250979)](https://github.com/faltosu)  
- [Alejandro González Campomanes (UO251427)](https://github.com/alexgonzcampomanes)  
- [Jorge González-Nuevo Bueno (UO251166)](https://github.com/jorgegnb)
- [Lucia Méndez López (UO250970)](https://github.com/UO250970)  
- [Roberto Pérez Sánchez (UO250973)](https://github.com/robertops18)  
- [Marcial Francisco Parrilla Socas (UO251851)](https://github.com/marcialfps)  
- [Pablo Suárez García (UO250924)](https://github.com/PabloSuaGar)  
