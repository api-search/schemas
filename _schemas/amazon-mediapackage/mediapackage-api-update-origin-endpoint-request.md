---
description: Configuration parameters used to update an existing OriginEndpoint.
layout: schema
name: UpdateOriginEndpointRequest
properties_list:
- description: ''
  name: Authorization
  type: object
- description: ''
  name: CmafPackage
  type: object
- description: ''
  name: DashPackage
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: HlsPackage
  type: object
- description: ''
  name: ManifestName
  type: object
- description: ''
  name: MssPackage
  type: object
- description: ''
  name: Origination
  type: object
- description: ''
  name: StartoverWindowSeconds
  type: object
- description: ''
  name: TimeDelaySeconds
  type: object
- description: ''
  name: Whitelist
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-update-origin-endpoint-request-schema.json
slug: mediapackage-api-update-origin-endpoint-request
source_filename: mediapackage-api-update-origin-endpoint-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-update-origin-endpoint-request-schema.json\",\n  \"title\": \"UpdateOriginEndpointRequest\",\n  \"description\": \"Configuration parameters used to update an existing OriginEndpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Authorization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Authorization\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"authorization\"\n          }\n        }\n      ]\n    },\n    \"CmafPackage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafPackageCreateOrUpdateParameters\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cmafPackage\"\n          }\n        }\n      ]\n    },\n    \"DashPackage\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/DashPackage\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dashPackage\"\n          }\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"A short text description of the OriginEndpoint.\"\n        }\n      ]\n    },\n    \"HlsPackage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsPackage\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsPackage\"\n          }\n        }\n      ]\n    },\n    \"ManifestName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestName\"\n          },\n          \"description\": \"A short string that will be\
  \ appended to the end of the Endpoint URL.\"\n        }\n      ]\n    },\n    \"MssPackage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MssPackage\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mssPackage\"\n          }\n        }\n      ]\n    },\n    \"Origination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Origination\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"origination\"\n          },\n          \"description\": \"Control whether origination of video is allowed for this OriginEndpoint. If set to ALLOW, the OriginEndpoint\\nmay by requested, pursuant to any other form of access control. If set to DENY, the OriginEndpoint may not be\\nrequested. This can be helpful for Live to VOD harvesting, or for temporarily disabling origination\\n\"\n        }\n      ]\n    },\n    \"StartoverWindowSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"startoverWindowSeconds\"\n          },\n          \"description\": \"Maximum duration (in seconds) of content to retain for startover playback.\\nIf not specified, startover playback will be disabled for the OriginEndpoint.\\n\"\n        }\n      ]\n    },\n    \"TimeDelaySeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timeDelaySeconds\"\n          },\n          \"description\": \"Amount of delay (in seconds) to enforce on the playback of live content.\\nIf not specified, there will be no time delay in effect for the OriginEndpoint.\\n\"\n        }\n      ]\n    },\n    \"Whitelist\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"whitelist\"\n          },\n          \"description\"\
  : \"A list of source IP CIDR blocks that will be allowed to access the OriginEndpoint.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-update-origin-endpoint-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: UpdateOriginEndpointRequest
---
