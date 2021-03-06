# Road Safety Initiative

The road safety initiative has data that is important for decision makers.

This project develops a system to ingest, validate and write road safety data into a business intelligence database for further analysis.  

At the present time, road safety data is made up of the following types of events:
- the issuance of a ticket
- the payment of a ticket
- the dispute of a ticket
- the query of a ticket record
- an update or resolution of a dispute


The system to handle these events is made up of four containers / pods:
- An ingestor that accepts events as JSON data
- A Message Broker that temporarily stores the events while they're being processed.
- A validator that checks each event to make sure it includes the required fields.
- A writer that inserts the data into a buiness intelligence database

# Development 

To begin local development of this project:
- create a `.env` file by copying `.env.sample` to `.env` in the root of the project directory
- edit the default values in the `.env` file to reflect your secret values.
- run `docker-compose build && docker-compose up` 





