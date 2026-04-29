---
description: Information about an Direct Connect location.
layout: schema
name: Location
properties_list:
- description: ''
  name: locationCode
  type: object
- description: ''
  name: locationName
  type: object
- description: ''
  name: region
  type: object
- description: ''
  name: availablePortSpeeds
  type: object
- description: ''
  name: availableProviders
  type: object
- description: ''
  name: availableMacSecPortSpeeds
  type: object
provider_name: Amazon Direct Connect
provider_slug: amazon-direct-connect
schema_file: json-schema/amazon-direct-connect-location-schema.json
slug: amazon-direct-connect-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-location-schema.json\",\n  \"title\": \"Location\",\n  \"description\": \"Information about an Direct Connect location.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"locationCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationCode\"\n        },\n        {\n          \"description\": \"The code for the location.\"\n        }\n      ]\n    },\n    \"locationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationName\"\n        },\n        {\n          \"description\": \"The name of the location. This includes the name of the colocation partner and the physical site of the building.\"\n        }\n      ]\n    },\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Region\"\
  \n        },\n        {\n          \"description\": \"The Amazon Web Services Region for the location.\"\n        }\n      ]\n    },\n    \"availablePortSpeeds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailablePortSpeeds\"\n        },\n        {\n          \"description\": \"The available port speeds for the location.\"\n        }\n      ]\n    },\n    \"availableProviders\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProviderList\"\n        },\n        {\n          \"description\": \"The name of the service provider for the location.\"\n        }\n      ]\n    },\n    \"availableMacSecPortSpeeds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailableMacSecPortSpeeds\"\n        },\n        {\n          \"description\": \"The available MAC Security (MACsec) port speeds for the location.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-location-schema.json
tags:
- AWS
- Dedicated Connection
- Direct Connect
- Hybrid Cloud
- Networking
title: Location
---
