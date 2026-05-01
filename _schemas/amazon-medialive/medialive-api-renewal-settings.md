---
description: The Renewal settings for Reservations
layout: schema
name: RenewalSettings
properties_list:
- description: ''
  name: AutomaticRenewal
  type: object
- description: ''
  name: RenewalCount
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-renewal-settings-schema.json
slug: medialive-api-renewal-settings
source_filename: medialive-api-renewal-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-renewal-settings-schema.json\",\n  \"title\": \"RenewalSettings\",\n  \"description\": \"The Renewal settings for Reservations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutomaticRenewal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservationAutomaticRenewal\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"automaticRenewal\"\n          },\n          \"description\": \"Automatic renewal status for the reservation\"\n        }\n      ]\n    },\n    \"RenewalCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"renewalCount\"\n          },\n          \"description\": \"Count for the reservation renewal\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-renewal-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: RenewalSettings
---
