# err-topic-a-day

This is a plugin for [Errbot](http://errbot.io) to manage a "topic-a-day" channel for daily discussion of topics.

## Installation
This plugin can be installed following [Errbot's plugin installation guide](https://errbot.readthedocs.io/en/latest/user_guide/administration.html#installing-plugins).

### What Version to Use
Errbot can install a plugin based on a git branch or a git tag. It is suggested that you choose a [Release](https://github.com/andrewthetechie/err-topic-a-day/releases) rather than Master or Dev. Releases will stay stable, but Master and Dev will change frequently.

## Slack commands
These are the command you can send privately to the bot and he will respond appropriately

### add_topic
send it the topic and the topic name and it will add it to the back of the queue

### list_topics
shows all the topics in all of the states

## Configuration
The plugin is configured by setting environment variables.

### TOPIC_CHANNEL
The name of the channel to post in
This value is required

### TOPIC_DAYS
Days to post a topic. Comma separated list of day names
the default is Monday to Friday 

For example TOPIC_DAYS="monday,tuesday,wednesday,thursday,friday"

### TOPIC_TIME
What time the topic is posted every day, 24hr notation
The default is "09:00" i.e. 9:00 AM. 
This time is based on the time of the system the bot is deployed on.

## Development
Development is done against the Dev branch. Changes are then merged into the Master branch and a release is made. 
