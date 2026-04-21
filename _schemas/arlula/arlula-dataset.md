---
description: A dataset produced from a campaign containing downloadable resources.
layout: schema
name: Dataset
properties_list:
- description: Dataset identifier.
  name: datasetId
  type: string
- description: Parent campaign identifier.
  name: campaignId
  type: string
- description: Dataset status.
  name: status
  type: string
- description: ''
  name: resources
  type: array
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-dataset-schema.json
slug: arlula-dataset
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: Dataset
---
