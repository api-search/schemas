---
description: An Apify Actor run execution.
layout: schema
name: Run
properties_list:
- description: Run ID.
  name: id
  type: string
- description: Actor ID.
  name: actId
  type: string
- description: Run status.
  name: status
  type: string
- description: Run start time.
  name: startedAt
  type: string
- description: Run finish time.
  name: finishedAt
  type: string
- description: ID of the default dataset for this run.
  name: defaultDatasetId
  type: string
provider_name: Apify
provider_slug: apify
schema_file: json-schema/apify-run-schema.json
slug: apify-run
tags:
- Actors
- Browser Automation
- Crawling
- Data Aggregation
- Data Extraction
- Web Automation
- Web Scraping
title: Run
---
