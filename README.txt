
Treasure hunt game with NAO robot. Uses julius for voice interface and OpenCV for vision.
Running in Ubuntu 14.04

USAGE


##########################################
# 	Setting Up Voice interface	 #
##########################################

- Configure Julius by going to julius folder and following the README
(big thanks to https://github.com/Dayof)

- Go to the voiceControll folder and run 
	$ ./build.sh

- Run 
	$ ./test

- Open another terminal and go to julius folder, there you will run 
	$ julius -quiet -input mic -C julius.jconf 2>/dev/null | ./../voiceControl/commandModule

- Say "Quente", "Frio" ou "chegou". You shoud see the command arriving on the test terminal.

#########################################
#		NAO			#
#########################################

- Must be configured with NAOqi 2.1

- Run 
	$ build_all.sh

-Connect NAO and run
	$ send_all.sh <your robot's IP>

- Access robot though SSH and go to naoqi folder. There run 
	$ ./TreasureHunt

