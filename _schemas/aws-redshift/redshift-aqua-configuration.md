---
description: The operation that uses this structure is retired. Amazon Redshift automatically determines whether to use AQUA (Advanced Query Accelerator).
layout: schema
name: AquaConfiguration
properties_list:
- description: ''
  name: AquaStatus
  type: object
- description: ''
  name: AquaConfigurationStatus
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-aqua-configuration-schema.json
slug: redshift-aqua-configuration
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AquaStatus\": {},\n    \"AquaConfigurationStatus\": {}\n  },\n  \"description\": \"The operation that uses this structure is retired. Amazon Redshift automatically determines whether to use AQUA (Advanced Query Accelerator).\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-aqua-configuration-schema.json\",\n  \"title\": \"AquaConfiguration\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-aqua-configuration-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: AquaConfiguration
---
