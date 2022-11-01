# figshare-oaipmh-proxy
An httpd proxy to a single set in figshare's OAI-PMH feed 

# Why we use it
ALMA's OAI-PMH harvesting GUI interacts poorly with the default figshare OAI-PMH feed. 

# How it works
We use a Apache httpd server as a proxy, rewriting the URLs of figshare OAI-PMH feed to focus on 
the set we're interested in. No data is cached or stored locally. 


