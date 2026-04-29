---
description: Schema for the .all-contributorsrc configuration file used by the All Contributors specification and bot to manage open-source project contributor attribution.
layout: schema
name: AllContributorsConfig
properties_list:
- description: Name of the project repository.
  name: projectName
  type: string
- description: GitHub username or organization that owns the project.
  name: projectOwner
  type: string
- description: Type of repository hosting service.
  name: repoType
  type: string
- description: Hostname of the repository hosting service.
  name: repoHost
  type: string
- description: List of files to update with contributor tables.
  name: files
  type: array
- description: Size in pixels for contributor avatar images.
  name: imageSize
  type: integer
- description: Whether to automatically commit changes when contributors are added.
  name: commit
  type: boolean
- description: Commit message convention to follow.
  name: commitConvention
  type: string
- description: Maximum number of contributors to display per line in the table.
  name: contributorsPerLine
  type: integer
- description: Custom template for the contributors badge markdown.
  name: badgeTemplate
  type: string
- description: Custom template for individual contributor entries in the table.
  name: contributorTemplate
  type: string
- description: Custom contribution type definitions extending the default types.
  name: types
  type: object
- description: List of contributors to the project.
  name: contributors
  type: array
provider_name: AUTHORS.md
provider_slug: authors-md
schema_file: json-schema/all-contributors-config-schema.json
slug: all-contributors-config
source_filename: all-contributors-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/authors-md/refs/heads/main/json-schema/all-contributors-config-schema.json\",\n  \"title\": \"AllContributorsConfig\",\n  \"description\": \"Schema for the .all-contributorsrc configuration file used by the All Contributors specification and bot to manage open-source project contributor attribution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the project repository.\",\n      \"example\": \"all-contributors\"\n    },\n    \"projectOwner\": {\n      \"type\": \"string\",\n      \"description\": \"GitHub username or organization that owns the project.\",\n      \"example\": \"all-contributors\"\n    },\n    \"repoType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of repository hosting service.\",\n      \"enum\": [\"github\", \"gitlab\",\
  \ \"bitbucket\"],\n      \"example\": \"github\"\n    },\n    \"repoHost\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the repository hosting service.\",\n      \"example\": \"https://github.com\"\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"description\": \"List of files to update with contributor tables.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\"README.md\"]\n    },\n    \"imageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Size in pixels for contributor avatar images.\",\n      \"example\": 100\n    },\n    \"commit\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to automatically commit changes when contributors are added.\",\n      \"example\": false\n    },\n    \"commitConvention\": {\n      \"type\": \"string\",\n      \"description\": \"Commit message convention to follow.\",\n      \"enum\": [\"none\", \"angular\", \"atom\", \"ember\", \"eslint\", \"\
  jshint\", \"gitmoji\"],\n      \"example\": \"none\"\n    },\n    \"contributorsPerLine\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of contributors to display per line in the table.\",\n      \"example\": 7\n    },\n    \"badgeTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"Custom template for the contributors badge markdown.\",\n      \"example\": \"[![All Contributors](https://img.shields.io/badge/all_contributors-<%= contributors.length %>-orange.svg?style=flat-square)](#contributors-)\"\n    },\n    \"contributorTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"Custom template for individual contributor entries in the table.\",\n      \"example\": \"<a href=\\\"<%= contributor.profile %>\\\"><img src=\\\"<%= contributor.avatar_url %>\\\" width=\\\"<%= options.imageSize %>px;\\\" alt=\\\"\\\"/><br /><sub><b><%= contributor.name %></b></sub></a>\"\n    },\n    \"types\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Custom contribution type definitions extending the default types.\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"symbol\": {\n            \"type\": \"string\",\n            \"description\": \"Emoji symbol for this contribution type.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"Human-readable description of this contribution type.\"\n          },\n          \"link\": {\n            \"type\": \"string\",\n            \"description\": \"URL template for linking this contribution type.\"\n          }\n        }\n      }\n    },\n    \"contributors\": {\n      \"type\": \"array\",\n      \"description\": \"List of contributors to the project.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Contributor\"\n      }\n    }\n  },\n  \"required\": [\"projectName\", \"projectOwner\", \"contributors\"],\n  \"$defs\": {\n    \"Contributor\": {\n      \"type\": \"\
  object\",\n      \"title\": \"Contributor\",\n      \"description\": \"An individual contributor to the project with their profile information and contribution types.\",\n      \"properties\": {\n        \"login\": {\n          \"type\": \"string\",\n          \"description\": \"GitHub/GitLab username of the contributor.\",\n          \"example\": \"jsmith\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Full display name of the contributor.\",\n          \"example\": \"Jane Smith\"\n        },\n        \"avatar_url\": {\n          \"type\": \"string\",\n          \"description\": \"URL to the contributor's avatar image.\",\n          \"format\": \"uri\",\n          \"example\": \"https://avatars.githubusercontent.com/u/12345?v=4\"\n        },\n        \"profile\": {\n          \"type\": \"string\",\n          \"description\": \"URL to the contributor's public profile page.\",\n          \"format\": \"uri\",\n          \"example\": \"https://github.com/jsmith\"\
  \n        },\n        \"contributions\": {\n          \"type\": \"array\",\n          \"description\": \"List of contribution types made by this contributor.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"audio\",\n              \"a11y\",\n              \"bug\",\n              \"blog\",\n              \"business\",\n              \"code\",\n              \"content\",\n              \"data\",\n              \"doc\",\n              \"design\",\n              \"example\",\n              \"eventOrganizing\",\n              \"financial\",\n              \"fundingFinding\",\n              \"ideas\",\n              \"infra\",\n              \"maintenance\",\n              \"mentoring\",\n              \"platform\",\n              \"plugin\",\n              \"projectManagement\",\n              \"promotion\",\n              \"question\",\n              \"research\",\n              \"review\",\n              \"security\",\n              \"\
  talk\",\n              \"test\",\n              \"tool\",\n              \"translation\",\n              \"tutorial\",\n              \"userTesting\",\n              \"video\"\n            ]\n          },\n          \"example\": [\"code\", \"doc\", \"review\"]\n        }\n      },\n      \"required\": [\"login\", \"name\", \"contributions\"]\n    },\n    \"AuthorEntry\": {\n      \"type\": \"object\",\n      \"title\": \"AuthorEntry\",\n      \"description\": \"A structured entry representing an author or contributor in an AUTHORS.md file.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Full name of the author.\",\n          \"example\": \"Jane Smith\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"description\": \"Email address of the author.\",\n          \"format\": \"email\",\n          \"example\": \"jsmith@example.com\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"Personal website or profile URL of the author.\",\n          \"format\": \"uri\",\n          \"example\": \"https://jsmith.example.com\"\n        },\n        \"contributions\": {\n          \"type\": \"string\",\n          \"description\": \"Description of which files or portions of the project the author contributed.\",\n          \"example\": \"Initial implementation of the core parser module and authentication system.\"\n        },\n        \"organization\": {\n          \"type\": \"string\",\n          \"description\": \"Organization or employer affiliation of the author.\",\n          \"example\": \"Example Corp\"\n        },\n        \"role\": {\n          \"type\": \"string\",\n          \"description\": \"Role of the author in the project.\",\n          \"enum\": [\"author\", \"contributor\", \"maintainer\", \"emeritus\"],\n          \"example\": \"author\"\n        }\n      },\n      \"required\": [\"name\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/authors-md/refs/heads/main/json-schema/all-contributors-config-schema.json
tags:
- Attribution
- Documentation
- Open Source
- Repository
- File Format
- Contributor Management
- License Compliance
- Standard
title: AllContributorsConfig
---
