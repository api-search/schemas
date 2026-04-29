---
description: Program transition configuration.
layout: schema
name: Transition
properties_list:
- description: ''
  name: DurationMillis
  type: object
- description: ''
  name: RelativePosition
  type: object
- description: ''
  name: RelativeProgram
  type: object
- description: ''
  name: ScheduledStartTimeMillis
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-transition-schema.json
slug: mediatailor-api-transition
source_filename: mediatailor-api-transition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-transition-schema.json\",\n  \"title\": \"Transition\",\n  \"description\": \"Program transition configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DurationMillis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The duration of the live program in seconds.\"\n        }\n      ]\n    },\n    \"RelativePosition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelativePosition\"\n        },\n        {\n          \"description\": \"The position where this program will be inserted relative to the <code>RelativePosition</code>.\"\n        }\n      ]\n    },\n    \"RelativeProgram\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"description\": \"The name of the program that this program will be inserted next to, as defined by <code>RelativePosition</code>.\"\n        }\n      ]\n    },\n    \"ScheduledStartTimeMillis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The date and time that the program is scheduled to start, in epoch milliseconds.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>Defines when the program plays in the schedule. You can set the value to <code>ABSOLUTE</code> or <code>RELATIVE</code>.</p> <p> <code>ABSOLUTE</code> - The program plays at a specific wall clock time. This setting can only be used for channels using the <code>LINEAR</code> <code>PlaybackMode</code>.</p> <p>Note the following considerations when using <code>ABSOLUTE</code>\
  \ transitions:</p> <p>If the preceding program in the schedule has a duration that extends past the wall clock time, MediaTailor truncates the preceding program on a common segment boundary.</p> <p>If there are gaps in playback, MediaTailor plays the <code>FillerSlate</code> you configured for your linear channel.</p> <p> <code>RELATIVE</code> - The program is inserted into the schedule either before or after a program that you specify via <code>RelativePosition</code>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RelativePosition\",\n    \"Type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-transition-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Transition
---
