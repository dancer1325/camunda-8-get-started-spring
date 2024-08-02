# Get started with Camunda 8 and Spring Boot

* Spring Boot + [Spring Zeebe SDK](https://docs.camunda.io/docs/apis-tools/spring-zeebe-sdk/getting-started/#add-the-spring-zeebe-sdk-to-your-project) 
  * -- interact with a -- local Self-Managed Camunda installation

## Written guide

[Check Camunda docs][the-guide]

## Interactions with Zeebe

* Examples | this project:
  1. Deploying a process model.
  2. Initiating a process instance.
  3. Handling a service task.

## Prerequisites

1. A running Self-Managed Camunda installation (see [the associated guide][the-guide] for instructions).
2. [Maven](https://maven.apache.org/).
3. JDK 17+

## Running the project
* `mvn spring-boot:run`
  * Problems:
    * Problem1: "Failed to start bean 'zeebeLifecycleEventProducer'"
      * Attempt1: Adjust `zeebe.client.broker.restAddress`
      * Attempt2: Kill Camunda Modeler instance running
      * Solution: TODO:
* Output
  * process has been deployed,
  * process instance has been started,
  * service task has been handled

## Troubleshooting

* Camunda installation is running
  * TODO: How to check? What Camunda refers to?
* Zeebe Broker is accessible | `localhost:8080`, and the Zeebe Gateway is accessible | `localhost:26500`, or adjust the `application.properties` / match your configuration
  * TODO: How to check Zeebe is up?

[the-guide]: https://docs.camunda.io/docs/guides/getting-started-java-spring
