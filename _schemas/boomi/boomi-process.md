---
description: Represents a Boomi integration process — an automated workflow that moves and transforms data between connected applications. Processes consist of a start shape (trigger), action shapes (steps), and optional decision logic.
layout: schema
name: Boomi Integration Process
properties_list:
- description: Unique component ID of the integration process (UUID format).
  name: id
  type: string
- description: Display name of the integration process.
  name: name
  type: string
- description: Component type. Always 'process' for integration processes.
  name: type
  type: string
- description: ID of the folder containing this process within the component library.
  name: folderId
  type: string
- description: Whether this process has been deleted from the component library.
  name: deleted
  type: boolean
- description: Version identifier of the current saved version of this process.
  name: currentVersion
  type: string
- description: ISO 8601 timestamp when the process was created.
  name: createdDate
  type: string
- description: ISO 8601 timestamp when the process was last modified.
  name: modifiedDate
  type: string
- description: Scheduling configurations for running this process on a time-based trigger.
  name: schedules
  type: array
- description: Active deployments of this process across environments.
  name: deployments
  type: array
provider_name: Boomi
provider_slug: boomi
schema_file: json-schema/boomi-process-schema.json
slug: boomi-process
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.boomi.com/schemas/process.json\",\n  \"title\": \"Boomi Integration Process\",\n  \"description\": \"Represents a Boomi integration process — an automated workflow that moves and transforms data between connected applications. Processes consist of a start shape (trigger), action shapes (steps), and optional decision logic.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique component ID of the integration process (UUID format).\",\n      \"pattern\": \"^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the integration process.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Component\
  \ type. Always 'process' for integration processes.\",\n      \"const\": \"process\"\n    },\n    \"folderId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the folder containing this process within the component library.\"\n    },\n    \"deleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this process has been deleted from the component library.\"\n    },\n    \"currentVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version identifier of the current saved version of this process.\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the process was created.\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the process was last modified.\"\n    },\n    \"schedules\": {\n      \"type\": \"array\",\n      \"description\": \"Scheduling configurations\
  \ for running this process on a time-based trigger.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ProcessSchedule\"\n      }\n    },\n    \"deployments\": {\n      \"type\": \"array\",\n      \"description\": \"Active deployments of this process across environments.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DeployedPackage\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"ProcessSchedule\": {\n      \"type\": \"object\",\n      \"title\": \"Process Schedule\",\n      \"description\": \"A time-based schedule that triggers a Boomi integration process to run automatically.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the schedule.\"\n        },\n        \"atomId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the Atom on which the scheduled process runs.\"\n        },\n        \"processId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the\
  \ process this schedule belongs to.\"\n        },\n        \"schedule\": {\n          \"type\": \"object\",\n          \"description\": \"Cron-based scheduling parameters.\",\n          \"properties\": {\n            \"minutes\": {\n              \"type\": \"string\",\n              \"description\": \"Minute field of the cron expression.\"\n            },\n            \"hours\": {\n              \"type\": \"string\",\n              \"description\": \"Hour field of the cron expression.\"\n            },\n            \"daysOfWeek\": {\n              \"type\": \"string\",\n              \"description\": \"Days-of-week field of the cron expression.\"\n            },\n            \"daysOfMonth\": {\n              \"type\": \"string\",\n              \"description\": \"Days-of-month field of the cron expression.\"\n            },\n            \"months\": {\n              \"type\": \"string\",\n              \"description\": \"Month field of the cron expression.\"\n            },\n          \
  \  \"years\": {\n              \"type\": \"string\",\n              \"description\": \"Year field of the cron expression.\"\n            }\n          }\n        }\n      }\n    },\n    \"ExecutionRecord\": {\n      \"type\": \"object\",\n      \"title\": \"Execution Record\",\n      \"description\": \"A record of a single integration process execution (job run).\",\n      \"required\": [\"executionId\", \"status\"],\n      \"properties\": {\n        \"executionId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of this execution instance.\"\n        },\n        \"processId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the process that was executed.\"\n        },\n        \"atomId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the Atom that ran the process.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Final status of the execution.\",\n     \
  \     \"enum\": [\"COMPLETE\", \"ERROR\", \"INPROCESS\", \"ABORTED\", \"DISCARDED\"]\n        },\n        \"executionTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the execution started.\"\n        },\n        \"duration\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Execution duration in milliseconds.\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Status message or error details for this execution.\"\n        },\n        \"inboundDocumentCount\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of documents processed in this execution.\"\n        },\n        \"outboundDocumentCount\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of output documents produced.\"\n        },\n        \"errorDocumentCount\"\
  : {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of documents that resulted in errors.\"\n        }\n      }\n    },\n    \"Environment\": {\n      \"type\": \"object\",\n      \"title\": \"Environment\",\n      \"description\": \"A Boomi runtime environment where Atoms are assigned and processes are deployed.\",\n      \"required\": [\"id\", \"name\", \"classification\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the environment.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the environment.\",\n          \"minLength\": 1\n        },\n        \"classification\": {\n          \"type\": \"string\",\n          \"description\": \"Whether this environment is production or test.\",\n          \"enum\": [\"PRODUCTION\", \"TEST\"]\n        },\n        \"createdDate\": {\n          \"type\"\
  : \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the environment was created.\"\n        }\n      }\n    },\n    \"Atom\": {\n      \"type\": \"object\",\n      \"title\": \"Atom\",\n      \"description\": \"A Boomi Atom — the lightweight runtime engine that executes integration processes.\",\n      \"required\": [\"id\", \"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the Atom.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the Atom.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current connectivity status of the Atom.\",\n          \"enum\": [\"ONLINE\", \"OFFLINE\", \"UNKNOWN\"]\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Atom deployment type.\",\n          \"enum\":\
  \ [\"ATOM\", \"MOLECULE\", \"CLOUD\"]\n        },\n        \"hostName\": {\n          \"type\": \"string\",\n          \"description\": \"Hostname of the machine running the Atom.\"\n        },\n        \"currentVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Current Boomi runtime version installed on this Atom.\"\n        },\n        \"dateInstalled\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the Atom was installed.\"\n        },\n        \"purgeHistoryDays\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of days to retain execution history before automatic purge.\"\n        }\n      }\n    },\n    \"DeployedPackage\": {\n      \"type\": \"object\",\n      \"title\": \"Deployed Package\",\n      \"description\": \"A packaged Boomi component deployed to a specific runtime environment.\",\n      \"required\": [\"deploymentId\"\
  , \"environmentId\", \"packageId\"],\n      \"properties\": {\n        \"deploymentId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of this deployment record.\"\n        },\n        \"environmentId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the environment this package is deployed to.\"\n        },\n        \"packageId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the packaged component that was deployed.\"\n        },\n        \"componentId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the underlying component.\"\n        },\n        \"componentType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of the deployed component (process, connector, etc.).\"\n        },\n        \"packageVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Version label of the deployed package.\"\n        },\n        \"deployedDate\": {\n\
  \          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when this package was deployed.\"\n        },\n        \"active\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this deployment is currently active.\"\n        },\n        \"notes\": {\n          \"type\": \"string\",\n          \"description\": \"Optional deployment notes.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/json-schema/boomi-process-schema.json
tags:
- AI Agents
- Automation
- B2B
- Data Integration
- EDI
- Integrations
- Management
- MFT
- Platform
- Workflows
title: Boomi Integration Process
---
