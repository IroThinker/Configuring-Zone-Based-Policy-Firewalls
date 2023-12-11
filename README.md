In this task, you will create a zone-based policy firewall on R3, making it act not only as a router but also as a firewall. 
R3 is currently responsible for routing packets for the three networks connected to it. R3’s interface roles are configured as follows:
Serial 0/0/1 is connected to the Internet. Because this is a public network, it is considered an untrusted network and should have the lowest security level.
G0/1 is connected to the internal network. Only authorized users have access to this network. In addition, vital institution resources also reside in this network. The internal network is to be considered a trusted network and should have the highest security level.
G0/0 is connected to a conference room. The conference room is used to host meetings with people who are not part of the organization.
The security policy to be enforced by R3 when it is acting as a firewall dictates that:


•	No traffic initiated from the Internet should be allowed into the internal or conference room networks.
•	Returning Internet traffic (return packets coming from the Internet into the R3 site, in response to requests originating from any of the R3 networks) should be allowed.
•	Computers in the R3 internal network are considered trusted and are allowed to initiate any type traffic (TCP, UDP or ICMP based traffic).
•	Computers in the R3 conference room network are considered untrusted and are allowed to initiate only web traffic (HTTP or HTTPS) to the Internet.
•	No traffic is allowed between the internal network and the conference room network. There is no guarantee regarding the condition of guest computers in the conference room network. •	Such machines could be infected with malware and might attempt to send out spam or other malicious traffic.
