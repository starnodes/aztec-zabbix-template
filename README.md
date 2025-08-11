# Aztec Zabbix Template

Aztec Node Monitoring

Hey guys!  
This template for Zabbix Server can help you monitor your Aztec node.  
Just change the macro and set up the IP address and port of your node.

**Macro example:**  
`{$SERVER_URL} = http://88.88.88.88:8080`

## What does my template monitor?

1. **Node availability** – The template checks the node on port `8080`.  
   If the port is not responding → the node is considered down.
2. **Sync status** – If the synchronization differs from AztecScan by more than 3 blocks → the trigger is activated.
