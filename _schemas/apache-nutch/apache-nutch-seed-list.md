---
description: A named list of seed URLs.
layout: schema
name: SeedList
properties_list:
- description: The seed list identifier.
  name: id
  type: integer
- description: A human-readable name for this seed list.
  name: name
  type: string
- description: The HDFS path where the seed file is stored. Populated after creation.
  name: seedFilePath
  type: string
- description: The collection of seed URLs in this list.
  name: seedUrls
  type: array
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-seed-list-schema.json
slug: apache-nutch-seed-list
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: SeedList
---
