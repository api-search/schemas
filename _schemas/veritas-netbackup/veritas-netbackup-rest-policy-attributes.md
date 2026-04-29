---
description: Attributes of a NetBackup backup policy
layout: schema
name: PolicyAttributes
properties_list:
- description: Unique name of the policy
  name: policyName
  type: string
- description: The policy type defining the type of backup
  name: policyType
  type: string
- description: Whether the policy is currently active
  name: active
  type: boolean
- description: Date and time the policy becomes effective
  name: effectiveDate
  type: string
- description: Arguments for snapshot method if applicable
  name: snapshotMethodArgs
  type: string
- description: ''
  name: backupCopies
  type: object
- description: Job priority for this policy
  name: priority
  type: integer
- description: Keyword tag for the policy
  name: keyword
  type: string
- description: Data classification associated with this policy
  name: dataClassification
  type: string
provider_name: Veritas NetBackup
provider_slug: veritas-netbackup
schema_file: json-schema/veritas-netbackup-rest-policy-attributes-schema.json
slug: veritas-netbackup-rest-policy-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PolicyAttributes\",\n  \"type\": \"object\",\n  \"description\": \"Attributes of a NetBackup backup policy\",\n  \"properties\": {\n    \"policyName\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the policy\"\n    },\n    \"policyType\": {\n      \"type\": \"string\",\n      \"description\": \"The policy type defining the type of backup\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the policy is currently active\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time the policy becomes effective\"\n    },\n    \"snapshotMethodArgs\": {\n      \"type\": \"string\",\n      \"description\": \"Arguments for snapshot method if applicable\"\n    },\n    \"backupCopies\": {\n      \"type\": \"object\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Job priority for this policy\"\n    },\n    \"keyword\": {\n      \"type\": \"string\",\n      \"description\": \"Keyword tag for the policy\"\n    },\n    \"dataClassification\": {\n      \"type\": \"string\",\n      \"description\": \"Data classification associated with this policy\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/veritas-netbackup/refs/heads/main/json-schema/veritas-netbackup-rest-policy-attributes-schema.json
tags:
- Backup
- Data Protection
- Disaster Recovery
- Enterprise
- Recovery
- Storage
title: PolicyAttributes
---
