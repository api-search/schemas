---
description: Schema for an Amazon Connect instance resource, representing a cloud contact center instance with users, queues, and contact flows.
layout: schema
name: Amazon Connect Instance
properties_list:
- description: The identifier of the Amazon Connect instance.
  name: Id
  type: string
- description: The ARN of the Amazon Connect instance.
  name: Arn
  type: string
- description: The identity management type of the instance.
  name: IdentityManagementType
  type: string
- description: The alias of the instance.
  name: InstanceAlias
  type: string
- description: When the instance was created.
  name: CreatedTime
  type: string
- description: The service role of the instance.
  name: ServiceRole
  type: string
- description: The state of the instance.
  name: InstanceStatus
  type: string
- description: Whether inbound calls are enabled.
  name: InboundCallsEnabled
  type: boolean
- description: Whether outbound calls are enabled.
  name: OutboundCallsEnabled
  type: boolean
- description: ''
  name: User
  type: object
- description: ''
  name: Queue
  type: object
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/amazon-connect-instance-schema.json
slug: amazon-connect-instance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://example.com/schemas/amazon-connect-instance.json\",\n  \"title\": \"Amazon Connect Instance\",\n  \"description\": \"Schema for an Amazon Connect instance resource, representing a cloud contact center instance with users, queues, and contact flows.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the Amazon Connect instance.\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the Amazon Connect instance.\",\n      \"pattern\": \"^arn:aws:connect:[a-z0-9-]+:[0-9]{12}:instance/[a-f0-9-]+\"\n    },\n    \"IdentityManagementType\": {\n      \"type\": \"string\",\n      \"description\": \"The identity management type of the instance.\",\n      \"enum\": [\"SAML\", \"CONNECT_MANAGED\", \"EXISTING_DIRECTORY\"]\n    },\n    \"InstanceAlias\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The alias of the instance.\",\n      \"minLength\": 1,\n      \"maxLength\": 62,\n      \"pattern\": \"^[a-zA-Z0-9][a-zA-Z0-9-]+$\"\n    },\n    \"CreatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the instance was created.\"\n    },\n    \"ServiceRole\": {\n      \"type\": \"string\",\n      \"description\": \"The service role of the instance.\"\n    },\n    \"InstanceStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the instance.\",\n      \"enum\": [\"CREATION_IN_PROGRESS\", \"ACTIVE\", \"CREATION_FAILED\"]\n    },\n    \"InboundCallsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether inbound calls are enabled.\"\n    },\n    \"OutboundCallsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether outbound calls are enabled.\"\n    },\n    \"User\": {\n      \"$ref\": \"#/$defs/User\"\n    },\n    \"Queue\": {\n      \"$ref\"\
  : \"#/$defs/Queue\"\n    }\n  },\n  \"$defs\": {\n    \"User\": {\n      \"type\": \"object\",\n      \"description\": \"A user account in the Amazon Connect instance.\",\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the user account.\"\n        },\n        \"Arn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the user account.\"\n        },\n        \"Username\": {\n          \"type\": \"string\",\n          \"description\": \"The user name assigned to the user account.\",\n          \"minLength\": 1,\n          \"maxLength\": 100\n        },\n        \"IdentityInfo\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"FirstName\": {\n              \"type\": \"string\",\n              \"maxLength\": 100\n            },\n            \"LastName\": {\n              \"type\": \"string\",\n              \"maxLength\": 100\n            },\n            \"\
  Email\": {\n              \"type\": \"string\",\n              \"format\": \"email\"\n            }\n          }\n        },\n        \"PhoneConfig\": {\n          \"type\": \"object\",\n          \"required\": [\"PhoneType\"],\n          \"properties\": {\n            \"PhoneType\": {\n              \"type\": \"string\",\n              \"enum\": [\"SOFT_PHONE\", \"DESK_PHONE\"]\n            },\n            \"AutoAccept\": {\n              \"type\": \"boolean\"\n            },\n            \"AfterContactWorkTimeLimit\": {\n              \"type\": \"integer\",\n              \"minimum\": 0\n            },\n            \"DeskPhoneNumber\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"SecurityProfileIds\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"minItems\": 1,\n          \"maxItems\": 10\n        },\n        \"RoutingProfileId\": {\n          \"type\": \"string\",\n \
  \         \"description\": \"The identifier of the routing profile for the user.\"\n        }\n      }\n    },\n    \"Queue\": {\n      \"type\": \"object\",\n      \"description\": \"A queue in the Amazon Connect instance.\",\n      \"properties\": {\n        \"QueueId\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the queue.\"\n        },\n        \"QueueArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the queue.\"\n        },\n        \"Name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the queue.\",\n          \"maxLength\": 256\n        },\n        \"QueueType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of queue.\",\n          \"enum\": [\"STANDARD\", \"AGENT\"]\n        },\n        \"Description\": {\n          \"type\": \"string\",\n          \"description\": \"The description of the queue.\",\n          \"maxLength\": 250\n        },\n    \
  \    \"MaxContacts\": {\n          \"type\": \"integer\",\n          \"description\": \"The maximum number of contacts that can be in the queue.\",\n          \"minimum\": 0\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/amazon-connect-instance-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: Amazon Connect Instance
---
