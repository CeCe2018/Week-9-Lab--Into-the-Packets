# Week-9-Lab--Into-the-Packets

#Milestone 0: Networking Toolbox

#Network Config Challenges

Run ifconfig/ipconfig/ip and determine the name/id of your primary network interface
What is your primary interface's IP address? Is it different from your public IP? Why or why not?
What is the MAC address of your primary interface?
Identify and understand your loopback interface



#Ping Challenges

What is the IP address of codepath.com? The IP address of codepath.com is 198.58.125.217.
What is the IP address of google.com? The IP address of google.com is 216.58.195.68.
Why would the IP address of google.com change between runs or from different locations? This is done to load-balance the traffic to different servers.

#Nslookup Challenges

Using the IP for codepath.com from the previous, pass it to nslookup
Does the domain returned from nslookup match? If not, why not? Yes, it matched the domain.

#traceroute Challenges
Compare the traceroutes for codepath.com and google.com
How many of the hops are the same?
What accounts for this?
Which has more hops? 
What accounts for the difference?

#Telnet Challenges

What's one thing that makes telnet insecure?
Can you telnet to codepath.com? What port is open and why?

Curl and Wget Challenges

Identify some differences between the two
Which would you be more likely to use for interacting with a RESTful API from the command line?
Which support recursive downloading?
Which are you more likely to find pre-installed on a Linux OS?
What is the syntax for each for downloading a file to the current directory?

SSH and SCP Challenges

Why is key authentication preferred to passwords?
What is the syntax for copying a file from a local folder to a remote one?

#Milestone 1: Security-Flavored Net Tools

#Challenge 1: Run nmap against your localhost IP to see all open ports

See how many of the ports you can match to services
Hint: try shutting down Docker or Virtualbox and re-running nmap

#Milestone 2: Grabbing Packets with tcpdump

#Challenge 1: Determine the IP address for codepath.com and use tcpdump to display packets with that IP as the destination. Then open http://www.codepath.com in the browser and check the output. Notice the output displays the HTTP requests in addition to the packets.

How many requests to load the main codepath.com page?
What type of resource accounts for most of the requests?
Now try the same exercise with https://security.codepath.com. What differences do you see in the output? What accounts for those differences?

#Challenge 2: You can also monitor DNS queries on port 53 with tcpdump. Use this to determine the IP of your primary DNS:

Listen for DNS queries on port 53: sudo tcpdump -vvv -s 0 -l -n port 53
Think of a domain name that probably exists (common word or phrase + .com) but that you've never visited before (suggestion: zombo.com) and open it in a browser
Look at the tcpdump output for the UDP packets trying to resolve the domain. The destination IP should be the DNS

#Milestone 3: Hello, Wireshark

#Milestone 4: Traffic Analysis — Mike's Computer is Acting Weird

#Milestone 5: Traffic Analysis — Mystery Meat Malware

#Milestone 6: Wi-Fi Hacking — Crack a Handshake

Milestone 7: Wi-Fi Hacking — Grab a Handshake
