---
description: A request to update a channel.
layout: schema
name: UpdateChannelRequest
properties_list:
- description: ''
  name: CdiInputSpecification
  type: object
- description: ''
  name: Destinations
  type: object
- description: ''
  name: EncoderSettings
  type: object
- description: ''
  name: InputAttachments
  type: object
- description: ''
  name: InputSpecification
  type: object
- description: ''
  name: LogLevel
  type: object
- description: ''
  name: Maintenance
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: RoleArn
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-update-channel-request-schema.json
slug: medialive-api-update-channel-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-channel-request-schema.json\",\n  \"title\": \"UpdateChannelRequest\",\n  \"description\": \"A request to update a channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CdiInputSpecification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CdiInputSpecification\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cdiInputSpecification\"\n          },\n          \"description\": \"Specification of CDI inputs for this channel\"\n        }\n      ]\n    },\n    \"Destinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfOutputDestination\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinations\"\n          },\n          \"description\": \"A list of output\
  \ destinations for this channel.\"\n        }\n      ]\n    },\n    \"EncoderSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncoderSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encoderSettings\"\n          },\n          \"description\": \"The encoder settings for this channel.\"\n        }\n      ]\n    },\n    \"InputAttachments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInputAttachment\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputAttachments\"\n          }\n        }\n      ]\n    },\n    \"InputSpecification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputSpecification\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputSpecification\"\n          },\n          \"description\": \"Specification of network and file inputs for this channel\"\n        }\n      ]\n    },\n   \
  \ \"LogLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogLevel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"logLevel\"\n          },\n          \"description\": \"The log level to write to CloudWatch Logs.\"\n        }\n      ]\n    },\n    \"Maintenance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaintenanceUpdateSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenance\"\n          },\n          \"description\": \"Maintenance settings for this channel.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the channel.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"roleArn\"\n          },\n          \"description\": \"An optional Amazon Resource Name (ARN) of the role to assume when running the Channel. If you do not specify this on an update call but the role was previously set that role will be removed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-channel-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateChannelRequest
---
