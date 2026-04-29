---
description: Metadata describing a particular ephemeris.
layout: schema
name: EphemerisMetaData
properties_list:
- description: ''
  name: ephemerisId
  type: object
- description: ''
  name: epoch
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: source
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-ephemeris-meta-data-schema.json
slug: ground-station-ephemeris-meta-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-ephemeris-meta-data-schema.json\",\n  \"title\": \"EphemerisMetaData\",\n  \"description\": \"Metadata describing a particular ephemeris.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ephemerisId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"<p>UUID of a customer-provided ephemeris.</p> <p>This field is not populated for default ephemerides from Space Track.</p>\"\n        }\n      ]\n    },\n    \"epoch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"<p>The epoch of a default, ephemeris from Space Track in UTC.</p> <p>This field is not populated for customer-provided ephemerides.</p>\"\
  \n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SafeName\"\n        },\n        {\n          \"description\": \"<p>A name string associated with the ephemeris. Used as a human-readable identifier for the ephemeris.</p> <p>A name is only returned for customer-provider ephemerides that have a name associated.</p>\"\n        }\n      ]\n    },\n    \"source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EphemerisSource\"\n        },\n        {\n          \"description\": \"The <code>EphemerisSource</code> that generated a given ephemeris.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"source\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-ephemeris-meta-data-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: EphemerisMetaData
---
