---
description: Represents a worker in Workday, including employees and contingent workers, with personal data, employment details, job information, and organizational assignments.
layout: schema
name: Workday Worker
properties_list:
- description: Workday ID of the worker
  name: id
  type: string
- description: Display name of the worker
  name: descriptor
  type: string
- description: Type of worker
  name: workerType
  type: string
- description: ''
  name: personalData
  type: object
- description: ''
  name: employmentData
  type: object
- description: ''
  name: contactData
  type: object
provider_name: Workday Integrations
provider_slug: workday-integrations
schema_file: json-schema/workday-integrations-worker-schema.json
slug: workday-integrations-worker
source_filename: workday-integrations-worker-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://community.workday.com/schemas/workday-integrations/worker.json\",\n  \"title\": \"Workday Worker\",\n  \"description\": \"Represents a worker in Workday, including employees and contingent workers, with personal data, employment details, job information, and organizational assignments.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"descriptor\", \"workerType\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Workday ID of the worker\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the worker\"\n    },\n    \"workerType\": {\n      \"type\": \"string\",\n      \"enum\": [\"Employee\", \"Contingent_Worker\"],\n      \"description\": \"Type of worker\"\n    },\n    \"personalData\": {\n      \"$ref\": \"#/$defs/PersonalData\"\n    },\n    \"employmentData\": {\n      \"$ref\": \"#/$defs/EmploymentData\"\
  \n    },\n    \"contactData\": {\n      \"$ref\": \"#/$defs/ContactData\"\n    }\n  },\n  \"$defs\": {\n    \"PersonalData\": {\n      \"type\": \"object\",\n      \"description\": \"Personal information about the worker\",\n      \"properties\": {\n        \"legalName\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"firstName\": {\n              \"type\": \"string\",\n              \"description\": \"Legal first name\"\n            },\n            \"lastName\": {\n              \"type\": \"string\",\n              \"description\": \"Legal last name\"\n            },\n            \"middleName\": {\n              \"type\": \"string\",\n              \"description\": \"Legal middle name\"\n            }\n          },\n          \"required\": [\"firstName\", \"lastName\"]\n        },\n        \"dateOfBirth\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date of birth\"\n        },\n        \"gender\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"Gender identity\"\n        },\n        \"nationality\": {\n          \"type\": \"string\",\n          \"description\": \"Nationality or citizenship\"\n        }\n      }\n    },\n    \"EmploymentData\": {\n      \"type\": \"object\",\n      \"description\": \"Employment details for the worker\",\n      \"properties\": {\n        \"hireDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Original hire date\"\n        },\n        \"terminationDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"Termination date if applicable\"\n        },\n        \"workerStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\"Active\", \"Terminated\", \"On_Leave\"],\n          \"description\": \"Current employment status\"\n        },\n        \"employeeType\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Employee type classification\"\n        },\n        \"jobData\": {\n          \"$ref\": \"#/$defs/JobData\"\n        }\n      }\n    },\n    \"JobData\": {\n      \"type\": \"object\",\n      \"description\": \"Current job assignment details\",\n      \"properties\": {\n        \"jobTitle\": {\n          \"type\": \"string\",\n          \"description\": \"Current job title\"\n        },\n        \"businessTitle\": {\n          \"type\": \"string\",\n          \"description\": \"Business title\"\n        },\n        \"jobProfile\": {\n          \"$ref\": \"#/$defs/Reference\"\n        },\n        \"position\": {\n          \"$ref\": \"#/$defs/Reference\"\n        },\n        \"location\": {\n          \"$ref\": \"#/$defs/Reference\"\n        },\n        \"supervisoryOrganization\": {\n          \"$ref\": \"#/$defs/Reference\"\n        },\n        \"managementLevel\": {\n          \"$ref\": \"#/$defs/Reference\"\n        }\n      }\n    },\n    \"ContactData\": {\n      \"type\": \"\
  object\",\n      \"description\": \"Contact information for the worker\",\n      \"properties\": {\n        \"primaryWorkEmail\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Primary work email\"\n        },\n        \"primaryWorkPhone\": {\n          \"type\": \"string\",\n          \"description\": \"Primary work phone number\"\n        },\n        \"businessAddress\": {\n          \"$ref\": \"#/$defs/Address\"\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"Physical address\",\n      \"properties\": {\n        \"line1\": {\n          \"type\": \"string\"\n        },\n        \"line2\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"state\": {\n          \"type\": \"string\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"\
  string\"\n        }\n      }\n    },\n    \"Reference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a Workday business object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Workday ID of the referenced object\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the referenced object\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"API URL for the referenced resource\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/json-schema/workday-integrations-worker-schema.json
tags:
- Cloud
- Enterprise Software
- ERP
- Finance
- HCM
- HR
- Integration
title: Workday Worker
---
