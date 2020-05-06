# Class 17 - TCP Server - 5/5/2020

## OSI Model - Open Systems Interconnection
* This is how the computers communicate with each other under the hood.
* It has 7 layers:
  1. Physical
  2. Data Link
  3. Network
  4. Transport - TCP and UDP - Where our TCP server operates
  5. Session
  6. Presentation
  7. Application

## TCP Server
* TCP - Transimission Control Protocol.
* Creates a two way communication between two systems.
* Provides reliable, ordered, and error checked byte streams between the application.

## Chat App 
* Server: TCP based, broadcast messages to all chat-clients. It is publisher.
* Logger: it is a client, it only logs the messages and it is subscriber.
* Chat-client: it is a client, it sends and receives messages and it is publisher/suscriber.