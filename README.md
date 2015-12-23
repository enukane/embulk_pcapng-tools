embulk\_pcapng-tools
----

tools to convert embulk config that includes embulk-inpug-pcapng-files into each schema on different DB.
Currently it supports

 - BigQuery (pcapng2bigquery)
 - ElasticSearch (pcapng2elasticsearch)
 - PostgreSQL (pcapng2pgsql)


### usage

```
% pcapng2XXXX -i input [-o output] [DB specific options]
```

- DB independent options
  - -i: input file (config.yml)
  - -o: output file (stdout if unspecified)
  - -h: show help
- DB dependent options
  - ElasticSearch (pcapng2elasticsearch)
    - -I: specify index name
  - PostgreSQL (pcapng2pgsql)
    - -t: specify table name
