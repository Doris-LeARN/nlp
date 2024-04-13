# Sentiment Analysis using Forbes

#### WHAT IS KAFKA ?
Event streaming is the practice of capturing data in real-time from event sources like databases, sensors,
mobile devices, cloud services, and software applications in the form of streams of events; storing these
event streams durably for later retrieval; manipulating, processing, and reacting to the event streams in
real-time as well as retrospectively; and routing the event streams to different destination technologies
as needed. Event streaming thus ensures a continuous flow and interpretation of data so that the right
information is at the right place, at the right time.

#### EVENTS
An event records the fact that “something happened” in the world or in your business. It is also called record
or message in the documentation. When you read or write data to Kafka, you do this in the form of events.
Conceptually, an event has a key, value, timestamp, and optional metadata headers. Here’s an example
event:

- Event key : " Alice "
- Event value : " Made a payment of $200 to Bob "
- Event timestamp : " Jun . 25 , 2020 at 2:06 p . m ."

#### PRODUCERS / CONSUMERS
Producers are those client applications that publish (write) events to Kafka, and consumers are those that
subscribe to (read and process) these events. In Kafka, producers and consumers are fully decoupled and
agnostic of each other, which is a key design element to achieve the high scalability that Kafka is known for.
For example, producers never need to wait for consumers.

#### TOPICS
Events are organized and durably stored in topics. Topics in Kafka are always multi-producer and multisubscriber: a topic can have zero, one, or many producers that write events to it, as well as zero, one, or many
consumers that subscribe to these events. Topics in Kafka are always multi-producer and multi-subscriber: a
topic can have zero, one, or many producers that write events to it, as well as zero, one, or many consumers
that subscribe to these events. Events in a topic can be read as often as needed, you define for how long
Kafka should retain your events through a per-topic configuration setting, after which old events will be
discarded.

#### PROJECT SUMMARY
The goal of this project is to create an end-to-end Machine Learning project, including :
- extract tweets of specifics topics from Twitter, in real-time using Apache Kafka
- transform, using you trained-model for sentiments analysis classification
- load data into a data-warehouse using PostgreSQL
- real-time dashboard, to monitor the results for each topics using PowerBI 
Each parts can be start independently.
