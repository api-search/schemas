---
description: The properties for a VPC type input destination.
layout: schema
name: InputDestinationVpc
properties_list:
- description: ''
  name: AvailabilityZone
  type: object
- description: ''
  name: NetworkInterfaceId
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-destination-vpc-schema.json
slug: medialive-api-input-destination-vpc
source_filename: medialive-api-input-destination-vpc-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-destination-vpc-schema.json\",\n  \"title\": \"InputDestinationVpc\",\n  \"description\": \"The properties for a VPC type input destination.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailabilityZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"availabilityZone\"\n          },\n          \"description\": \"The availability zone of the Input destination.\\n\"\n        }\n      ]\n    },\n    \"NetworkInterfaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkInterfaceId\"\n          },\n          \"description\": \"The network interface\
  \ ID of the Input destination in the VPC.\\n\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-destination-vpc-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputDestinationVpc
---
