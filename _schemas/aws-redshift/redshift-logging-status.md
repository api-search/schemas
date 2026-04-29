---
description: Describes the status of logging for a cluster.
layout: schema
name: LoggingStatus
properties_list:
- description: ''
  name: LoggingEnabled
  type: object
- description: ''
  name: BucketName
  type: object
- description: ''
  name: S3KeyPrefix
  type: object
- description: ''
  name: LastSuccessfulDeliveryTime
  type: object
- description: ''
  name: LastFailureTime
  type: object
- description: ''
  name: LastFailureMessage
  type: object
- description: ''
  name: LogDestinationType
  type: object
- description: ''
  name: LogExports
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-logging-status-schema.json
slug: redshift-logging-status
source_filename: redshift-logging-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"LoggingEnabled\": {},\n    \"BucketName\": {},\n    \"S3KeyPrefix\": {},\n    \"LastSuccessfulDeliveryTime\": {},\n    \"LastFailureTime\": {},\n    \"LastFailureMessage\": {},\n    \"LogDestinationType\": {},\n    \"LogExports\": {}\n  },\n  \"description\": \"Describes the status of logging for a cluster.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-logging-status-schema.json\",\n  \"title\": \"LoggingStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-logging-status-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: LoggingStatus
---
