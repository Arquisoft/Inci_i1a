# Inci_i1a
The system is composed by 4 submodules:  
#### - Loader.jar  
    Parses the agents from an excel file and loads them unto the Agents database.  
#### - Agents  
    This module consists of a REST web service that allows to query and obtain information about the agents that participate in the system.   
#### - InciManager  
     This module will process the incidents that are delivered by the different agents. The module will request information to agents module to check if the agents are registered in the system and are allowed to submit incidents. If the agent info is correct, he will be able to submit new incidents through Apache Kafka.  
#### - InciDashboard  
    The incidence dashboard will be used by the incident management staff for visualizing and managing the incidents that appear in the system. This module will receive incidents submitted by module 3 (InciManagement) through Apache Kafka.  

## Team members:  
Pedro Blanco Suárez (UO251935)  
Roberto Pérez Sánchez (UO250973)  
Manuel García Fernández (UO250979)  
Jorge González-Nuevo Bueno (UO251166)  
David Ferreiro Fernández (UO250757)  
Lucia Méndez López (UO250970)  
Pablo Suárez García (UO250924)  
Marcial Francisco Parrilla Socas (UO251851)  
Alejandro González Campomanes (UO251427)  
