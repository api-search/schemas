---
description: A Contact business component record in Oracle Siebel CRM representing an individual person associated with an account. Contacts store personal and professional information including name, job title, communication details, and organizational affiliations.
layout: schema
name: Oracle Siebel CRM Contact
properties_list:
- description: Unique system-generated row identifier for the contact record
  name: Id
  type: string
- description: Contact first name
  name: First Name
  type: string
- description: Contact last name
  name: Last Name
  type: string
- description: Contact middle name
  name: Middle Name
  type: string
- description: Salutation or title prefix (e.g., Mr., Ms., Dr.)
  name: Salutation
  type: string
- description: Job title or role within the organization
  name: Job Title
  type: string
- description: Department within the organization
  name: Department
  type: string
- description: Primary email address
  name: Email Address
  type: string
- description: Work telephone number
  name: 'Work Phone #'
  type: string
- description: Mobile or cellular phone number
  name: 'Cellular Phone #'
  type: string
- description: Home telephone number
  name: 'Home Phone #'
  type: string
- description: Fax number
  name: 'Fax Phone #'
  type: string
- description: Name of the associated account
  name: Account
  type: string
- description: Row identifier of the associated account
  name: Account Id
  type: string
- description: Employee number if the contact is an internal employee
  name: Employee Number
  type: string
- description: Name of the employer organization
  name: Employer Name
  type: string
- description: Row identifier of the primary Siebel organization for visibility and access control
  name: Primary Organization Id
  type: string
- description: Contact status
  name: Status
  type: string
- description: Preferred method of communication
  name: Contact Method
  type: string
- description: ''
  name: Personal Address
  type: object
provider_name: Oracle Siebel
provider_slug: oracle-siebel
schema_file: json-schema/oracle-siebel-contact-schema.json
slug: oracle-siebel-contact
source_filename: oracle-siebel-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.oracle.com/schemas/oracle-siebel/contact.json\",\n  \"title\": \"Oracle Siebel CRM Contact\",\n  \"description\": \"A Contact business component record in Oracle Siebel CRM representing an individual person associated with an account. Contacts store personal and professional information including name, job title, communication details, and organizational affiliations.\",\n  \"type\": \"object\",\n  \"required\": [\"First Name\", \"Last Name\"],\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique system-generated row identifier for the contact record\"\n    },\n    \"First Name\": {\n      \"type\": \"string\",\n      \"description\": \"Contact first name\",\n      \"minLength\": 1,\n      \"maxLength\": 50\n    },\n    \"Last Name\": {\n      \"type\": \"string\",\n      \"description\": \"Contact last name\",\n      \"minLength\": 1,\n\
  \      \"maxLength\": 50\n    },\n    \"Middle Name\": {\n      \"type\": \"string\",\n      \"description\": \"Contact middle name\"\n    },\n    \"Salutation\": {\n      \"type\": \"string\",\n      \"description\": \"Salutation or title prefix (e.g., Mr., Ms., Dr.)\"\n    },\n    \"Job Title\": {\n      \"type\": \"string\",\n      \"description\": \"Job title or role within the organization\"\n    },\n    \"Department\": {\n      \"type\": \"string\",\n      \"description\": \"Department within the organization\"\n    },\n    \"Email Address\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Primary email address\"\n    },\n    \"Work Phone #\": {\n      \"type\": \"string\",\n      \"description\": \"Work telephone number\"\n    },\n    \"Cellular Phone #\": {\n      \"type\": \"string\",\n      \"description\": \"Mobile or cellular phone number\"\n    },\n    \"Home Phone #\": {\n      \"type\": \"string\",\n      \"description\": \"Home telephone\
  \ number\"\n    },\n    \"Fax Phone #\": {\n      \"type\": \"string\",\n      \"description\": \"Fax number\"\n    },\n    \"Account\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the associated account\"\n    },\n    \"Account Id\": {\n      \"type\": \"string\",\n      \"description\": \"Row identifier of the associated account\"\n    },\n    \"Employee Number\": {\n      \"type\": \"string\",\n      \"description\": \"Employee number if the contact is an internal employee\"\n    },\n    \"Employer Name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the employer organization\"\n    },\n    \"Primary Organization Id\": {\n      \"type\": \"string\",\n      \"description\": \"Row identifier of the primary Siebel organization for visibility and access control\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Contact status\",\n      \"enum\": [\"Active\", \"Inactive\"]\n    },\n    \"Contact Method\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"Preferred method of communication\"\n    },\n    \"Personal Address\": {\n      \"$ref\": \"#/$defs/Address\"\n    }\n  },\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"Physical address associated with the contact\",\n      \"properties\": {\n        \"Street Address\": {\n          \"type\": \"string\",\n          \"description\": \"Street address line\"\n        },\n        \"Street Address 2\": {\n          \"type\": \"string\",\n          \"description\": \"Secondary address line\"\n        },\n        \"City\": {\n          \"type\": \"string\",\n          \"description\": \"City name\"\n        },\n        \"State\": {\n          \"type\": \"string\",\n          \"description\": \"State or province\"\n        },\n        \"Postal Code\": {\n          \"type\": \"string\",\n          \"description\": \"Postal or ZIP code\"\n        },\n        \"Country\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Country name\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/json-schema/oracle-siebel-contact-schema.json
tags:
- CRM
- Customer Management
- Enterprise Software
- Marketing Automation
- Oracle
- Sales Automation
- Service Automation
title: Oracle Siebel CRM Contact
---
