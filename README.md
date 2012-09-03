# Q Bot

The Q Bot (or 'queue bot') is a tool that supports meeting chairs in managing meetings by maintaining a speakers list. The functionality and interface has been inspired by W3C's [Zakim bot](http://www.w3.org/2001/12/zakim-irc-bot#speakerqueue "Zakim IRC Teleconference Agent").

## Commands

To activate Q Bot, a single `q` followed by one of the following terms must occur on the chat:

	+ ... add user who types the command to the end of the speaker queue
	- ... remove user who types the command from the speaker queue
	? ... show the speaker queue

So for example, three people, Jim, John and Mary (meeting chair) would go like:

	Jim: q+
	Q Bot: I see Jim wants to speak, adding him to the queue
	John: q+
	Q Bot: I see John wants to speak, adding him to the queue
	Mary: q?
	Q Bot: I see two people on the queue: Jim, John
	...
	[Jim says something very important]
	Jim: q-
	Mary: q?
	Q Bot: I see John on the queue
	
## License

The software provided here is in the Public Domain.