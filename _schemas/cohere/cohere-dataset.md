---
description: Represents a dataset managed through the Cohere Datasets API, used for embed jobs, fine-tuning, and other batch processing tasks.
layout: schema
name: Cohere Dataset
properties_list:
- description: The unique identifier of the dataset.
  name: id
  type: string
- description: The human-readable name of the dataset.
  name: name
  type: string
- description: The type of dataset, which determines its schema and compatible operations.
  name: dataset_type
  type: string
- description: The current validation status of the dataset after upload.
  name: validation_status
  type: string
- description: The ISO 8601 timestamp when the dataset was created.
  name: created_at
  type: string
- description: The ISO 8601 timestamp when the dataset was last updated.
  name: updated_at
  type: string
- description: The expected schema definition for the dataset records.
  name: schema
  type: string
- description: The field names required in each record of the dataset.
  name: required_fields
  type: array
- description: The field names that are preserved through processing.
  name: preserve_fields
  type: array
- description: The error message if dataset validation failed.
  name: validation_error
  type: string
- description: Warning messages for rows that were dropped during validation.
  name: validation_warnings
  type: array
provider_name: cohere
provider_slug: cohere
schema_file: json-schema/cohere-dataset-schema.json
slug: cohere-dataset
tags: []
title: Cohere Dataset
---
