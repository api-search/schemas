---
description: Represents the output of a DescribeLoggingConfiguration operation.
layout: schema
name: DescribeLoggingConfigurationResponse
properties_list:
- description: ''
  name: loggingConfiguration
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-describe-logging-configuration-response-schema.json
slug: amazon-managed-prometheus-describe-logging-configuration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-describe-logging-configuration-response-schema.json\",\n  \"title\": \"DescribeLoggingConfigurationResponse\",\n  \"description\": \"Represents the output of a DescribeLoggingConfiguration operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"loggingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingConfigurationMetadata\"\n        },\n        {\n          \"description\": \"Metadata object containing information about the logging configuration of a workspace.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"loggingConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-describe-logging-configuration-response-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: DescribeLoggingConfigurationResponse
---
