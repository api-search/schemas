---
description: Schema representing a Contentstack content entry with its system metadata, localization properties, and workflow state. Entries are instances of content types and hold the actual content data for delivery via the Content Delivery API.
layout: schema
name: Contentstack Entry
properties_list:
- description: Unique identifier for the entry, assigned by Contentstack.
  name: uid
  type: string
- description: The primary title or name of the entry, typically mapped to the title field of the content type.
  name: title
  type: string
- description: The locale code for this entry (e.g., en-us, fr-fr, de-de). Follows BCP 47 language tag format.
  name: locale
  type: string
- description: Version number of the entry. Increments with each save. Published versions may differ from the current draft version.
  name: _version
  type: integer
- description: Indicates whether the entry is currently being processed (e.g., during a publish operation).
  name: _in_progress
  type: boolean
- description: UID of the user who originally created this entry.
  name: created_by
  type: string
- description: UID of the user who last updated this entry.
  name: updated_by
  type: string
- description: ISO 8601 UTC timestamp of when the entry was first created.
  name: created_at
  type: string
- description: ISO 8601 UTC timestamp of when the entry was last saved.
  name: updated_at
  type: string
- description: ISO 8601 UTC timestamp of when the entry was last published. Null if never published.
  name: published_at
  type: string
- description: Access control list defining role-level permissions for this entry.
  name: ACL
  type: object
- description: Arbitrary string tags associated with the entry for categorization and filtering.
  name: tags
  type: array
- description: ''
  name: _metadata
  type: object
- description: List of environments and locales where this entry is currently published.
  name: publish_details
  type: array
provider_name: contentstack
provider_slug: contentstack
schema_file: json-schema/contentstack-entry-schema.json
slug: contentstack-entry
source_filename: contentstack-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://contentstack.com/schemas/contentstack/entry.json\",\n  \"title\": \"Contentstack Entry\",\n  \"description\": \"Schema representing a Contentstack content entry with its system metadata, localization properties, and workflow state. Entries are instances of content types and hold the actual content data for delivery via the Content Delivery API.\",\n  \"type\": \"object\",\n  \"required\": [\"uid\", \"title\", \"locale\"],\n  \"properties\": {\n    \"uid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the entry, assigned by Contentstack.\",\n      \"pattern\": \"^[a-zA-Z0-9_-]+$\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The primary title or name of the entry, typically mapped to the title field of the content type.\",\n      \"minLength\": 1,\n      \"maxLength\": 1000\n    },\n    \"locale\": {\n      \"type\":\
  \ \"string\",\n      \"description\": \"The locale code for this entry (e.g., en-us, fr-fr, de-de). Follows BCP 47 language tag format.\",\n      \"pattern\": \"^[a-z]{2}(-[A-Z]{2})?$\",\n      \"examples\": [\"en-us\", \"fr-fr\", \"de-de\", \"ja-jp\"]\n    },\n    \"_version\": {\n      \"type\": \"integer\",\n      \"description\": \"Version number of the entry. Increments with each save. Published versions may differ from the current draft version.\",\n      \"minimum\": 1\n    },\n    \"_in_progress\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the entry is currently being processed (e.g., during a publish operation).\"\n    },\n    \"created_by\": {\n      \"type\": \"string\",\n      \"description\": \"UID of the user who originally created this entry.\"\n    },\n    \"updated_by\": {\n      \"type\": \"string\",\n      \"description\": \"UID of the user who last updated this entry.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n \
  \     \"format\": \"date-time\",\n      \"description\": \"ISO 8601 UTC timestamp of when the entry was first created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 UTC timestamp of when the entry was last saved.\"\n    },\n    \"published_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 UTC timestamp of when the entry was last published. Null if never published.\"\n    },\n    \"ACL\": {\n      \"type\": \"object\",\n      \"description\": \"Access control list defining role-level permissions for this entry.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/AclEntry\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Arbitrary string tags associated with the entry for categorization and filtering.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"maxLength\": 100\n      },\n \
  \     \"uniqueItems\": true\n    },\n    \"_metadata\": {\n      \"$ref\": \"#/$defs/EntryMetadata\"\n    },\n    \"publish_details\": {\n      \"type\": \"array\",\n      \"description\": \"List of environments and locales where this entry is currently published.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PublishDetail\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"AclEntry\": {\n      \"type\": \"object\",\n      \"description\": \"Access control permissions for a specific role.\",\n      \"properties\": {\n        \"read\": {\n          \"type\": \"boolean\",\n          \"description\": \"Permission to read this entry.\"\n        },\n        \"write\": {\n          \"type\": \"boolean\",\n          \"description\": \"Permission to create or update this entry.\"\n        },\n        \"delete\": {\n          \"type\": \"boolean\",\n          \"description\": \"Permission to delete this entry.\"\n        }\n      }\n    },\n    \"EntryMetadata\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"Workflow and editorial metadata for the entry.\",\n      \"properties\": {\n        \"workflow\": {\n          \"$ref\": \"#/$defs/WorkflowState\"\n        }\n      }\n    },\n    \"WorkflowState\": {\n      \"type\": \"object\",\n      \"description\": \"Current workflow stage assignment for the entry.\",\n      \"properties\": {\n        \"workflow\": {\n          \"type\": \"object\",\n          \"description\": \"Reference to the assigned workflow.\",\n          \"properties\": {\n            \"uid\": {\n              \"type\": \"string\",\n              \"description\": \"UID of the workflow.\"\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"Display name of the workflow.\"\n            }\n          }\n        },\n        \"workflow_stage\": {\n          \"type\": \"object\",\n          \"description\": \"Current stage within the workflow.\",\n          \"properties\": {\n            \"uid\"\
  : {\n              \"type\": \"string\",\n              \"description\": \"UID of the workflow stage.\"\n            },\n            \"title\": {\n              \"type\": \"string\",\n              \"description\": \"Display name of the workflow stage.\"\n            },\n            \"color\": {\n              \"type\": \"string\",\n              \"description\": \"Hex color code used to visually represent the workflow stage.\",\n              \"pattern\": \"^#[0-9A-Fa-f]{6}$\"\n            }\n          }\n        },\n        \"due_date\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Optional due date for completing this entry in the current workflow stage.\"\n        },\n        \"assigned_to\": {\n          \"type\": \"array\",\n          \"description\": \"List of users assigned to review this entry in the current stage.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n           \
  \   \"uid\": {\n                \"type\": \"string\",\n                \"description\": \"UID of the assigned user.\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Display name of the assigned user.\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"PublishDetail\": {\n      \"type\": \"object\",\n      \"description\": \"Publication state for an entry in a specific environment and locale.\",\n      \"properties\": {\n        \"environment\": {\n          \"type\": \"string\",\n          \"description\": \"UID of the environment where the entry is published.\"\n        },\n        \"locale\": {\n          \"type\": \"string\",\n          \"description\": \"Locale code of the published entry version.\"\n        },\n        \"time\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp of when the entry was published\
  \ to this environment.\"\n        },\n        \"user\": {\n          \"type\": \"string\",\n          \"description\": \"UID of the user who published the entry.\"\n        },\n        \"version\": {\n          \"type\": \"integer\",\n          \"description\": \"Version number of the entry that is published.\",\n          \"minimum\": 1\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/json-schema/contentstack-entry-schema.json
tags: []
title: Contentstack Entry
---
