---
description: UpdateApplicationMaintenanceConfigurationResponse schema from Amazon Managed Service for Apache Flink API
layout: schema
name: UpdateApplicationMaintenanceConfigurationResponse
properties_list:
- description: ''
  name: ApplicationARN
  type: object
- description: ''
  name: ApplicationMaintenanceConfigurationDescription
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-update-application-maintenance-configuration-response-schema.json
slug: amazon-managed-apache-flink-update-application-maintenance-configuration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-update-application-maintenance-configuration-response-schema.json\",\n  \"title\": \"UpdateApplicationMaintenanceConfigurationResponse\",\n  \"description\": \"UpdateApplicationMaintenanceConfigurationResponse schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the application.\"\n        }\n      ]\n    },\n    \"ApplicationMaintenanceConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationMaintenanceConfigurationDescription\"\n        },\n        {\n\
  \          \"description\": \"The application maintenance configuration description after the update.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-update-application-maintenance-configuration-response-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: UpdateApplicationMaintenanceConfigurationResponse
---
