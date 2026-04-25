---
description: Schema representing a CDISC SDTM or ADaM dataset domain specification including all variables.
layout: schema
name: CDISC Dataset (Domain)
properties_list:
- description: Dataset/domain abbreviation (e.g., AE, CM, DM)
  name: name
  type: string
- description: Human-readable label for the dataset
  name: label
  type: string
- description: Detailed description of the dataset purpose and content
  name: description
  type: string
- description: SDTM general observation class
  name: datasetClass
  type: string
- description: Dataset structure (one record per subject, one record per visit, etc.)
  name: structure
  type: string
- description: 'Dataset purpose: Tabulation or Analysis'
  name: purpose
  type: string
- description: Key variables that uniquely identify a record
  name: keys
  type: array
- description: List of variables (columns) in the dataset
  name: variables
  type: array
- description: HAL hypermedia links
  name: _links
  type: object
provider_name: cdisc
provider_slug: cdisc
schema_file: json-schema/cdisc-dataset-schema.json
slug: cdisc-dataset
tags: []
title: CDISC Dataset (Domain)
---
