# PowerDNS-Graylog
Extraction pattern to extract DNS query information from PowerDNS logs

## PowerDNS Logging
Within the pdns.conf file, enable logging with the following setting:
  
	log-dns-queries=yes	
	loglevel=5
	
## Graylog Input
Create a UDP Syslog input and send log data to that input

## Extractor
Apply the extractor from extractor.json to the graylog input, and have the logs processed

The important data will be exported from the raw logs and copied to the original query
