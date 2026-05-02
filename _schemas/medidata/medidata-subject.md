---
description: A trial subject enrolled in a Medidata Rave clinical study
layout: schema
name: Medidata Rave Clinical Trial Subject
properties_list:
- description: Unique subject identifier within the study (may be auto-generated)
  name: subjectKey
  type: string
- description: ID of the investigator site where the subject is enrolled
  name: siteID
  type: string
- description: ''
  name: siteName
  type: string
- description: Current enrollment status of the subject
  name: status
  type: string
- description: ''
  name: enrollmentDate
  type:
  - string
  - 'null'
- description: ''
  name: screeningDate
  type:
  - string
  - 'null'
- description: Subject initials (used in place of PII)
  name: initials
  type: string
- description: Parent study Object Identifier
  name: studyOID
  type: string
- description: Clinical events (visits) for this subject
  name: events
  type: array
provider_name: medidata
provider_slug: medidata
schema_file: json-schema/medidata-subject-schema.json
slug: medidata-subject
source_filename: medidata-subject-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/medidata/refs/heads/main/json-schema/medidata-subject-schema.json\",\n  \"title\": \"Medidata Rave Clinical Trial Subject\",\n  \"description\": \"A trial subject enrolled in a Medidata Rave clinical study\",\n  \"type\": \"object\",\n  \"required\": [\"subjectKey\", \"siteID\", \"status\"],\n  \"properties\": {\n    \"subjectKey\": {\n      \"type\": \"string\",\n      \"description\": \"Unique subject identifier within the study (may be auto-generated)\"\n    },\n    \"siteID\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the investigator site where the subject is enrolled\"\n    },\n    \"siteName\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Inactive\", \"Screened\", \"Failed\", \"Randomized\", \"Completed\", \"Withdrawn\"],\n      \"description\":\
  \ \"Current enrollment status of the subject\"\n    },\n    \"enrollmentDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\"\n    },\n    \"screeningDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\"\n    },\n    \"initials\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Subject initials (used in place of PII)\"\n    },\n    \"studyOID\": {\n      \"type\": \"string\",\n      \"description\": \"Parent study Object Identifier\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"Clinical events (visits) for this subject\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ClinicalEvent\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"ClinicalEvent\": {\n      \"type\": \"object\",\n      \"required\": [\"eventOID\"],\n      \"properties\": {\n        \"eventOID\": {\n          \"type\": \"string\",\n          \"description\": \"Event Object Identifier (visit definition OID)\"\
  \n        },\n        \"eventName\": {\n          \"type\": \"string\"\n        },\n        \"eventDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\"\n        },\n        \"repeatKey\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Repeat key for recurring events\"\n        },\n        \"forms\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/CRFForm\"\n          }\n        }\n      }\n    },\n    \"CRFForm\": {\n      \"type\": \"object\",\n      \"required\": [\"formOID\"],\n      \"properties\": {\n        \"formOID\": {\n          \"type\": \"string\"\n        },\n        \"formName\": {\n          \"type\": \"string\"\n        },\n        \"fields\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/CRFField\"\n          }\n        }\n      }\n    },\n    \"CRFField\": {\n      \"type\": \"object\",\n      \"required\": [\"fieldOID\"\
  ],\n      \"properties\": {\n        \"fieldOID\": {\n          \"type\": \"string\"\n        },\n        \"value\": {\n          \"type\": [\"string\", \"null\"]\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"NotStarted\", \"Saved\", \"Incomplete\", \"Complete\", \"Verified\", \"Signed\", \"Frozen\", \"Locked\"]\n        },\n        \"dataEntryDateTime\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\"\n        },\n        \"enteredBy\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/medidata/refs/heads/main/json-schema/medidata-subject-schema.json
tags: []
title: Medidata Rave Clinical Trial Subject
---
