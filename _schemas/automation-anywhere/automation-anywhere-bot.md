---
description: Schema representing a bot (automation file) stored in the Automation Anywhere Control Room repository, including its metadata, versioning, workspace context, and repository permissions.
layout: schema
name: Automation Anywhere Bot
properties_list:
- description: Unique numeric identifier of the bot file in the Control Room repository
  name: id
  type: integer
- description: Numeric ID of the parent folder containing this bot in the repository hierarchy
  name: parentId
  type: integer
- description: Display name of the bot file as shown in the Control Room repository browser
  name: name
  type: string
- description: Full repository path from the workspace root (e.g., /Automation/Finance/Invoice Processing)
  name: path
  type: string
- description: Type of the repository object
  name: type
  type: string
- description: File size in bytes
  name: size
  type: integer
- description: Current version number of the bot file
  name: version
  type: integer
- description: Whether this version is labeled as the production version
  name: isProductionVersion
  type: boolean
- description: Workspace this bot belongs to
  name: workspaceType
  type: string
- description: Optional human-readable description of the bot's purpose
  name: description
  type: string
- description: ''
  name: permission
  type: object
- description: List of other bot files this bot depends on during execution
  name: dependencies
  type: array
- description: Optional tags applied to the bot for organization and search
  name: tags
  type: array
- description: Username of the Control Room user who created this bot
  name: createdBy
  type: string
- description: ISO 8601 timestamp when the bot was first created in the repository
  name: createdOn
  type: string
- description: Username of the Control Room user who last modified this bot
  name: updatedBy
  type: string
- description: ISO 8601 timestamp when the bot was last modified
  name: updatedOn
  type: string
provider_name: automation-anywhere
provider_slug: automation-anywhere
schema_file: json-schema/automation-anywhere-bot-schema.json
slug: automation-anywhere-bot
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://automationanywhere.com/schemas/bot.json\",\n  \"title\": \"Automation Anywhere Bot\",\n  \"description\": \"Schema representing a bot (automation file) stored in the Automation Anywhere Control Room repository, including its metadata, versioning, workspace context, and repository permissions.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"path\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier of the bot file in the Control Room repository\"\n    },\n    \"parentId\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric ID of the parent folder containing this bot in the repository hierarchy\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the bot file as shown in the Control Room repository browser\",\n      \"minLength\": 1,\n\
  \      \"maxLength\": 255\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Full repository path from the workspace root (e.g., /Automation/Finance/Invoice Processing)\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the repository object\",\n      \"enum\": [\"BOT\", \"FILE\", \"FOLDER\", \"TASK_BOT\", \"META_BOT\", \"IQ_BOT\", \"API_TASK\"]\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"File size in bytes\",\n      \"minimum\": 0\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Current version number of the bot file\",\n      \"minimum\": 1\n    },\n    \"isProductionVersion\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this version is labeled as the production version\"\n    },\n    \"workspaceType\": {\n      \"type\": \"string\",\n      \"description\": \"Workspace this bot belongs to\",\n      \"enum\": [\"PUBLIC\", \"\
  PRIVATE\"]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional human-readable description of the bot's purpose\",\n      \"maxLength\": 1000\n    },\n    \"permission\": {\n      \"$ref\": \"#/$defs/ObjectPermission\"\n    },\n    \"dependencies\": {\n      \"type\": \"array\",\n      \"description\": \"List of other bot files this bot depends on during execution\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DependencyRef\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Optional tags applied to the bot for organization and search\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the Control Room user who created this bot\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the bot was first created\
  \ in the repository\"\n    },\n    \"updatedBy\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the Control Room user who last modified this bot\"\n    },\n    \"updatedOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the bot was last modified\"\n    }\n  },\n  \"$defs\": {\n    \"ObjectPermission\": {\n      \"type\": \"object\",\n      \"description\": \"Actions the current authenticated user can perform on this repository object\",\n      \"properties\": {\n        \"delete\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the user can delete this bot from the repository\"\n        },\n        \"download\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the user can download this bot file\"\n        },\n        \"upload\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the user can upload a new version of this\
  \ bot\"\n        },\n        \"run\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the user can deploy and run this bot\"\n        },\n        \"view\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the user can view this bot in the repository\"\n        },\n        \"clone\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the user can clone (copy) this bot to another location\"\n        }\n      }\n    },\n    \"DependencyRef\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a file that this bot depends on\",\n      \"required\": [\"id\", \"name\", \"path\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Numeric ID of the dependency file\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the dependency file\"\n        },\n        \"path\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Repository path of the dependency file\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of the dependency object\",\n          \"enum\": [\"BOT\", \"FILE\", \"FOLDER\"]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/json-schema/automation-anywhere-bot-schema.json
tags: []
title: Automation Anywhere Bot
---
