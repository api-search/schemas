---
description: GetBootstrapBrokersResponse schema from Amazon MSK API
layout: schema
name: GetBootstrapBrokersResponse
properties_list:
- description: ''
  name: BootstrapBrokerString
  type: object
- description: ''
  name: BootstrapBrokerStringTls
  type: object
- description: ''
  name: BootstrapBrokerStringSaslScram
  type: object
- description: ''
  name: BootstrapBrokerStringSaslIam
  type: object
- description: ''
  name: BootstrapBrokerStringPublicTls
  type: object
- description: ''
  name: BootstrapBrokerStringPublicSaslScram
  type: object
- description: ''
  name: BootstrapBrokerStringPublicSaslIam
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-get-bootstrap-brokers-response-schema.json
slug: msk-api-get-bootstrap-brokers-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-get-bootstrap-brokers-response-schema.json\",\n  \"title\": \"GetBootstrapBrokersResponse\",\n  \"description\": \"GetBootstrapBrokersResponse schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BootstrapBrokerString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bootstrapBrokerString\"\n          },\n          \"description\": \"\\n            <p>A string containing one or more hostname:port pairs.</p>\"\n        }\n      ]\n    },\n    \"BootstrapBrokerStringTls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bootstrapBrokerStringTls\"\n      \
  \    },\n          \"description\": \"\\n            <p>A string containing one or more DNS names (or IP) and TLS port pairs.</p>\"\n        }\n      ]\n    },\n    \"BootstrapBrokerStringSaslScram\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bootstrapBrokerStringSaslScram\"\n          },\n          \"description\": \"\\n            <p>A string containing one or more DNS names (or IP) and Sasl Scram port pairs.</p>\"\n        }\n      ]\n    },\n    \"BootstrapBrokerStringSaslIam\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bootstrapBrokerStringSaslIam\"\n          },\n          \"description\": \"\\n            <p>A string that contains one or more DNS names (or IP addresses) and SASL IAM port pairs.</p>\"\n        }\n      ]\n    },\n    \"BootstrapBrokerStringPublicTls\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bootstrapBrokerStringPublicTls\"\n          },\n          \"description\": \"\\n            <p>A string containing one or more DNS names (or IP) and TLS port pairs.</p>\"\n        }\n      ]\n    },\n    \"BootstrapBrokerStringPublicSaslScram\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bootstrapBrokerStringPublicSaslScram\"\n          },\n          \"description\": \"\\n            <p>A string containing one or more DNS names (or IP) and Sasl Scram port pairs.</p>\"\n        }\n      ]\n    },\n    \"BootstrapBrokerStringPublicSaslIam\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bootstrapBrokerStringPublicSaslIam\"\
  \n          },\n          \"description\": \"\\n            <p>A string that contains one or more DNS names (or IP addresses) and SASL IAM port pairs.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-get-bootstrap-brokers-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: GetBootstrapBrokersResponse
---
