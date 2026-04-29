---
description: BatchDisassociateScramSecretResponse schema from Amazon MSK API
layout: schema
name: BatchDisassociateScramSecretResponse
properties_list:
- description: ''
  name: ClusterArn
  type: object
- description: ''
  name: UnprocessedScramSecrets
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-batch-disassociate-scram-secret-response-schema.json
slug: msk-api-batch-disassociate-scram-secret-response
source_filename: msk-api-batch-disassociate-scram-secret-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-batch-disassociate-scram-secret-response-schema.json\",\n  \"title\": \"BatchDisassociateScramSecretResponse\",\n  \"description\": \"BatchDisassociateScramSecretResponse schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterArn\"\n          },\n          \"description\": \"\\n            <p>The Amazon Resource Name (ARN) of the cluster.</p>\"\n        }\n      ]\n    },\n    \"UnprocessedScramSecrets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfUnprocessedScramSecret\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"unprocessedScramSecrets\"\
  \n          },\n          \"description\": \"\\n            <p>List of errors when disassociating secrets to cluster.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-batch-disassociate-scram-secret-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BatchDisassociateScramSecretResponse
---
