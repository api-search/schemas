---
description: Status information about the running Nutch server.
layout: schema
name: NutchServerInfo
properties_list:
- description: The date and time the server was started.
  name: startDate
  type: string
- description: Set of known configuration IDs.
  name: configuration
  type: array
- description: All jobs (any state).
  name: jobs
  type: array
- description: Currently running jobs.
  name: runningJobs
  type: array
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-nutch-server-info-schema.json
slug: apache-nutch-nutch-server-info
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: NutchServerInfo
---
