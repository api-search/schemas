---
description: Parameters for a CrawlDB query.
layout: schema
name: DbQuery
properties_list:
- description: Configuration ID. Falls back to "default" if not provided.
  name: confId
  type: string
- description: The type of CrawlDB query to execute.
  name: type
  type: string
- description: Additional arguments for the query.
  name: args
  type: object
- description: The crawl identifier.
  name: crawlId
  type: string
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-db-query-schema.json
slug: apache-nutch-db-query
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: DbQuery
---
