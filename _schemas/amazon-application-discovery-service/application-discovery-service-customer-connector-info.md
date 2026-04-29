---
description: CustomerConnectorInfo schema from Amazon Application Discovery Service API
layout: schema
name: CustomerConnectorInfo
properties_list:
- description: Number of active discovery connectors.
  name: activeConnectors
  type: integer
- description: Number of healthy discovery connectors.
  name: healthyConnectors
  type: integer
- description: Number of blacklisted discovery connectors.
  name: blackListedConnectors
  type: integer
- description: Number of discovery connectors with status SHUTDOWN.
  name: shutdownConnectors
  type: integer
- description: Number of unhealthy discovery connectors.
  name: unhealthyConnectors
  type: integer
- description: Total number of discovery connectors.
  name: totalConnectors
  type: integer
- description: Number of unknown discovery connectors.
  name: unknownConnectors
  type: integer
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-customer-connector-info-schema.json
slug: application-discovery-service-customer-connector-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-customer-connector-info-schema.json\",\n  \"title\": \"CustomerConnectorInfo\",\n  \"description\": \"CustomerConnectorInfo schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activeConnectors\": {\n      \"type\": \"integer\",\n      \"example\": 0,\n      \"description\": \"Number of active discovery connectors.\"\n    },\n    \"healthyConnectors\": {\n      \"type\": \"integer\",\n      \"example\": 0,\n      \"description\": \"Number of healthy discovery connectors.\"\n    },\n    \"blackListedConnectors\": {\n      \"type\": \"integer\",\n      \"example\": 0,\n      \"description\": \"Number of blacklisted discovery connectors.\"\n    },\n    \"shutdownConnectors\": {\n      \"type\": \"integer\"\
  ,\n      \"example\": 0,\n      \"description\": \"Number of discovery connectors with status SHUTDOWN.\"\n    },\n    \"unhealthyConnectors\": {\n      \"type\": \"integer\",\n      \"example\": 0,\n      \"description\": \"Number of unhealthy discovery connectors.\"\n    },\n    \"totalConnectors\": {\n      \"type\": \"integer\",\n      \"example\": 0,\n      \"description\": \"Total number of discovery connectors.\"\n    },\n    \"unknownConnectors\": {\n      \"type\": \"integer\",\n      \"example\": 0,\n      \"description\": \"Number of unknown discovery connectors.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-customer-connector-info-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: CustomerConnectorInfo
---
