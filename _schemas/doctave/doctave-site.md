---
description: A documentation site managed on the Doctave docs-as-code platform, representing a collection of pages, configuration, and deployment settings.
layout: schema
name: Doctave Site
properties_list:
- description: Unique identifier for the documentation site.
  name: id
  type: string
- description: Display name of the documentation site.
  name: name
  type: string
- description: URL-friendly slug for the site.
  name: slug
  type: string
- description: A brief description of the documentation site.
  name: description
  type: string
- description: Custom domain configured for the site.
  name: customDomain
  type: string
- description: Source repository URL for the documentation content.
  name: repository
  type: string
- description: Git branch used for building the site.
  name: branch
  type: string
- description: Whether the site is publicly accessible or private.
  name: visibility
  type: string
- description: Ordered list of navigation items defining the site structure.
  name: navigation
  type: array
- description: Theme and branding configuration for the site.
  name: theme
  type: object
- description: Timestamp when the site was created.
  name: createdAt
  type: string
- description: Timestamp when the site was last updated.
  name: updatedAt
  type: string
provider_name: Doctave
provider_slug: doctave
schema_file: json-schema/doctave-site-schema.json
slug: doctave-site
source_filename: doctave-site-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/doctave/refs/heads/main/json-schema/doctave-site-schema.json\",\n  \"title\": \"Doctave Site\",\n  \"description\": \"A documentation site managed on the Doctave docs-as-code platform, representing a collection of pages, configuration, and deployment settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the documentation site.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the documentation site.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly slug for the site.\",\n      \"pattern\": \"^[a-z0-9]+(?:-[a-z0-9]+)*$\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A brief description of the documentation site.\"\n   \
  \ },\n    \"customDomain\": {\n      \"type\": \"string\",\n      \"format\": \"hostname\",\n      \"description\": \"Custom domain configured for the site.\"\n    },\n    \"repository\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Source repository URL for the documentation content.\"\n    },\n    \"branch\": {\n      \"type\": \"string\",\n      \"description\": \"Git branch used for building the site.\",\n      \"default\": \"main\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\"public\", \"private\"],\n      \"description\": \"Whether the site is publicly accessible or private.\"\n    },\n    \"navigation\": {\n      \"type\": \"array\",\n      \"description\": \"Ordered list of navigation items defining the site structure.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/NavigationItem\"\n      }\n    },\n    \"theme\": {\n      \"type\": \"object\",\n      \"description\": \"Theme and branding configuration\
  \ for the site.\",\n      \"properties\": {\n        \"primaryColor\": {\n          \"type\": \"string\",\n          \"description\": \"Primary brand color in hex format.\",\n          \"pattern\": \"^#[0-9a-fA-F]{6}$\"\n        },\n        \"logo\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the site logo image.\"\n        },\n        \"favicon\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the site favicon.\"\n        }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the site was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the site was last updated.\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"slug\"],\n  \"$defs\": {\n    \"NavigationItem\": {\n      \"type\": \"\
  object\",\n      \"description\": \"A navigation entry representing a page or section in the site hierarchy.\",\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"Display title of the navigation item.\"\n        },\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"URL path for the navigation item.\"\n        },\n        \"children\": {\n          \"type\": \"array\",\n          \"description\": \"Nested navigation items for sub-sections.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/NavigationItem\"\n          }\n        }\n      },\n      \"required\": [\"title\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/doctave/refs/heads/main/json-schema/doctave-site-schema.json
tags:
- Documentation
- OpenAPI
- Platform
- Portals
title: Doctave Site
---
