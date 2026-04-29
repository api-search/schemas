---
description: ''
layout: schema
name: PutTableMaintenanceConfigurationRequest
properties_list:
- description: The type of maintenance configuration.
  name: type
  type: string
- description: ''
  name: value
  type: object
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-tables-put-table-maintenance-configuration-request-schema.json
slug: amazon-s3-tables-put-table-maintenance-configuration-request
source_filename: amazon-s3-tables-put-table-maintenance-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PutTableMaintenanceConfigurationRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of maintenance configuration.\"\n    },\n    \"value\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-tables-put-table-maintenance-configuration-request-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: PutTableMaintenanceConfigurationRequest
---
