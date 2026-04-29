---
description: A full CMDB configuration item record. Fields vary by CI class but common attributes are included below.
layout: schema
name: CmdbInstance
properties_list:
- description: Unique identifier for the configuration item.
  name: sys_id
  type: string
- description: The display name of the configuration item.
  name: name
  type: string
- description: The CMDB class name for this CI.
  name: sys_class_name
  type: string
- description: The category of the CI.
  name: category
  type: string
- description: The subcategory of the CI.
  name: subcategory
  type: string
- description: The operational status of the CI.
  name: operational_status
  type: string
- description: The installation status of the CI.
  name: install_status
  type: string
- description: The serial number of the hardware asset.
  name: serial_number
  type: string
- description: The asset tag identifier.
  name: asset_tag
  type: string
- description: The IP address of the CI.
  name: ip_address
  type: string
- description: The MAC address of the CI.
  name: mac_address
  type: string
- description: The DNS domain of the CI.
  name: dns_domain
  type: string
- description: The fully qualified domain name.
  name: fqdn
  type: string
- description: The operating system.
  name: os
  type: string
- description: The operating system version.
  name: os_version
  type: string
- description: The sys_id of the manufacturer.
  name: manufacturer
  type: string
- description: The sys_id of the model.
  name: model_id
  type: string
- description: The sys_id of the CI location.
  name: location
  type: string
- description: The sys_id of the department.
  name: department
  type: string
- description: The sys_id of the owning company.
  name: company
  type: string
- description: The sys_id of the assigned user.
  name: assigned_to
  type: string
- description: The sys_id of the managing user.
  name: managed_by
  type: string
- description: The sys_id of the owner.
  name: owned_by
  type: string
- description: The sys_id of the support group.
  name: support_group
  type: string
- description: The date and time when the CI was created.
  name: sys_created_on
  type: string
- description: The date and time when the CI was last updated.
  name: sys_updated_on
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-cmdb-instance-cmdb-instance-schema.json
slug: servicenow-cmdb-instance-cmdb-instance
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A full CMDB configuration item record. Fields vary by CI class but common attributes are included below.\",\n  \"properties\": {\n    \"sys_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the configuration item.\",\n      \"example\": \"500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the configuration item.\",\n      \"example\": \"Example Title\"\n    },\n    \"sys_class_name\": {\n      \"type\": \"string\",\n      \"description\": \"The CMDB class name for this CI.\",\n      \"example\": \"example_value\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The category of the CI.\",\n      \"example\": \"example_value\"\n    },\n    \"subcategory\": {\n      \"type\": \"string\",\n      \"description\": \"The subcategory of the CI.\",\n      \"example\": \"example_value\"\n    },\n    \"operational_status\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The operational status of the CI.\",\n      \"example\": \"1\",\n      \"enum\": [\n        \"1\",\n        \"2\",\n        \"3\",\n        \"4\",\n        \"5\",\n        \"6\"\n      ]\n    },\n    \"install_status\": {\n      \"type\": \"string\",\n      \"description\": \"The installation status of the CI.\",\n      \"example\": \"example_value\"\n    },\n    \"serial_number\": {\n      \"type\": \"string\",\n      \"description\": \"The serial number of the hardware asset.\",\n      \"example\": \"example_value\"\n    },\n    \"asset_tag\": {\n      \"type\": \"string\",\n      \"description\": \"The asset tag identifier.\",\n      \"example\": \"example_value\"\n    },\n    \"ip_address\": {\n      \"type\": \"string\",\n      \"description\": \"The IP address of the CI.\",\n      \"example\": \"example_value\"\n    },\n    \"mac_address\": {\n      \"type\": \"string\",\n      \"description\": \"The MAC address of the CI.\"\
  ,\n      \"example\": \"example_value\"\n    },\n    \"dns_domain\": {\n      \"type\": \"string\",\n      \"description\": \"The DNS domain of the CI.\",\n      \"example\": \"example_value\"\n    },\n    \"fqdn\": {\n      \"type\": \"string\",\n      \"description\": \"The fully qualified domain name.\",\n      \"example\": \"example_value\"\n    },\n    \"os\": {\n      \"type\": \"string\",\n      \"description\": \"The operating system.\",\n      \"example\": \"example_value\"\n    },\n    \"os_version\": {\n      \"type\": \"string\",\n      \"description\": \"The operating system version.\",\n      \"example\": \"example_value\"\n    },\n    \"manufacturer\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the manufacturer.\",\n      \"example\": \"example_value\"\n    },\n    \"model_id\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the model.\",\n      \"example\": \"500123\"\n    },\n    \"location\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The sys_id of the CI location.\",\n      \"example\": \"example_value\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the department.\",\n      \"example\": \"example_value\"\n    },\n    \"company\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the owning company.\",\n      \"example\": \"example_value\"\n    },\n    \"assigned_to\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the assigned user.\",\n      \"example\": \"example_value\"\n    },\n    \"managed_by\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the managing user.\",\n      \"example\": \"example_value\"\n    },\n    \"owned_by\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the owner.\",\n      \"example\": \"example_value\"\n    },\n    \"support_group\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the support\
  \ group.\",\n      \"example\": \"example_value\"\n    },\n    \"sys_created_on\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the CI was created.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"sys_updated_on\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the CI was last updated.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CmdbInstance\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-cmdb-instance-cmdb-instance-schema.json
tags:
- Automation
- Cloud Services
- Digital Workflows
- Enterprise Platform
- IT Service Management
- ITSM
- Processes
- T1
- Workflow Automation
- Workflows
title: CmdbInstance
---
