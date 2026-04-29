---
description: MediaPackage Output Destination Settings
layout: schema
name: MediaPackageOutputDestinationSettings
properties_list:
- description: ''
  name: ChannelId
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-media-package-output-destination-settings-schema.json
slug: medialive-api-media-package-output-destination-settings
source_filename: medialive-api-media-package-output-destination-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-media-package-output-destination-settings-schema.json\",\n  \"title\": \"MediaPackageOutputDestinationSettings\",\n  \"description\": \"MediaPackage Output Destination Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChannelId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelId\"\n          },\n          \"description\": \"ID of the channel in MediaPackage that is the destination for this output group. You do not need to specify the individual inputs in MediaPackage; MediaLive will handle the connection of the two MediaLive pipelines to the two MediaPackage inputs. The MediaPackage channel and MediaLive channel must be in the same region.\"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-media-package-output-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MediaPackageOutputDestinationSettings
---
