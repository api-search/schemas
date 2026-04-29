---
description: UpdateApplicationMaintenanceConfigurationRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: UpdateApplicationMaintenanceConfigurationRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: ApplicationMaintenanceConfigurationUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-update-application-maintenance-configuration-request-schema.json
slug: amazon-managed-apache-flink-update-application-maintenance-configuration-request
source_filename: amazon-managed-apache-flink-update-application-maintenance-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-update-application-maintenance-configuration-request-schema.json\",\n  \"title\": \"UpdateApplicationMaintenanceConfigurationRequest\",\n  \"description\": \"UpdateApplicationMaintenanceConfigurationRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of the application for which you want to update the maintenance configuration.\"\n        }\n      ]\n    },\n    \"ApplicationMaintenanceConfigurationUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationMaintenanceConfigurationUpdate\"\
  \n        },\n        {\n          \"description\": \"Describes the application maintenance configuration update.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationName\",\n    \"ApplicationMaintenanceConfigurationUpdate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-update-application-maintenance-configuration-request-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: UpdateApplicationMaintenanceConfigurationRequest
---
