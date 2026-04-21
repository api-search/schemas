---
description: Configuration for creating a new crawl job.
layout: schema
name: JobConfig
properties_list:
- description: The crawl identifier.
  name: crawlId
  type: string
- description: The type of Nutch crawl job.
  name: type
  type: string
- description: The configuration ID to use for this job. Defaults to "default" if not specified.
  name: confId
  type: string
- description: Fully qualified class name when type is CLASS.
  name: jobClassName
  type: string
- description: Additional arguments for the job.
  name: args
  type: object
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-job-config-schema.json
slug: apache-nutch-job-config
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: JobConfig
---
