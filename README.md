# Meetup.com Real-Time Analytics #

## Abstract ##

The concept of real time analytics assumes ever increasing importance with more and more data coming from smart connected devices. The constant stream of data that is coming from these connected systems is unique in its volume, variety and velocity. Ingesting, analyzing and presenting these highly unstructured data assumes significance as it will throw insights in real time that will help businesses make decisions quicker.

In our project we wanted to dig deeper into this exciting field of real time analytics and get an insight into the technologies and the working of the real time streaming analytics. Hence, we analyzed the real time RSVP data of meetup.com to get real-time insights such as trending topics, cities etc. along with other business insights related to Meetups RSVPs. 

We utilized Apache Kafka for building real-time pipelines and Apache Spark to do real-time analysis and matplotlib for visualization. As and when an RSVP response is made by a user, our Kafka Producer receives that message through meetup’s web socket and feeds it to a topic. Then Kafka’s Consumer which has subscribed to that topic sends it to Spark’s streaming platform where only the U.S. messages are filtered and real time analysis to get the trending cities within the U.S. takes place. Then the results of the analysis get stored to a text file in our local system, using which visualizations is done in near real time using matplotlib. 

This project can be extended to get the real time trending topics across the world or for a specific geography along with other business insights. By giving real time trends in topics like in twitter, users of meetup will be aware of the more popular and less popular topics in near real time. With minor modifications, this project can also be extended to process and analyze IoT data.
