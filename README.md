# Inci_i1a
The application is an incidence analysis system composed by 4 submodules:  
#### - Module 1.- Information Loader: [Loader](https://github.com/Arquisoft/Loader_i1a)  
   
   Parses the agents from an excel file and loads them unto the Agents database.  

#### - Module 2.- Agent management and querying: [Agents](https://github.com/Arquisoft/Agents_i1a)  

   This module consists of a REST web service that allows to query and obtain information about the agents that participate in the system.   
   
#### - Module 3.- Incidence Management: [InciManager](https://github.com/Arquisoft/InciManager_i1a)

   This module will process the incidents that are delivered by the different agents. The module will request information to agents module to check if the agents are registered in the system and are allowed to submit incidents. If the agent info is correct, he will be able to submit new incidents through Apache Kafka.  
   
#### - Module 4.- Analysis and dashboard: [InciDashboard](https://github.com/Arquisoft/InciManager_i1a)  

   The incidence dashboard will be used by the incident management staff for visualizing and managing the incidents that appear in the system. This module will receive incidents submitted by module 3 (InciManagement) through Apache Kafka.  

## Spring Boot  

The application has been developed using [Spring Boot 1.4.](https://projects.spring.io/spring-boot/)  

## MongoDB  
The submodules share a common MongoDB database on the cloud storage of the [mLab webpage.](https://mlab.com/)  

## Apache Kafka  
The last two submodules communicate sending the incidents through Apache Kafka. A quick tutorial on how to set the zookeeper and the kafka server needed may be found on the [Apache Kafka webpage](https://kafka.apache.org/quickstart)  

## Team members:  
- [Pedro Blanco Suárez (UO251935)](https://github.com/pedrytus)  
- [Roberto Pérez Sánchez (UO250973)](https://github.com/robertops18)  
- [Manuel García Fernández (UO250979)](https://github.com/faltosu)  
- [Jorge González-Nuevo Bueno (UO251166)](https://github.com/jorgegnb)  
- [David Ferreiro Fernández (UO250757)](https://github.com/rimorD)  
- [Lucia Méndez López (UO250970)](https://github.com/UO250970)  
- [Pablo Suárez García (UO250924)](https://github.com/PabloSuaGar)  
- [Marcial Francisco Parrilla Socas (UO251851)](https://github.com/marcialfps)  
- [Alejandro González Campomanes (UO251427)](https://github.com/alexgonzcampomanes)  
