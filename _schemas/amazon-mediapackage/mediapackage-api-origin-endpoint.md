---
description: An OriginEndpoint resource configuration.
layout: schema
name: OriginEndpoint
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Authorization
  type: object
- description: ''
  name: ChannelId
  type: object
- description: ''
  name: CmafPackage
  type: object
- description: ''
  name: CreatedAt
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
  name: Id
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
  name: Tags
  type: object
- description: ''
  name: TimeDelaySeconds
  type: object
- description: ''
  name: Url
  type: object
- description: ''
  name: Whitelist
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-origin-endpoint-schema.json
slug: mediapackage-api-origin-endpoint
source_filename: mediapackage-api-origin-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-origin-endpoint-schema.json\",\n  \"title\": \"OriginEndpoint\",\n  \"description\": \"An OriginEndpoint resource configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) assigned to the OriginEndpoint.\"\n        }\n      ]\n    },\n    \"Authorization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Authorization\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"authorization\"\n          }\n        }\n      ]\n    },\n    \"ChannelId\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelId\"\n          },\n          \"description\": \"The ID of the Channel the OriginEndpoint is associated with.\"\n        }\n      ]\n    },\n    \"CmafPackage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafPackage\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cmafPackage\"\n          }\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"createdAt\"\n          },\n          \"description\": \"The date and time the OriginEndpoint was created.\"\n        }\n      ]\n    },\n    \"DashPackage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DashPackage\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"dashPackage\"\n          }\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"A short text description of the OriginEndpoint.\"\n        }\n      ]\n    },\n    \"HlsPackage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsPackage\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsPackage\"\n          }\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The ID of the OriginEndpoint.\"\n        }\n      ]\n    },\n    \"ManifestName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestName\"\n          },\n          \"description\": \"A short string appended to the end of the OriginEndpoint URL.\"\n        }\n      ]\n    },\n    \"MssPackage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MssPackage\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mssPackage\"\n          }\n        }\n      ]\n    },\n    \"Origination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Origination\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"origination\"\n          },\n          \"description\": \"Control whether origination of video is allowed for this OriginEndpoint. If set to ALLOW, the OriginEndpoint\\nmay by requested, pursuant to any other form of access control. If set to DENY, the OriginEndpoint may not be\\nrequested. This can be helpful for Live to VOD harvesting, or for temporarily disabling\
  \ origination\\n\"\n        }\n      ]\n    },\n    \"StartoverWindowSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"startoverWindowSeconds\"\n          },\n          \"description\": \"Maximum duration (seconds) of content to retain for startover playback.\\nIf not specified, startover playback will be disabled for the OriginEndpoint.\\n\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          }\n        }\n      ]\n    },\n    \"TimeDelaySeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timeDelaySeconds\"\n          },\n          \"description\": \"Amount of delay (seconds) to enforce on the\
  \ playback of live content.\\nIf not specified, there will be no time delay in effect for the OriginEndpoint.\\n\"\n        }\n      ]\n    },\n    \"Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"url\"\n          },\n          \"description\": \"The URL of the packaged OriginEndpoint for consumption.\"\n        }\n      ]\n    },\n    \"Whitelist\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"whitelist\"\n          },\n          \"description\": \"A list of source IP CIDR blocks that will be allowed to access the OriginEndpoint.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-origin-endpoint-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: OriginEndpoint
---
