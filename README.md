# ES_Dev

Development Elastic stack installation, as a proof of concept.

Installed Elasticsearch on a 3 virtual node cluster, running Centos 7.

Elasticsearch:
  Installed elasticsearch on 3 nodes.
  elasticsearch.yml configured to create a 3 node cluster.
  
Logstash:
  Configured LS_Syslog.conf, to retrieve syslog file as input.
  Used grok filtering to filter out timestamps and messages etc.  
  Output the results into appropriate index in Elasticsearch.
  
Kibana:
  Installed and configured on only one node.
  Configure kibana.yml with appropriate ports.
  
Beats:
  Filebeat:  
    installed and configured filebeat on client device to ship data into elasticseach.
  Topbeat:
    installed and configured topbeat on client device to ship data into logstash.
  Winlogbeat:
    installed and configured winlogbeat on client device to ship data into logstash.
    
Syslog-ng:
  installed and configured syslog-ng to store incoming syslog data into desired file.
  



