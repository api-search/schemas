---
description: Information about a fetched node in the FetchDB.
layout: schema
name: FetchNodeDbInfo
properties_list:
- description: The URL of the fetched node.
  name: url
  type: string
- description: The HTTP status code of the fetch.
  name: status
  type: integer
- description: The number of outgoing links discovered.
  name: numOfOutlinks
  type: integer
- description: The outgoing links from this node.
  name: children
  type: array
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-fetch-node-db-info-schema.json
slug: apache-nutch-fetch-node-db-info
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: FetchNodeDbInfo
---
