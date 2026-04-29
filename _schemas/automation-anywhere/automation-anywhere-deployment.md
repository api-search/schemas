---
description: Schema representing a bot deployment request and response in the Automation Anywhere Control Room, including deployment configuration, target device specification, input variables, and the resulting deployment identifier.
layout: schema
name: Automation Anywhere Bot Deployment
properties_list:
- description: Unique UUID identifier assigned to this deployment instance by the Control Room upon successful dispatch
  name: deploymentId
  type: string
- description: Numeric file ID of the bot to deploy, referencing the bot's ID in the repository
  name: botId
  type: integer
- description: Optional human-readable label for this automation instance as displayed in activity logs and dashboards
  name: automationName
  type: string
- description: Optional description of this specific deployment for tracking and audit purposes
  name: description
  type: string
- description: Optional label tag for identifying this deployment instance
  name: botLabel
  type: string
- description: Whether to run the bot with elevated system privileges on the Bot Runner device
  name: runElevated
  type: boolean
- description: Whether to suppress the Bot Agent user interface on the runner device during execution
  name: hideBotAgentUi
  type: boolean
- description: Priority level for this automation in the dispatch queue relative to other pending deployments
  name: automationPriority
  type: string
- description: ''
  name: callbackInfo
  type: object
- description: Runtime input variables to pass to the bot at execution time. Keys are variable names as defined in the bot; values are typed variable objects.
  name: botInput
  type: object
- description: ''
  name: unattendedRequest
  type: object
- description: ''
  name: attendedRequest
  type: object
- description: ''
  name: headlessRequest
  type: object
provider_name: automation-anywhere
provider_slug: automation-anywhere
schema_file: json-schema/automation-anywhere-deployment-schema.json
slug: automation-anywhere-deployment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://automationanywhere.com/schemas/deployment.json\",\n  \"title\": \"Automation Anywhere Bot Deployment\",\n  \"description\": \"Schema representing a bot deployment request and response in the Automation Anywhere Control Room, including deployment configuration, target device specification, input variables, and the resulting deployment identifier.\",\n  \"type\": \"object\",\n  \"required\": [\"botId\"],\n  \"properties\": {\n    \"deploymentId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique UUID identifier assigned to this deployment instance by the Control Room upon successful dispatch\"\n    },\n    \"botId\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric file ID of the bot to deploy, referencing the bot's ID in the repository\",\n      \"minimum\": 1\n    },\n    \"automationName\": {\n      \"type\": \"string\",\n \
  \     \"description\": \"Optional human-readable label for this automation instance as displayed in activity logs and dashboards\",\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of this specific deployment for tracking and audit purposes\",\n      \"maxLength\": 1000\n    },\n    \"botLabel\": {\n      \"type\": \"string\",\n      \"description\": \"Optional label tag for identifying this deployment instance\",\n      \"maxLength\": 100\n    },\n    \"runElevated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to run the bot with elevated system privileges on the Bot Runner device\"\n    },\n    \"hideBotAgentUi\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to suppress the Bot Agent user interface on the runner device during execution\"\n    },\n    \"automationPriority\": {\n      \"type\": \"string\",\n      \"description\": \"Priority level for this automation\
  \ in the dispatch queue relative to other pending deployments\",\n      \"enum\": [\"PRIORITY_LOW\", \"PRIORITY_MEDIUM\", \"PRIORITY_HIGH\"]\n    },\n    \"callbackInfo\": {\n      \"$ref\": \"#/$defs/CallbackInfo\"\n    },\n    \"botInput\": {\n      \"type\": \"object\",\n      \"description\": \"Runtime input variables to pass to the bot at execution time. Keys are variable names as defined in the bot; values are typed variable objects.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/BotInputVariable\"\n      }\n    },\n    \"unattendedRequest\": {\n      \"$ref\": \"#/$defs/UnattendedRequest\"\n    },\n    \"attendedRequest\": {\n      \"$ref\": \"#/$defs/AttendedRequest\"\n    },\n    \"headlessRequest\": {\n      \"$ref\": \"#/$defs/HeadlessRequest\"\n    }\n  },\n  \"$defs\": {\n    \"CallbackInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Webhook callback configuration for receiving execution completion or failure notifications\",\n      \"required\"\
  : [\"url\"],\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"HTTPS endpoint URL to POST the execution result notification to upon completion or failure\"\n        },\n        \"headers\": {\n          \"type\": \"object\",\n          \"description\": \"Optional HTTP headers to include in the callback POST request (e.g., authorization headers)\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"BotInputVariable\": {\n      \"type\": \"object\",\n      \"description\": \"A typed input variable value passed to the bot at deployment time\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Data type of the variable matching its declaration in the bot definition\",\n          \"enum\": [\"STRING\", \"NUMBER\", \"BOOLEAN\", \"LIST\", \"DICTIONARY\"\
  , \"DATETIME\", \"CREDENTIAL\"]\n        },\n        \"string\": {\n          \"type\": \"string\",\n          \"description\": \"String value for variables of type STRING\"\n        },\n        \"number\": {\n          \"type\": \"string\",\n          \"description\": \"Numeric value represented as a string for NUMBER type variables\",\n          \"pattern\": \"^-?[0-9]+(\\\\.[0-9]+)?$\"\n        },\n        \"boolean\": {\n          \"type\": \"boolean\",\n          \"description\": \"Boolean value for BOOLEAN type variables\"\n        },\n        \"list\": {\n          \"type\": \"object\",\n          \"description\": \"Structured list value for LIST type variables\"\n        },\n        \"dictionary\": {\n          \"type\": \"object\",\n          \"description\": \"Key-value map for DICTIONARY type variables\",\n          \"additionalProperties\": true\n        }\n      }\n    },\n    \"UnattendedRequest\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for\
  \ unattended bot execution on Bot Runner devices associated with specified user accounts\",\n      \"properties\": {\n        \"runAsUsers\": {\n          \"type\": \"array\",\n          \"description\": \"User accounts whose associated Bot Runner devices will execute the bot\",\n          \"items\": {\n            \"$ref\": \"#/$defs/RunAsUser\"\n          },\n          \"minItems\": 1\n        },\n        \"poolIds\": {\n          \"type\": \"array\",\n          \"description\": \"Device pool IDs to dispatch the bot to; the Control Room selects an available device from each pool\",\n          \"items\": {\n            \"type\": \"integer\",\n            \"description\": \"Numeric ID of a device pool\"\n          }\n        }\n      }\n    },\n    \"AttendedRequest\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for attended bot execution on the device of a currently logged-in user\",\n      \"properties\": {\n        \"currentUserDeviceId\": {\n          \"\
  type\": \"integer\",\n          \"description\": \"Device ID of the machine where the attended user is currently logged in\"\n        }\n      }\n    },\n    \"HeadlessRequest\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for headless bot execution on On-Demand cloud Bot Runner devices\",\n      \"properties\": {\n        \"numOfRunAsUsersToUse\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of On-Demand Bot Runner instances to allocate for parallel headless execution\",\n          \"minimum\": 1\n        }\n      }\n    },\n    \"RunAsUser\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a user account whose associated Bot Runner device will execute an unattended bot\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Numeric user ID of the run-as user in the Control Room\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/automation-anywhere/refs/heads/main/json-schema/automation-anywhere-deployment-schema.json
tags: []
title: Automation Anywhere Bot Deployment
---
