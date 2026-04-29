---
description: <p/>
layout: schema
name: EnableLoggingMessage
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: BucketName
  type: object
- description: ''
  name: S3KeyPrefix
  type: object
- description: ''
  name: LogDestinationType
  type: object
- description: ''
  name: LogExports
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-enable-logging-message-schema.json
slug: redshift-enable-logging-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"BucketName\": {},\n    \"S3KeyPrefix\": {},\n    \"LogDestinationType\": {},\n    \"LogExports\": {}\n  },\n  \"required\": [\n    \"ClusterIdentifier\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-enable-logging-message-schema.json\",\n  \"title\": \"EnableLoggingMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-enable-logging-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: EnableLoggingMessage
---
