---
description: Schema representing a Contentstack stack, which is an independent content repository within an organization. Stacks contain all content types, entries, assets, environments, and configuration for a digital experience project.
layout: schema
name: Contentstack Stack
properties_list:
- description: The unique API key that identifies this stack. Used as the primary authentication credential for Content Management and Content Delivery API requests.
  name: api_key
  type: string
- description: Internal unique identifier for the stack.
  name: uid
  type: string
- description: Human-readable display name of the stack.
  name: name
  type: string
- description: Optional description of the stack's purpose and contents.
  name: description
  type: string
- description: The default locale code for the stack. All content must have a version in the master locale before it can be localized to other locales.
  name: master_locale
  type: string
- description: UID of the organization that owns this stack.
  name: org_uid
  type: string
- description: Identifier of the Contentstack subscription plan for this stack.
  name: plan_id
  type: string
- description: ''
  name: settings
  type: object
- description: UID of the user who created the stack.
  name: created_by
  type: string
- description: UID of the user who last modified stack settings.
  name: updated_by
  type: string
- description: ISO 8601 UTC timestamp of when the stack was created.
  name: created_at
  type: string
- description: ISO 8601 UTC timestamp of when the stack settings were last updated.
  name: updated_at
  type: string
provider_name: contentstack
provider_slug: contentstack
schema_file: json-schema/contentstack-stack-schema.json
slug: contentstack-stack
source_filename: contentstack-stack-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://contentstack.com/schemas/contentstack/stack.json\",\n  \"title\": \"Contentstack Stack\",\n  \"description\": \"Schema representing a Contentstack stack, which is an independent content repository within an organization. Stacks contain all content types, entries, assets, environments, and configuration for a digital experience project.\",\n  \"type\": \"object\",\n  \"required\": [\"api_key\", \"name\", \"master_locale\", \"org_uid\"],\n  \"properties\": {\n    \"api_key\": {\n      \"type\": \"string\",\n      \"description\": \"The unique API key that identifies this stack. Used as the primary authentication credential for Content Management and Content Delivery API requests.\",\n      \"pattern\": \"^[a-zA-Z0-9]{16,}$\"\n    },\n    \"uid\": {\n      \"type\": \"string\",\n      \"description\": \"Internal unique identifier for the stack.\"\n    },\n    \"name\": {\n      \"type\":\
  \ \"string\",\n      \"description\": \"Human-readable display name of the stack.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the stack's purpose and contents.\",\n      \"maxLength\": 2000\n    },\n    \"master_locale\": {\n      \"type\": \"string\",\n      \"description\": \"The default locale code for the stack. All content must have a version in the master locale before it can be localized to other locales.\",\n      \"pattern\": \"^[a-z]{2}(-[A-Z]{2})?$\",\n      \"examples\": [\"en-us\", \"en-gb\", \"de-de\"]\n    },\n    \"org_uid\": {\n      \"type\": \"string\",\n      \"description\": \"UID of the organization that owns this stack.\"\n    },\n    \"plan_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the Contentstack subscription plan for this stack.\"\n    },\n    \"settings\": {\n      \"$ref\": \"#/$defs/StackSettings\"\n  \
  \  },\n    \"created_by\": {\n      \"type\": \"string\",\n      \"description\": \"UID of the user who created the stack.\"\n    },\n    \"updated_by\": {\n      \"type\": \"string\",\n      \"description\": \"UID of the user who last modified stack settings.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 UTC timestamp of when the stack was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 UTC timestamp of when the stack settings were last updated.\"\n    }\n  },\n  \"$defs\": {\n    \"StackSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration settings for the stack.\",\n      \"properties\": {\n        \"version\": {\n          \"type\": \"integer\",\n          \"description\": \"Version number of the stack settings configuration.\",\n          \"minimum\": 1\n        },\n        \"rte_version\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"Version of the rich text editor used in this stack.\",\n          \"enum\": [2, 3]\n        },\n        \"blockEditorExperience\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether the block editor experience is enabled for this stack.\"\n        },\n        \"locales\": {\n          \"type\": \"array\",\n          \"description\": \"List of locale codes enabled for this stack.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"pattern\": \"^[a-z]{2}(-[A-Z]{2})?$\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/json-schema/contentstack-stack-schema.json
tags: []
title: Contentstack Stack
---
