1. The publisher program will send 5 data messages to the message broker in one run. This is because there are 5 calls to publish_event() method, each sending a UserCreatedEventMessage to the message broker.

2. I think  The URL "amqp://guest:guest@localhost:5672" is the same as the one in the subscriber, the amqp is the protocol used like http and https. guest:guest is the username:password, localhost is the machine runnning it, and 5672 is the port used/ 

3. A screenshot showing RabbitMQ running 
![Screenshot of RabbitMQ](img/rabbitMQ.png "RabbitMQ.png")

4. A screenshot showing the subscriber recieving what the publisher is sending
![Screenshot sending and processing event](img/cargoRunPubXSubs.png "cargorRunPubXSubs")