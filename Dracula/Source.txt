"English Project" by Cory Brzyck

The block giving rule is not listed in the check giving it to rules.
Persuasion rule for asking people to try doing something: 
persuasion succeeds.

Persuasion rule for asking someone to try giving something to player: 
persuasion succeeds.

Understand the command "read" as something new.
Reading is an action applying to one thing.
Understand "read [something]" as reading.
A thing can be readable. A thing is usually not readable. 
A written thing is a kind of thing. A written thing is usually readable. 
A written thing has some text called writing. The writing of a written thing is usually "Nothing unusual is written here."

Understand the command "shoot" as something new.
Shooting is an action applying to one thing.
Understand "fire[something]" as shooting.
A thing can be shootable. A thing is usually not shootable.
A gun is a kind of thing. A gun is usually shootable.

Understand the command "blow" as something new.
Blowing is an action applying to one thing.
Understand "blow[something]" as blowing.
A thing can be blowable. A thing is usually not blowable.
A whistle is a kind of thing. A gun is usually blowable.

Number left is a number that varies. Number left is 50.

Requesting number left is an action out of world.
Report requesting number left: say "[number left] boxes left to destroy".
Understand  "Number of boxes left" as requesting number left.

Requesting help is an action out of world.
Report requesting help: say "Use N to move North, S to move South, E to move East, W to move West. [line break]Use 'read' <object> to attempt to read something. [line break]Use 'examine' or 'x' to get a detailed description of a person or object.[line break]Use 'shoot' <object> to attempt to fire something. [line break]Use 'blow' <object> to attempt to blow air through it. [line break]Use 'Number of boxes left' to find out the number of boxes left to destroy.[line break]Use 'ask' <person> about/for <object> to try to receive an object from someone."
Understand "help" as requesting help.

Check reading when the noun is not readable: say "That's not something that can be read." instead.
Report reading: say the writing of the noun.

Understand the command "destroy" as something new.
Destroying is an action applying to one thing.
Understand "destroy [something]" as destroying.
A thing can be destroyable. A thing is usually not destroyable.
A destructable thing is a kind of thing. A destructable thing is usually destroyable.
When a thing is destroyed it is removed.

Understand "destroy [something] with holy wafer" as destroying [something].

A box of earth is a kind of thing. The plural of a box of earth is boxes of earth.

A cell is a thing.
Rats are a thing.
A pistol is a gun.
A silver whistle is a whistle.

A person has a table name called conversation.
		
Mina, Seward, Van Helsing, Holmwood, Morris, and Renfield are people.

Morris carries a pistol.
Van Helsing carries a thing called a cross and a thing called a holy wafer.
Seward carries a thing called keys.
Holmwood carries a silver whistle.

Instead of asking [someone] about something: 
	let the source be the conversation of noun; 
	if topic understood is a topic listed in source: 
		say "[action entry]";
		say "[reply entry][paragraph break]".
		
		
Instead of asking [someone] for something:
	try asking noun about it.

The conversation of Morris is Table of Morris' Words. 

Table of Morris' Words
	topic	reply											action											
	"pistol"	"I don't think using a pistol is a good idea here" 		"[Morris giving a pistol to the player]"

To say Morris giving a pistol to the player:
		try Morris giving a pistol to the player;
	
The conversation of Holmwood is Table of Holmwood Words. 

Table of Holmwood Words
	topic	reply											action											
	"whistle"	"I'm not sure what good it will be, but I think I did see some dogs around the neighborhood" 		"[Holmwood giving a silver whistle to the player]"

To say Holmwood giving a silver whistle to the player:
		try Holmwood giving a silver whistle to the player;
	
The conversation of Van Helsing is Table of Van Helsing Words. 

Table of Van Helsing Words
	topic	reply											action											
	"cross"	"I cannot give this to you" 							""
	"holy wafer"	"It would be best for me to hold onto these"		""
	
The conversation of Seward is Table of Seward Words. 

Table of Seward Words
	topic	reply											action											
	"keys"	"It would be foolish for me to give you my keys" 		""
	


The description of Mina is "My fiancé. She's hard at work peicing together information that will hopefully help us defeat Dracula. I worry that she might be at risk because of how close she was to Lucy...".

The description of Seward is "The doctor of this asylum. He's used to seeing strange things, but recent events have even seemed to overwhelm him. More than any of us, he is dedicated to defeat Dracula, perhaps because of the time he spent with Van Helsing".

The description of Van Helsing is "A professor from the Netherlands. He seems to know about everything. It's obvious that this isn't the first time that he is dealing with the supernatural".

The description of Holmwood is "Lucy's fiancé. I'm not sure how he is still standing after what he's been through. It take a strong man to continue to fight after the thing he loved most in this world has been taken away from him by the devil".

The description of Morris is "A brave American (you don't see those everyday).".

The description of Renfield is "A twisted being. Seward has told us about his obsession with consuming living things. Mina seems to think that he may have some connection to the Count.".

The description of player is "I've been through too much already to give up. I must stay strong, if not for myself, for Mina".

The description of Asylum Door is "A heavy door."

When play begins:
	say "Welcome to the interactive adventure of Dracula. The Count has recently begun his conquest of England in London.  It is up to you, as Johnathan Harker, to find a way to banish the Count and force him to retreat to Transylvania. It is imperative that you work as quick as possible.  'Denn die Todten reiten Schnell.'~For the dead travel fast [paragraph break] At any point in the game, typing 'help' will bring up a list of commands at your disposal".

The Asylum Atrium is a room. "You notice Mina working hard a typewriter and Seward squinting at your journal. Van Helsing sits in the back, staring at the ceiling. To the south you see a heavy door leading out of the Asylum. You can hear rustling coming from the room to west".
	Mina and Seward are in the Asylum Atrium.

After player  going to the Asylum Atrium:
	 if Holmwood is in the Asylum Atrium:
		say "Van Helsing steps forward and begins to address the group: 'It  is our duty to drive this vampire back to his home. I know it will not be easy, he can take the form of any animal and is stronger than all of us put together. He is also smart. No matter the cost, we must  band together to create a brighter tomorrow.' [paragraph break] Seward walks over to the door to the East and unlocks it [paragraph break] Morris, Holmwood, and Van Helsing exit the Asylum to head for Carfax";
		Now the Asylum Door is unlocked;
		Now Van Helsing is in the Carfax;
		Now Holmwood is in the Carfax;
		Now Morris is in the Carfax;
		Now Seward is in the Carfax;
	otherwise if the rats are in the Secret Room:
		say "Mina runs over and tells you that she has found the locations of the remaining 21 boxes. 12 of them are located in the East End while the other 9 are at a house in Piccadilly. The group has decided to split up, you to go with Van Helsing to Piccadilly while Holmwood and Morris take care of the other boxes";
		Now Morris is in the Secret Room.
		Now Holmwood is in the Secret Room.
		
The Holding Cell is a room. The Holding Cell is west of the Asylum Atrium. 
After player going to the Holding Cell:
	if the rats are not in the Secret Room:
		say "You hear Renfield rambling nonsense about animals, blood, and life. You best leave before he notices you and enters into a fit of rage";
		Now a cell is in the Holding Cell;
		Now Renfield is in the Cell;
	else:
		say "You find that Renfield has had is neck snapped. Perhaps you aren't as far ahead of Dracula as you thought you were.".
	
		
		
Secret Room is a room.
Morris and Holmwood are in Secret Room.	

The Study is a room. The Study is south of the Asylum Atrium. "This room is full of books and shelves. You notice a shipping log sitting on the desk".
	Seward's Desk is in the Study. 
	The shipping log is a written thing on Seward's Desk. 
	The writing of the shipping log is "You take note  of fifty crates that have been shipped to England from Translyvania. It appears that they were all delivered to the chapel Carafax next door."
			
			After the player reading shipping log:
				now the player has the shipping log;
				say "You pick up the shipping log and begin to read.";
				if Holmwood is in the Secret Room begin;
					say "You take note  of fifty crates that have been shipped to England from Translyvania. It appears that they were all delivered to the chapel Carafax next door.";
					now  Holmwood is in the Asylum Atrium;
					now Morris is in the Asylum Atrium;
				end if.
				
The Asylum Door is a lockable door. The Asylum Door is locked. The Asylum Door is east of the Asylum Atrium and west of the Essex Purfleet. 
				
The Essex Purfleet is a room. The Essex Purfleet is east of the Asylum Door.  The Essex Purfleet is south of Carfax. "A sprawling road that leads north to the Carfax. Dracula's choice of location is odd considering its proximity to the Asylum. Hopefully we can be one step ahead of him for once."
				
The Carfax is a room. The Carfax is north of the Essex Purfleet.
	Twenty-nine boxes of earth are in the Carfax.
	After player going to the Carfax:
		if Holmwood is in the Carfax begin;
			Now a rats are in the Carfax;
			say "You see a lot of boxes in the room, you're unsure of how many there are. There is an overwhelming stench in the chapel that would normally have lead you to leave. As you and your allies begin to take a step toward them the room begins to fill with rats! [paragraph break] You take a quick survey of what everyone has with them. [line break] ";
				     say "    Van Helsing has a cross and holy wafers with him.
			[line break]";
				    say "     Seward only has keys with him.
			[line break]";
				    say "     Holmwood has a silver whistle with him.
			[line break]";
				    say "     Morris has his pistol with him.
			";
			end if.
		
	Before player shooting pistol, say "It probably isn't a good idea to fire that in here."
	
	After player blowing silver whistle:
			say "You hear low grumbles as a group of dogs run in and chase away the rats[paragraph break]";
			Now rats are in the Secret Room;
			say "Van Helsing walks around the room and places a holy wafer in each box.  (There are only 21 boxes left to take care of).";
			Now number left is 21;
			say "[line break] You best return to the asylum and see if Mina has found out anything new.".
			
The London Road is a room. The London Road is south of the Essex Purfleet.
	After player going to London Road:
		if Rats are not in the Secret Room begin;
			say "You shouldn't be heading in this direction, Carfax is to the North";
			Move player to Essex Purfleet;
			end if.
			
Piccadilly is a Room. Piccadilly is west of the London Road. Dracula's House is south of Piccadilly.

	