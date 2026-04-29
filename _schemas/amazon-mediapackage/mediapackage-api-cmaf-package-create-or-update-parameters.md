---
description: A Common Media Application Format (CMAF) packaging configuration.
layout: schema
name: CmafPackageCreateOrUpdateParameters
properties_list:
- description: ''
  name: Encryption
  type: object
- description: ''
  name: HlsManifests
  type: object
- description: ''
  name: SegmentDurationSeconds
  type: object
- description: ''
  name: SegmentPrefix
  type: object
- description: ''
  name: StreamSelection
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-cmaf-package-create-or-update-parameters-schema.json
slug: mediapackage-api-cmaf-package-create-or-update-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-cmaf-package-create-or-update-parameters-schema.json\",\n  \"title\": \"CmafPackageCreateOrUpdateParameters\",\n  \"description\": \"A Common Media Application Format (CMAF) packaging configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Encryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafEncryption\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryption\"\n          }\n        }\n      ]\n    },\n    \"HlsManifests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfHlsManifestCreateOrUpdateParameters\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsManifests\"\n          },\n          \"description\": \"A list of HLS manifest configurations\"\
  \n        }\n      ]\n    },\n    \"SegmentDurationSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentDurationSeconds\"\n          },\n          \"description\": \"Duration (in seconds) of each segment. Actual segments will be\\nrounded to the nearest multiple of the source segment duration.\\n\"\n        }\n      ]\n    },\n    \"SegmentPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentPrefix\"\n          },\n          \"description\": \"An optional custom string that is prepended to the name of each segment. If not specified, it defaults to the ChannelId.\"\n        }\n      ]\n    },\n    \"StreamSelection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamSelection\"\n        },\n        {\n         \
  \ \"xml\": {\n            \"name\": \"streamSelection\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-cmaf-package-create-or-update-parameters-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CmafPackageCreateOrUpdateParameters
---
