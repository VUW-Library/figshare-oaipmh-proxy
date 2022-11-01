# figshare-oaipmh-proxy
An httpd proxy to a single set in figshare's OAI-PMH feed 

# Why we use it
ALMA's OAI-PMH harvesting GUI interacts poorly (slowly) with the default figshare OAI-PMH feed. 
This appears to be related to the sheer number of sets in the feed, which ALMA downloads to 
populate a dropdown. 

# How it works
We use a Apache httpd server as a proxy, rewriting the URLs of figshare OAI-PMH feed to focus on 
the set we're interested in and only that set. 

No data is cached or stored locally, so the data is always 'live'. 

# How to use it
The proxy is a single file of Apache httpd configuration. It was developed in a linux / RHEL7 
context but is likely to work on other platfroms. Installation instructions appear at the top of 
the file. Some experience configuring Apache httpd is recommended, particularly if the server is 
serving other websites. 

