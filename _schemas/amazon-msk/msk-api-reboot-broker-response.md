---
description: RebootBrokerResponse schema from Amazon MSK API
layout: schema
name: RebootBrokerResponse
properties_list:
- description: ''
  name: ClusterArn
  type: object
- description: ''
  name: ClusterOperationArn
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-reboot-broker-response-schema.json
slug: msk-api-reboot-broker-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-reboot-broker-response-schema.json\",\n  \"title\": \"RebootBrokerResponse\",\n  \"description\": \"RebootBrokerResponse schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterArn\"\n          },\n          \"description\": \"\\n            <p>The Amazon Resource Name (ARN) of the cluster.</p>\"\n        }\n      ]\n    },\n    \"ClusterOperationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterOperationArn\"\n          },\n          \"description\": \"\\n            <p>The Amazon\
  \ Resource Name (ARN) of the cluster operation.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-reboot-broker-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: RebootBrokerResponse
---
