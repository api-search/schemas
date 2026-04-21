---
description: Information about a crawl job.
layout: schema
name: JobInfo
properties_list:
- description: The unique job identifier.
  name: id
  type: string
- description: The type of Nutch crawl job.
  name: type
  type: string
- description: The configuration ID used for this job.
  name: confId
  type: string
- description: Arguments passed to the job.
  name: args
  type: object
- description: Result data returned after job completion.
  name: result
  type: object
- description: The current state of a job.
  name: state
  type: string
- description: A human-readable status or error message.
  name: msg
  type: string
- description: The crawl identifier associated with this job.
  name: crawlId
  type: string
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-job-info-schema.json
slug: apache-nutch-job-info
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: JobInfo
---
