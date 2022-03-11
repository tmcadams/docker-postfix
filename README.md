docker-postfix
==============

Simple postfix in a docker container to act as a relay to another host

## Requirement
+ Docker 1.0

## Installation
1. Build image

	```bash
	$ sudo docker pull tmcadams222/tmcadams:latest
	```

## Usage
1. Create postfix container

	```bash
	$ sudo docker run -p 25:25 \
			-e maildomain=mail.example.com \
			-e relayhost=[mail.example.com]:25 \
			-e mynetworks=172.0.0.0/24,192.168.1.0/24 \
			--name postfix -d tmcadams222/tmcadams:latest
	```

## Reference
+ TBD
