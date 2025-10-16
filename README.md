## project plan:

### 2 or more file inputs
- if only 2 file inputs use json and delimited format
-- we will use delimited data for batch processing
- if more than 2 file inputs, use multiple formats *for fun* (i.e. json, csv, tab)

### architecture needs
- we need two or more web services to support client / business partners application
- service will follow microservice architecture and expose data to http calls
- - proven through tests for every endpoint
  - fails properly with correct messaging
  - work properly returning good data
- each web service will need to receive data (posting of batch raw data or file submission)
- - will follow RESTful architecture guidance here
  - error messaging should be client application specific with internal logging for errors
- each service will need to read DTO type in, then process into an internal format *after validating DTO inputs*, then persist into cache or in-memory db
- validation for each received record is required
- inbound data format should not be echoed by internal format, DTO pattern used for inbound data
- internal data will eventually need to be processed into repository
- all behavior will be required to be proven through testing
- logging centrally - error / info logs
- produce input processing logging (records processed, records failed)






### we want to have each file represent data for a business process
- for example: application for service contract and inventory of widgets(something fun like cars, boats, medical supplies, organic farm to table produce)
- for example: medical services company that has inventory, employees, services, insured records
- or cargo ship management for international shipping company
- or transaction batch process for multiple transaction types: trade, account, exchange monies
- or your idea here .....

## examples built on the fly during session
- [Spring Restful Service with Couple of tests](https://github.com/beachedcoder/2025_14_10_demo_restful_spring)
