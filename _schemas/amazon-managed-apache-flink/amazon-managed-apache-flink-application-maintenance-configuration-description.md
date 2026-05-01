---
description: The details of the maintenance configuration for the application.
layout: schema
name: ApplicationMaintenanceConfigurationDescription
properties_list:
- description: ''
  name: ApplicationMaintenanceWindowStartTime
  type: object
- description: ''
  name: ApplicationMaintenanceWindowEndTime
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-application-maintenance-configuration-description-schema.json
slug: amazon-managed-apache-flink-application-maintenance-configuration-description
source_filename: amazon-managed-apache-flink-application-maintenance-configuration-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-maintenance-configuration-description-schema.json\",\n  \"title\": \"ApplicationMaintenanceConfigurationDescription\",\n  \"description\": \"The details of the maintenance configuration for the application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationMaintenanceWindowStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationMaintenanceWindowStartTime\"\n        },\n        {\n          \"description\": \"The start time for the maintenance window.\"\n        }\n      ]\n    },\n    \"ApplicationMaintenanceWindowEndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationMaintenanceWindowEndTime\"\n        },\n        {\n          \"description\": \"\
  The end time for the maintenance window.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationMaintenanceWindowStartTime\",\n    \"ApplicationMaintenanceWindowEndTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-maintenance-configuration-description-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ApplicationMaintenanceConfigurationDescription
---
