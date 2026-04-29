---
description: UpdateClusterConfigurationRequest schema from Amazon MSK API
layout: schema
name: UpdateClusterConfigurationRequest
properties_list:
- description: ''
  name: ConfigurationInfo
  type: object
- description: ''
  name: CurrentVersion
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-update-cluster-configuration-request-schema.json
slug: msk-api-update-cluster-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-cluster-configuration-request-schema.json\",\n  \"title\": \"UpdateClusterConfigurationRequest\",\n  \"description\": \"UpdateClusterConfigurationRequest schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"configurationInfo\"\n          },\n          \"description\": \"\\n            <p>Represents the configuration that you want MSK to use for the brokers in a cluster.</p>\"\n        }\n      ]\n    },\n    \"CurrentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"currentVersion\"\n          },\n          \"description\": \"\\n            <p>The version of the cluster that needs to be updated.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CurrentVersion\",\n    \"ConfigurationInfo\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-cluster-configuration-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateClusterConfigurationRequest
---
