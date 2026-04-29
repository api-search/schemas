---
description: Schema for a CVP VXML application. Applications are VoiceXML programs typically built with Cisco Unified Call Studio that execute on the CVP VXML Server to provide interactive voice response (IVR) functionality. Applications consist of call flow elements including voice elements, action elements, and decision elements.
layout: schema
name: Cisco Voice Portal Application
properties_list:
- description: Unique identifier for the application
  name: applicationId
  type: string
- description: Name of the application as deployed
  name: applicationName
  type: string
- description: Type of VXML application. Call Studio applications are built with Cisco Unified Call Studio. Standalone VXML applications are hand-coded VoiceXML. Micro-applications are built-in CVP IVR functions.
  name: applicationType
  type: string
- description: Current deployment and operational status
  name: status
  type: string
- description: Application version
  name: version
  type: string
- description: Description of the application purpose
  name: description
  type: string
- description: Name of the starting call flow element
  name: entryPoint
  type: string
- description: Call flow elements that make up the application
  name: elements
  type: array
- description: Application-level runtime configuration parameters
  name: configParameters
  type: object
- description: Default language for prompts and ASR
  name: defaultLanguage
  type: string
- description: Allowed caller input modes
  name: inputModes
  type: array
- description: VXML Servers this application is deployed to
  name: deployedServers
  type: array
- description: Path to associated audio prompt files
  name: mediaDirectory
  type: string
- description: Path to associated speech grammar files
  name: grammarDirectory
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-application.json
slug: cisco-voice-portal-application
source_filename: cisco-voice-portal-application.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/cisco-voice-portal/json-schema/cisco-voice-portal-application.json\",\n  \"title\": \"Cisco Voice Portal Application\",\n  \"description\": \"Schema for a CVP VXML application. Applications are VoiceXML programs typically built with Cisco Unified Call Studio that execute on the CVP VXML Server to provide interactive voice response (IVR) functionality. Applications consist of call flow elements including voice elements, action elements, and decision elements.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the application\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the application as deployed\"\n    },\n    \"applicationType\": {\n      \"type\": \"string\",\n      \"enum\": [\"callstudio\", \"standalone_vxml\"\
  , \"microapp\"],\n      \"description\": \"Type of VXML application. Call Studio applications are built with Cisco Unified Call Studio. Standalone VXML applications are hand-coded VoiceXML. Micro-applications are built-in CVP IVR functions.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"deployed\", \"undeployed\", \"deploying\", \"error\", \"active\", \"inactive\"],\n      \"description\": \"Current deployment and operational status\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Application version\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the application purpose\"\n    },\n    \"entryPoint\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the starting call flow element\"\n    },\n    \"elements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CallFlowElement\"\n      },\n      \"description\": \"Call flow\
  \ elements that make up the application\"\n    },\n    \"configParameters\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Application-level runtime configuration parameters\"\n    },\n    \"defaultLanguage\": {\n      \"type\": \"string\",\n      \"default\": \"en-US\",\n      \"description\": \"Default language for prompts and ASR\"\n    },\n    \"inputModes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"dtmf\", \"voice\"]\n      },\n      \"description\": \"Allowed caller input modes\"\n    },\n    \"deployedServers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ServerDeployment\"\n      },\n      \"description\": \"VXML Servers this application is deployed to\"\n    },\n    \"mediaDirectory\": {\n      \"type\": \"string\",\n      \"description\": \"Path to associated audio prompt files\"\n    },\n    \"\
  grammarDirectory\": {\n      \"type\": \"string\",\n      \"description\": \"Path to associated speech grammar files\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"applicationName\", \"applicationType\"],\n  \"$defs\": {\n    \"CallFlowElement\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"elementName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the call flow element\"\n        },\n        \"elementType\": {\n          \"type\": \"string\",\n          \"enum\": [\"voice\", \"action\", \"decision\", \"subdialog\"],\n          \"description\": \"Type of element. Voice elements interact with the caller (e.g., play prompt, collect digits). Action elements perform backend operations (e.g., database lookup, web service call). Decision elements control flow logic. Subdialog\
  \ elements invoke sub-applications.\"\n        },\n        \"className\": {\n          \"type\": \"string\",\n          \"description\": \"Fully qualified Java class name implementing the element\"\n        },\n        \"configParameters\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Element-specific configuration\"\n        },\n        \"exits\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Exit name (e.g., done, error, timeout, nomatch)\"\n              },\n              \"targetElement\": {\n                \"type\": \"string\",\n                \"description\": \"Name of the target element for this exit\"\n              }\n            },\n            \"required\": [\"name\"]\n          },\n       \
  \   \"description\": \"Available exit paths from this element\"\n        }\n      },\n      \"required\": [\"elementName\", \"elementType\"]\n    },\n    \"ServerDeployment\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"serverId\": {\n          \"type\": \"string\"\n        },\n        \"serverHostname\": {\n          \"type\": \"string\"\n        },\n        \"deploymentStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\"deployed\", \"pending\", \"error\"]\n        },\n        \"deployedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      },\n      \"required\": [\"serverId\", \"deploymentStatus\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-application.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: Cisco Voice Portal Application
---
