# RabbitMQ Tutorial Using Spring AMQP

These tutorials use Maven. To build them run

```
mvn package
```
The app uses Spring Profiles to control what tutorial it's running, and if it's a
Sender or Receiver. Choose which tutorial to run by using these profiles:

- {tut1|hello-world},{sender|receiver}
- {tut2|work-queues},{sender|receiver}
- {tut3|pub-sub|publish-subscribe},{sender|receiver}
- {tut4|routing},{sender|receiver}
- {tut5|topics},{sender|receiver}
- {tut6|rpc},{client|server}

After building with maven, run the app however you like to run boot apps.

For example:

```
java -jar rabbit-tutorials-1.7.1.RELEASE.jar --spring.profiles.active=hello-world,sender


java -jar rabbit-tutorials-1.7.1.RELEASE.jar --spring.profiles.active=hello-world,receiver


java -jar rabbit-tutorials-1.7.1.RELEASE.jar --spring.profiles.active=pub-sub,receiver --tutorial.client.duration=60000


java -jar rabbit-tutorials-1.7.1.RELEASE.jar  --spring.profiles.active=pub-sub,sender --tutorial.client.duration=60000

```
