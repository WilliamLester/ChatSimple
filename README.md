# ChatSimple
Personal Project:

     Purpose:
     
          To Learn C++
          Develop strong OOP practice
          Better develop through git-like environments
          To begin development of features for future projects
          
     Program Outline:
     
               A simple chat program where NPCs, and users, can interact between each 
          other via chat messages relative to a simple time system. Actors, NPCs or users,
          can choose to interact by sending messages or wait. Program termination occurs when
          all users choose to exit.
          OPTIONAL: Save state on exit and load prior exit-state
          
          specifics:
               
               There can be zero or more NPCs.
               There can be one or more Users.
               There can be zero or more discussions
          
     Definitions:
     
          Actor:
          An user or a NPC.
          
          NPC:
          "Non-player character", cumpter controlled entity that randomly selects actions and types non-sense messages.
          
          User:
          Stdin, keyboard input.
          
          Time System:
          Standard turn system, all actors must wait for all actors to choose an action. The actions are then
          carried out while the actors busy wait for the next time they can choose. A time cycle is considered
          a 'turn', a period comprised of actors choosing their action and the carring out of that choice.
          
          Action:
          Committed by actors once every time cycle. Actors may choose to leave the current discussion group,
          send a message, wait, or exit program. Leaving the discussion group can only be done while in a discussion group.
          
          Wait:
          Idle/do nothing this time cycle.
          
          Messages:
          Messages may be send by actors. Messages contain a sender, reciever, and text block.
          Messages can only be received by actors in the same discussion group. If the
          senter/receiver are not in the same discussion group, then both are placed in the same
          discussion group and the messages are recieved. They have an unlimited length.
          Users may type their messages.
          
          Discussion Groups:
          Interactions are encapsulated by discussion groups. A discussion group is created and 
          maintained by two, or more, actors sending/recieving messages to/from the other(s). Actors may choose to continue
          sending messages, leave the discussion group, or wait. When a discussion group contains one 
          actor, or less, then it ceases to exist. An actor may not start a new discussion without first
          leaving the current discussion.
