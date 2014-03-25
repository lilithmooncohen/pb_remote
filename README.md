# PB_Remote

This is a script to remotely execute scripts across multiple servers in elevated privileges via PowerBroker.

## WARNING

This will execute any script you tell it to **AS ROOT** on the remote server!
Be sure to check your scripts to make sure this will not do any damage.
You are liable for whatever you do!

## Use
Add the scripts you want to execute remotely to the 'scripts' folder.

Add the hostnames on which you want to run the script to the 'hosts' file.

Run pb_remote:
    ./pb_remote
	
Enter the name of you script:
    SCRIPT NAME: scriptname.sh
	
Enter your SSH username:
    SSH USERNAME: myname
	
Verify the list of hostnames shown. The script will then execute the script on the servers.

If a script is unable to execute remotely, the hostname will be logged to pb_remote.hosts.err

## Author
* Ryan C Koch (ryanckoch@gmail.com)