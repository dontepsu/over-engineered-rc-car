# Over engineered RC car
Radio controlled car with Raspberry PI, PS4 controller, Go, Websockets and React.

## The plan
In the center of the project is a Raspberry PI. The RPI acts as the cars central computer by controlling the motor and steering while providing an API. To minimize the connection overhead, all communication between the car and client sending commands will be done using Websockets.

The car will be connected to wifi, or if no wifi avaliable it will turn into access point mode. There are some plans to add a 5g mobile network connection, but that is low priority at the moment thus focusing getting the connection working through wifi first.

Controlling the car is done by using a Playstation 4 remote controller. The idea here is simple, the car will provide a Webserver and API using Websockets. Also the car will be hosting a React Web App. The PS4 controller will be connected to a device such as laptop or tablet computer and the command will be passed to the Web App though [Gamepad API](https://developer.mozilla.org/en-US/docs/Web/API/Gamepad_API). The server will receive commands through the Websocket API and will then be propagated to services abstracting the usage of Raspberry PI GPIO.

## About the projects
All source code related to project will be published within this repository. I will also be including here more detailed text describing and YouTube videos to show more in depth how the code and the hardware works. This is not a project to be done in weeks, rather in months.
