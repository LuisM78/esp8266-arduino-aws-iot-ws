# AWS IoT Websockets

Library for connecting to the AWS IoT service from an ESP8266 using websockets. Authenticates using AWS IAM credentials and sigV4.

Based on the work of [AWS labs](https://github.com/awslabs/aws-sdk-arduino), basically using its SigV4 implementation and a fork by [Sander van de Graaf](https://github.com/svdgraaf/aws-sdk-arduino). The fork is reflected in [the License](LICENSE).

Inspired by [Fábio Toledo](https://github.com/odelot/aws-mqtt-websockets)s work on [aws-mqtt-websockets](https://github.com/odelot/aws-mqtt-websockets), but using libraries accessible through the PlatformIO library manager. **This is actually the main reason for creating the library**.

Adds MQTT functionality using the [Paho](https://projects.eclipse.org/projects/technology.paho) library. It is fairly easy to replace with another MQTT client, e.g. [PubSubClient](https://github.com/knolleary/pubsubclient).

## Attributions

Big thanks to [Fábio Toledo](https://github.com/odelot) for his work on [aws-mqtt-websockets](https://github.com/odelot/aws-mqtt-websockets). Any credit should be directed to him and the authors of the libraries used in this project.

The library uses code from the following projects. License information can be found in the [NOTICE](NOTICE) file:
- [AWS labs - aws-sdk-arduino](https://github.com/awslabs/aws-sdk-arduino)
- [Sander van de Graaf - aws-sdk-arduino](https://github.com/svdgraaf/aws-sdk-arduino)
- [Fábio Toledo - aws-mqtt-websockets](https://github.com/odelot/aws-mqtt-websockets)
- [Serge Zaitsev - JSMN](https://github.com/zserge/jsmn)
- [Paho MQTT client](https://www.eclipse.org)
- [Stephan Brumme - SHA256](http://create.stephan-brumme.com/)

In the case of missing license information, I took the liberty of adding it.

## Architecture

![class diagram](http://yuml.me/69df5325 "AWS IoT Websockets class diagram")
