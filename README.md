docker-postfix
==============

Simple postfix in a docker container to act as a relay to Office 365.

## Requirement
+ Docker 1.0

## Installation
1. Build image

	```bash
	$ sudo docker pull tmcadams222/postfix
	```

## Usage
1. Create postfix container with smtp authentication

	```bash
	$ sudo docker run -p 25:25 \
			-e maildomain=mail.example.com \
			--name postfix -d tmcadams222/postfix
	```

## Reference
+ TBD
