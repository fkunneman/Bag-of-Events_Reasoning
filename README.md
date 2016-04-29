# Bag-of-Events_Reasoning
This repository is the RU-VU place to drop data in the form of bags-of-events and share code to reason over these events and find common patterns. A bag-of-events can be described as a sequence of events that relate to one unifying event. For example: all campaign events and debates that relate to specific elections. Reasoning over such instances can result in knowledge about subsumption and temporal relations between events. Bags-of-events might be automatically extracted from reports in the news media as well as social media.  

# Dataformat *
Bags of events might be formatted in .json, with the following keys:

bag-of-events_id : str                  Unique key \\
bag-of-events_name : str                Phrase that describes the unifying event 
bag-of-events_type : str                Event type (disaster, human interest, sports, etc.), if known 
bag-of-events_starttime : datetime      The start time of the event 
bag-of-events_endtime : datetime        The end time of the event 
sub_events : list                       All events in the bag-of-events 
    sub_event_id : str
    sub_event_name : str
    sub_event_type : str
    sub_event_starttime : datetime
    sub_event_endtime : datetime

\* This is of course open to debate. 
