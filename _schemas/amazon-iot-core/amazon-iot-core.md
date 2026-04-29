---
description: Schema defining the structure of an Amazon IoT Core thing resource, including attributes, thing type, thing group membership, certificates, and shadow state.
layout: schema
name: Amazon IoT Core Thing Definition
properties_list:
- description: The name of the thing.
  name: thingName
  type: string
- description: The unique identifier of the thing.
  name: thingId
  type: string
- description: The ARN of the thing.
  name: thingArn
  type: string
- description: The name of the thing type, if assigned.
  name: thingTypeName
  type: string
- description: A list of thing attributes as name-value pairs.
  name: attributes
  type: object
- description: The current version of the thing record.
  name: version
  type: integer
- description: The name of the billing group the thing belongs to.
  name: billingGroupName
  type: string
- description: The default MQTT client ID.
  name: defaultClientId
  type: string
- description: ''
  name: shadow
  type: object
- description: Certificates attached to the thing.
  name: certificates
  type: array
- description: Policies attached to the thing's certificates.
  name: policies
  type: array
- description: The thing groups the thing belongs to.
  name: thingGroups
  type: array
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/amazon-iot-core-schema.json
slug: amazon-iot-core
source_filename: amazon-iot-core-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.apievangelist.com/amazon-iot-core/thing-definition\",\n  \"title\": \"Amazon IoT Core Thing Definition\",\n  \"description\": \"Schema defining the structure of an Amazon IoT Core thing resource, including attributes, thing type, thing group membership, certificates, and shadow state.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"thingName\"\n  ],\n  \"properties\": {\n    \"thingName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the thing.\",\n      \"minLength\": 1,\n      \"maxLength\": 128,\n      \"pattern\": \"^[a-zA-Z0-9:_-]+$\"\n    },\n    \"thingId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the thing.\"\n    },\n    \"thingArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the thing.\"\n    },\n    \"thingTypeName\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The name of the thing type, if assigned.\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A list of thing attributes as name-value pairs.\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"The current version of the thing record.\"\n    },\n    \"billingGroupName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the billing group the thing belongs to.\"\n    },\n    \"defaultClientId\": {\n      \"type\": \"string\",\n      \"description\": \"The default MQTT client ID.\"\n    },\n    \"shadow\": {\n      \"$ref\": \"#/$defs/Shadow\"\n    },\n    \"certificates\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Certificate\"\n      },\n      \"description\": \"Certificates attached to the thing.\"\n    },\n    \"policies\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"\
  $ref\": \"#/$defs/Policy\"\n      },\n      \"description\": \"Policies attached to the thing's certificates.\"\n    },\n    \"thingGroups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The thing groups the thing belongs to.\"\n    }\n  },\n  \"$defs\": {\n    \"Shadow\": {\n      \"type\": \"object\",\n      \"description\": \"The device shadow state for the thing.\",\n      \"properties\": {\n        \"state\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"desired\": {\n              \"type\": \"object\",\n              \"additionalProperties\": true,\n              \"description\": \"The desired state of the thing.\"\n            },\n            \"reported\": {\n              \"type\": \"object\",\n              \"additionalProperties\": true,\n              \"description\": \"The reported state of the thing.\"\n            },\n            \"delta\": {\n              \"type\": \"\
  object\",\n              \"additionalProperties\": true,\n              \"description\": \"The difference between desired and reported state.\"\n            }\n          }\n        },\n        \"metadata\": {\n          \"type\": \"object\",\n          \"description\": \"Metadata about the shadow state.\"\n        },\n        \"version\": {\n          \"type\": \"integer\",\n          \"description\": \"The shadow version.\"\n        },\n        \"timestamp\": {\n          \"type\": \"integer\",\n          \"description\": \"The shadow timestamp.\"\n        }\n      }\n    },\n    \"Certificate\": {\n      \"type\": \"object\",\n      \"description\": \"An X.509 certificate for device authentication.\",\n      \"properties\": {\n        \"certificateId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the certificate.\"\n        },\n        \"certificateArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the certificate.\"\
  \n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ACTIVE\",\n            \"INACTIVE\",\n            \"REVOKED\",\n            \"PENDING_TRANSFER\",\n            \"REGISTER_INACTIVE\",\n            \"PENDING_ACTIVATION\"\n          ],\n          \"description\": \"The status of the certificate.\"\n        },\n        \"creationDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date the certificate was created.\"\n        }\n      }\n    },\n    \"Policy\": {\n      \"type\": \"object\",\n      \"description\": \"An IoT policy that defines allowed operations.\",\n      \"properties\": {\n        \"policyName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the policy.\"\n        },\n        \"policyArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the policy.\"\n        },\n        \"policyDocument\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"The JSON document that describes the policy.\"\n        },\n        \"defaultVersionId\": {\n          \"type\": \"string\",\n          \"description\": \"The default version of the policy.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/amazon-iot-core-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: Amazon IoT Core Thing Definition
---
