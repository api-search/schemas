---
description: Represents a worker in Workday, including employees and contingent workers. A worker has personal information, job data, compensation, and organizational relationships.
layout: schema
name: Worker
properties_list:
- description: The Workday ID of the worker.
  name: id
  type: string
- description: A display descriptor for the worker, typically the full name.
  name: descriptor
  type: string
- description: The employee ID or contingent worker ID.
  name: workerID
  type: string
- description: The type of worker (e.g., Employee, Contingent Worker).
  name: workerType
  type: object
- description: Personal information for the worker.
  name: personalInformation
  type: object
- description: Contact information for the worker.
  name: contactInformation
  type: object
- description: Primary job data for the worker.
  name: jobData
  type: object
- description: Organizational assignment data.
  name: organizationData
  type: object
- description: Management chain data.
  name: managementData
  type: object
- description: The original hire date.
  name: hireDate
  type: string
- description: The original hire date across all employments.
  name: originalHireDate
  type: string
- description: The termination date, if applicable.
  name: terminationDate
  type:
  - string
  - 'null'
- description: Whether the worker is currently active.
  name: isActive
  type: boolean
- description: An external system identifier for the worker.
  name: externalID
  type: string
- description: A link to the full worker resource.
  name: href
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/worker.json
slug: worker
source_filename: worker.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://workday.com/schemas/worker.json\",\n  \"title\": \"Worker\",\n  \"description\": \"Represents a worker in Workday, including employees and contingent workers. A worker has personal information, job data, compensation, and organizational relationships.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the worker.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"A display descriptor for the worker, typically the full name.\"\n    },\n    \"workerID\": {\n      \"type\": \"string\",\n      \"description\": \"The employee ID or contingent worker ID.\"\n    },\n    \"workerType\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The type of worker (e.g., Employee, Contingent Worker).\"\n    },\n    \"personalInformation\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"Personal information for the worker.\",\n      \"properties\": {\n        \"legalName\": {\n          \"$ref\": \"#/$defs/PersonName\",\n          \"description\": \"The legal name of the worker.\"\n        },\n        \"preferredName\": {\n          \"$ref\": \"#/$defs/PersonName\",\n          \"description\": \"The preferred name of the worker.\"\n        },\n        \"dateOfBirth\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The date of birth.\"\n        },\n        \"gender\": {\n          \"$ref\": \"#/$defs/ResourceReference\"\n        },\n        \"nationality\": {\n          \"$ref\": \"#/$defs/ResourceReference\"\n        },\n        \"maritalStatus\": {\n          \"$ref\": \"#/$defs/ResourceReference\"\n        }\n      }\n    },\n    \"contactInformation\": {\n      \"type\": \"object\",\n      \"description\": \"Contact information for the worker.\",\n      \"properties\": {\n  \
  \      \"primaryWorkEmail\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The primary work email address.\"\n        },\n        \"primaryWorkPhone\": {\n          \"type\": \"string\",\n          \"description\": \"The primary work phone number.\"\n        },\n        \"workAddress\": {\n          \"$ref\": \"#/$defs/Address\",\n          \"description\": \"The primary work address.\"\n        },\n        \"homeAddress\": {\n          \"$ref\": \"#/$defs/Address\",\n          \"description\": \"The primary home address.\"\n        }\n      }\n    },\n    \"jobData\": {\n      \"type\": \"object\",\n      \"description\": \"Primary job data for the worker.\",\n      \"properties\": {\n        \"businessTitle\": {\n          \"type\": \"string\",\n          \"description\": \"The business title for the worker.\"\n        },\n        \"jobProfile\": {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The\
  \ job profile assigned to the worker.\"\n        },\n        \"position\": {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The position the worker holds.\"\n        },\n        \"location\": {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The work location.\"\n        },\n        \"timeType\": {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The time type (e.g., Full Time, Part Time).\"\n        },\n        \"workerSubType\": {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The worker sub-type (e.g., Regular, Temporary).\"\n        },\n        \"isPrimaryJob\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is the primary job.\"\n        }\n      }\n    },\n    \"organizationData\": {\n      \"type\": \"object\",\n      \"description\": \"Organizational assignment data.\",\n      \"properties\": {\n        \"primarySupervisoryOrganization\"\
  : {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The primary supervisory organization.\"\n        },\n        \"costCenter\": {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The cost center assignment.\"\n        },\n        \"company\": {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The company the worker belongs to.\"\n        },\n        \"region\": {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The region assignment.\"\n        }\n      }\n    },\n    \"managementData\": {\n      \"type\": \"object\",\n      \"description\": \"Management chain data.\",\n      \"properties\": {\n        \"isManager\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the worker is a manager.\"\n        },\n        \"manager\": {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The worker's direct manager.\"\
  \n        },\n        \"managementLevel\": {\n          \"$ref\": \"#/$defs/ResourceReference\",\n          \"description\": \"The management level.\"\n        }\n      }\n    },\n    \"hireDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The original hire date.\"\n    },\n    \"originalHireDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The original hire date across all employments.\"\n    },\n    \"terminationDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"The termination date, if applicable.\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the worker is currently active.\"\n    },\n    \"externalID\": {\n      \"type\": \"string\",\n      \"description\": \"An external system identifier for the worker.\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n    \
  \  \"description\": \"A link to the full worker resource.\"\n    }\n  },\n  \"required\": [\"id\", \"descriptor\"],\n  \"$defs\": {\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a Workday resource.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The Workday ID of the referenced resource.\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\",\n          \"description\": \"A display descriptor for the referenced resource.\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"A link to the referenced resource.\"\n        }\n      }\n    },\n    \"PersonName\": {\n      \"type\": \"object\",\n      \"description\": \"A person's name components.\",\n      \"properties\": {\n        \"firstName\": {\n          \"type\": \"string\",\n          \"description\": \"The first name.\"\n   \
  \     },\n        \"middleName\": {\n          \"type\": \"string\",\n          \"description\": \"The middle name.\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"description\": \"The last name.\"\n        },\n        \"fullName\": {\n          \"type\": \"string\",\n          \"description\": \"The full formatted name.\"\n        },\n        \"prefix\": {\n          \"type\": \"string\",\n          \"description\": \"The name prefix (e.g., Mr., Dr.).\"\n        },\n        \"suffix\": {\n          \"type\": \"string\",\n          \"description\": \"The name suffix (e.g., Jr., III).\"\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"A physical address.\",\n      \"properties\": {\n        \"addressLine1\": {\n          \"type\": \"string\"\n        },\n        \"addressLine2\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n      \
  \  \"stateProvince\": {\n          \"$ref\": \"#/$defs/ResourceReference\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"$ref\": \"#/$defs/ResourceReference\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/worker.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Worker
---
