---
description: Configuration for creating a new Nutch configuration.
layout: schema
name: NutchConfig
properties_list:
- description: The identifier for this configuration.
  name: configId
  type: string
- description: If true, overwrites an existing configuration with the same ID.
  name: force
  type: boolean
- description: Key-value pairs of Nutch configuration properties.
  name: params
  type: object
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-nutch-config-schema.json
slug: apache-nutch-nutch-config
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: NutchConfig
---
