---
description: Describes the updated maintenance configuration for the application.
layout: schema
name: ApplicationMaintenanceConfigurationUpdate
properties_list:
- description: ''
  name: ApplicationMaintenanceWindowStartTimeUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-application-maintenance-configuration-update-schema.json
slug: amazon-managed-apache-flink-application-maintenance-configuration-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-maintenance-configuration-update-schema.json\",\n  \"title\": \"ApplicationMaintenanceConfigurationUpdate\",\n  \"description\": \"Describes the updated maintenance configuration for the application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationMaintenanceWindowStartTimeUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationMaintenanceWindowStartTime\"\n        },\n        {\n          \"description\": \"The updated start time for the maintenance window.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationMaintenanceWindowStartTimeUpdate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-maintenance-configuration-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ApplicationMaintenanceConfigurationUpdate
---
