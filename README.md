# CommandTestSuite
A client-side application running off network tables to easily test commands without joystick mapping

# Justification
Testing the slew of commands a team has can possibly be very tiring, becuase mapping to buttons is annoying, and remembering the button maps its impossible, resulting in a back and forth process of looking up commands in RobotMap after just opening back up the driver station.

# Goal
This Application is a client-side application which communicates to the Robot Program through the network tables and a utility in TinManLib.  At load-up time, the app will send a list of commands to the client, which will display them.  When one wants to test a command, they simply chose the command to run, then give the arguments to test it with, with the option to interrupt the command at any time.  It will detect realtime when commands have stopped and which are still running.  There is no limit to the number of simultaneous commands, but those which 'require' the same subsystem will still interrupt eachother.
