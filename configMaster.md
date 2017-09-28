# Set up Github keys

## Create a key pair

	sh-keygen -t rsa -b 4096 -C "your_email@example.com"

## Add the private key to your sssh agent

	ssh-add -K ~/.ssh/id_rsa

## Upload the public key to your github account

	id_rsa.pub 

### You can use xclip to copy the contents to clipboard

	xclip -sel clip < ~/.ssh/id_rsa.pub

## Setup your git repo as SSH instead of https 
