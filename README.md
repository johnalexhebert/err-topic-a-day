# err-topic-a-day

## Description
This is a plugin for Errbot (http://errbot.io) to manage a "topic-a-day" channel for daily discussion of topics

## Usage
you might want to look here for details (https://errbot.readthedocs.io/en/latest/user_guide/administration.html#installing-plugins)

## Validation
When running the program, some validations will run and if they are not configured properly an exception will be raised with the appropriate response

# Slack commands
These are the command you can send privately to the bot and he will respond appropriately

## add_topic
send it the topic and the topic name and it will add it to the back of the queue

## list_topics
shows all the topics in all of the states

# Environment Variables

## Customizable
In this section you can see all of the environment variables that can be used.

### TOPIC_CHANNEL
The name of the channel to post in
This value is required
the value should start with a pound key(`#`) as all channels do 


### TOPIC_DAYS
Days to post a topic. Comma separated list of day names
the default is Monday to Friday 

For example TOPIC_DAYS="monday,tuesday,wednesday,thursday,friday"

### TOPIC_TIME
What time the topic is posted every day, 24hr notation
the default is 9AM

### TOPIC_POLLER_INTERVAL
How frequently the poller runs. Lower numbers might result in higher load
the default is 5, and it's an integer value (so no funny business with 2.5 okay?)

## Automatic
These are generated from previous ones, they will show up in the config but don't touch them

### TOPIC_CHANNEL_ID
channel id that is extracted from the channel name

