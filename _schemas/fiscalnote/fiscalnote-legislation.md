---
description: A legislative measure such as a bill, resolution, or amendment tracked by FiscalNote across federal, state, and international jurisdictions.
layout: schema
name: FiscalNote Legislation
properties_list:
- description: Unique identifier for the legislation record.
  name: id
  type: string
- description: Official title of the legislation.
  name: title
  type: string
- description: Short or popular title of the legislation.
  name: shortTitle
  type: string
- description: Bill or resolution number such as HR 1234 or S 567.
  name: number
  type: string
- description: Type of legislation.
  name: type
  type: string
- description: Jurisdiction code where the legislation was introduced, such as US, US-CA, GB, or EU.
  name: jurisdiction
  type: string
- description: Legislative session identifier such as 118th Congress.
  name: session
  type: string
- description: Current status of the legislation.
  name: status
  type: string
- description: Date the legislation was introduced in ISO 8601 format.
  name: introducedDate
  type: string
- description: Date of the most recent action on the legislation.
  name: lastActionDate
  type: string
- description: Description of the most recent action taken.
  name: lastAction
  type: string
- description: List of sponsors and co-sponsors of the legislation.
  name: sponsors
  type: array
- description: Committees to which the legislation has been referred.
  name: committees
  type: array
- description: Subject tags associated with the legislation.
  name: subjects
  type: array
- description: Summary text of the legislation.
  name: summary
  type: string
- description: URL to the full text of the legislation.
  name: fullTextUrl
  type: string
- description: URL to the legislation record on the FiscalNote platform.
  name: url
  type: string
- description: Timestamp when the record was created in the system.
  name: createdAt
  type: string
- description: Timestamp when the record was last updated.
  name: updatedAt
  type: string
provider_name: FiscalNote
provider_slug: fiscalnote
schema_file: json-schema/fiscalnote-legislation-schema.json
slug: fiscalnote-legislation
source_filename: fiscalnote-legislation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://fiscalnote.com/schemas/fiscalnote/legislation.json\",\n  \"title\": \"FiscalNote Legislation\",\n  \"description\": \"A legislative measure such as a bill, resolution, or amendment tracked by FiscalNote across federal, state, and international jurisdictions.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"title\", \"jurisdiction\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the legislation record.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Official title of the legislation.\"\n    },\n    \"shortTitle\": {\n      \"type\": \"string\",\n      \"description\": \"Short or popular title of the legislation.\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Bill or resolution number such as HR 1234 or S 567.\"\n    },\n    \"type\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Type of legislation.\",\n      \"enum\": [\"bill\", \"resolution\", \"joint_resolution\", \"concurrent_resolution\", \"amendment\"]\n    },\n    \"jurisdiction\": {\n      \"type\": \"string\",\n      \"description\": \"Jurisdiction code where the legislation was introduced, such as US, US-CA, GB, or EU.\"\n    },\n    \"session\": {\n      \"type\": \"string\",\n      \"description\": \"Legislative session identifier such as 118th Congress.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the legislation.\",\n      \"enum\": [\"introduced\", \"in_committee\", \"passed_one_chamber\", \"passed_both_chambers\", \"enacted\", \"vetoed\"]\n    },\n    \"introducedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the legislation was introduced in ISO 8601 format.\"\n    },\n    \"lastActionDate\": {\n      \"type\": \"string\",\n   \
  \   \"format\": \"date\",\n      \"description\": \"Date of the most recent action on the legislation.\"\n    },\n    \"lastAction\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the most recent action taken.\"\n    },\n    \"sponsors\": {\n      \"type\": \"array\",\n      \"description\": \"List of sponsors and co-sponsors of the legislation.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Sponsor\"\n      }\n    },\n    \"committees\": {\n      \"type\": \"array\",\n      \"description\": \"Committees to which the legislation has been referred.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CommitteeRef\"\n      }\n    },\n    \"subjects\": {\n      \"type\": \"array\",\n      \"description\": \"Subject tags associated with the legislation.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"Summary text of the legislation.\"\n    },\n    \"fullTextUrl\":\
  \ {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the full text of the legislation.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the legislation record on the FiscalNote platform.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the record was created in the system.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the record was last updated.\"\n    }\n  },\n  \"$defs\": {\n    \"Sponsor\": {\n      \"type\": \"object\",\n      \"description\": \"A sponsor or co-sponsor of legislation.\",\n      \"required\": [\"id\", \"name\", \"role\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the sponsor.\"\n        },\n        \"\
  name\": {\n          \"type\": \"string\",\n          \"description\": \"Full name of the sponsor.\"\n        },\n        \"role\": {\n          \"type\": \"string\",\n          \"description\": \"Role of the sponsor.\",\n          \"enum\": [\"primary\", \"cosponsor\"]\n        },\n        \"party\": {\n          \"type\": \"string\",\n          \"description\": \"Political party affiliation.\"\n        },\n        \"jurisdiction\": {\n          \"type\": \"string\",\n          \"description\": \"Jurisdiction the sponsor represents.\"\n        }\n      }\n    },\n    \"CommitteeRef\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a legislative committee.\",\n      \"required\": [\"id\", \"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the committee.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the committee.\"\n\
  \        },\n        \"chamber\": {\n          \"type\": \"string\",\n          \"description\": \"Chamber the committee belongs to.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/json-schema/fiscalnote-legislation-schema.json
tags:
- Government
- Legislation
- Policy
- Political Intelligence
- Regulation
title: FiscalNote Legislation
---
