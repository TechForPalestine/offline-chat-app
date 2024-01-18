# Software Requirements Specifications

## Introduction
..

### Scope & Value
...

### Audience & Intended use
...

### Definitions
...

### Table of Contents
...

## Functional Requirements

### Connection
Connect two or more devices in a local network through a connection medium.

Specifications of the connection medium:
- Supported on the oldest possible smartphones.
- Independent of the blacked-out mediums: does not require the Internet/Satellite or electricity. Hence, extra hardware that runs on electricity e.g. routers.
- Compatible with multiplatforms: Android, iOS, linux phones. - (debatable for MVP) 
- Covers a wide range. - (debatable for MVP) _range specifications needed_
- Provides high data transfer rate. - (debatable for MVP) _rate and size specifications needed_
- ...
 
Specifications of the local network:
- Decentralized: without a point of failure.
- Distributed: data is distributed among the connected points.
- Allows routing of packets: sent packets are routed in the network till it reaches the intended receiver. (debatable for MVP)
- ...

_Type of used connection would be submitted with an ADR (architecture decision record)._

Stories:
- As a user, I want to be able to connect to the local network.
- As a user, I want to be able to disconnect from the local network.
- As a user, I want to see an indicator of my connection status.
- As a user, I want to see a list of possible devices to connect to. (could use a breakdown later on)

### Communication
Allow connected devices to share text messages in three ways: one-to-one conversations, many-to-many conversations or a public room.
In case a device disconnects, allow them to receive their missed messages when they connect back into the network.

### Ways of Communications

#### One-to-One Conversations
Allow two connected devices to initiate a chat between each other. 

Stories:
- As a user, I want to be able to send a message to a connected device of my choice.
- As a user, I want to be able to receive a message when a device initiates a chat with me.

##### Many-to-Many Conversations (debatable for MVP)
Allow a connected devices to initiate a chat between themselves and many other chosen connected users.

#### Public room (debatable for MVP)
All devices on the network are able to read and send messages in this room. The data in this room bounces over connected devices.

Stories:
- As a user, I want to be able to send a message in a public room for everyone to see.
- As a user, I want to be able to read messages in the public room.

### Sync offline Messages
_Submit an ADR to decide on the sync messages service_

Stories:
- As a user, I want to be able to receive the messages that I have missed during my disconnection once I am connected back into the network.
- As a user, I want to be able to re-sending messages that I sent during a disconnection.

## known Constraints
- Battery consumption.
- Connection coverage distance.
- Multiplatform support.
- ...
