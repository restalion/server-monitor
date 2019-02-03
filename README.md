# server-monitor
Extremely simple server monitor. Just to monitor if server is up&running, also maintain historical monitoring data and can add, remove, activate and deactivate servers to monitor.

![Main](img/server-monitor-main.png "server-monitor main")

## Quick start
Instructions to start easily using this project

### Maven
#### Prerrequisites
1. JDK 8 installed
1. Maven installed
1. MongoDB instance available

#### Execution
##### Review configuration
1. Review applicaton.properties:
    1. **spring.data.mongodb.uri:** maybe you need to use *spring.data.mongodb.host* and *spring.data.mongodb.port* instead

    1.**spring.data.mongodb.database:** if you want to change the database

    1.**server.port:** if you want to change the port that the application is using

### Docker
#### Prerrequisites
1. Docker installed in the system. Docker compose should also be available.
1. Ports 27017 and 8080 should be available.

#### Preparation
1. Clone the project into your system
1. Find docker-compose.yml file (it's the only file needed for this option)

#### Execution
1. Open a console and go to the folder containing the docker-compose.yml file
1. Run docker-compose up
1. Now the solution is up&running

## Advanced Options
### Execution parameters

## Application description
### Topology
Application itself it's very simple, just a Spring Boot application using Vaadin and Spring Data to access to a MongoDB database.

![Application Topology](img/server-monitor-topology.png "server-monitor topology")

Both parts can be executed independient elements, as docker images os as a whole using the provided docker-compose.yml file.

### Elements
Going deeper into the project we can view the elements below:

![Elements](img/server-monitor-elements.png "server-monitor elements")
#### Endpoints
#### Views
#### Services
#### Scheduled processes
#### Database

## Next Steps

## Contact
