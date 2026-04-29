---
description: Details for updating an instance
layout: schema
name: UpdateInstanceDetails
properties_list:
- description: A user-friendly name. Does not have to be unique. Avoid entering confidential information.
  name: displayName
  type: string
- description: The shape of the instance. Changing the shape requires the instance to be stopped first.
  name: shape
  type: string
- description: Custom metadata key/value pairs
  name: metadata
  type: object
- description: Additional metadata key/value pairs
  name: extendedMetadata
  type: object
- description: The fault domain for the instance
  name: faultDomain
  type: string
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-update-instance-details-schema.json
slug: oci-compute-update-instance-details
source_filename: oci-compute-update-instance-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateInstanceDetails\",\n  \"type\": \"object\",\n  \"description\": \"Details for updating an instance\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly name. Does not have to be unique. Avoid entering confidential information.\"\n    },\n    \"shape\": {\n      \"type\": \"string\",\n      \"description\": \"The shape of the instance. Changing the shape requires the instance to be stopped first.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Custom metadata key/value pairs\"\n    },\n    \"extendedMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Additional metadata key/value pairs\"\n    },\n    \"faultDomain\": {\n      \"type\": \"string\",\n      \"description\": \"The fault domain for the instance\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-update-instance-details-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: UpdateInstanceDetails
---
