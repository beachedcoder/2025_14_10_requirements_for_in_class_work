## project plan:

### 2 or more file inputs
- if only 2 file inputs use two different file formats (i.e. json,delimited)
- if more than 2 file inputs, use multiple formats (i.e. json, csv, tab)

### we want to have each file represent data for a business process
- for example: application for service contract and inventory of widgets(something fun)
- for example: medical services company that has inventory, employees, services, insured records
- or cargo ship management for international shipping company
- or transaction batch process for multiple transaction types: trade, account, exchange monies
- or your idea here .....

### architecture needs
- we need two or more web services to support client / business partners application
- each web service will need to receive data (posting of batch raw data or file submission)
- each service will need to then process into an internal format (fake company domain data structure to share within fake company applications)
- validation for each received record is required
