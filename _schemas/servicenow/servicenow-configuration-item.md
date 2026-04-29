---
description: A ServiceNow CMDB configuration item record representing a hardware, software, or service component tracked in the Configuration Management Database.
layout: schema
name: ServiceNow Configuration Item
properties_list:
- description: The unique 32-character system identifier for the configuration item.
  name: sys_id
  type: string
- description: The display name of the configuration item.
  name: name
  type: string
- description: The CMDB class name identifying the type of CI, such as cmdb_ci_server, cmdb_ci_appl, or cmdb_ci_service.
  name: sys_class_name
  type: string
- description: The category of the configuration item.
  name: category
  type:
  - string
  - 'null'
- description: The subcategory of the configuration item.
  name: subcategory
  type:
  - string
  - 'null'
- description: A brief description of the configuration item.
  name: short_description
  type:
  - string
  - 'null'
- description: 'The operational status: 1=Operational, 2=Non-Operational, 3=Repair in Progress, 4=DR Standby, 5=Ready, 6=Retired.'
  name: operational_status
  type: string
- description: 'The install status: 1=Installed, 2=In Maintenance, 3=Pending Install, 4=Pending Repair, 5=In Stock, 6=Retired, 7=Stolen, 8=Absent, 100=On Order.'
  name: install_status
  type: string
- description: The serial number of the hardware asset.
  name: serial_number
  type:
  - string
  - 'null'
- description: The asset tag identifier.
  name: asset_tag
  type:
  - string
  - 'null'
- description: The IP address of the CI.
  name: ip_address
  type:
  - string
  - 'null'
- description: The MAC address of the CI.
  name: mac_address
  type:
  - string
  - 'null'
- description: The DNS domain of the CI.
  name: dns_domain
  type:
  - string
  - 'null'
- description: The fully qualified domain name.
  name: fqdn
  type:
  - string
  - 'null'
- description: The operating system installed on the CI.
  name: os
  type:
  - string
  - 'null'
- description: The version of the operating system.
  name: os_version
  type:
  - string
  - 'null'
- description: The OS domain.
  name: os_domain
  type:
  - string
  - 'null'
- description: The CPU type.
  name: cpu_type
  type:
  - string
  - 'null'
- description: The number of CPUs.
  name: cpu_count
  type:
  - integer
  - 'null'
- description: The CPU speed in MHz.
  name: cpu_speed
  type:
  - number
  - 'null'
- description: The amount of RAM in MB.
  name: ram
  type:
  - integer
  - 'null'
- description: The total disk space in GB.
  name: disk_space
  type:
  - number
  - 'null'
- description: The manufacturer of the CI.
  name: manufacturer
  type: object
- description: The model of the CI.
  name: model_id
  type: object
- description: The model number.
  name: model_number
  type:
  - string
  - 'null'
- description: The vendor of the CI.
  name: vendor
  type: object
- description: The physical location of the CI.
  name: location
  type: object
- description: The department that owns the CI.
  name: department
  type: object
- description: The company that owns the CI.
  name: company
  type: object
- description: The user assigned to the CI.
  name: assigned_to
  type: object
- description: The user managing the CI.
  name: managed_by
  type: object
- description: The user who owns the CI.
  name: owned_by
  type: object
- description: The group responsible for supporting the CI.
  name: support_group
  type: object
- description: The user providing primary support for the CI.
  name: supported_by
  type: object
- description: The source that discovered or populated this CI.
  name: discovery_source
  type:
  - string
  - 'null'
- description: When the CI was first discovered.
  name: first_discovered
  type:
  - string
  - 'null'
- description: When the CI was last discovered.
  name: last_discovered
  type:
  - string
  - 'null'
- description: Whether the CI can print.
  name: can_print
  type: boolean
- description: Whether the CI is unverified.
  name: unverified
  type: boolean
- description: The date and time the record was created.
  name: sys_created_on
  type: string
- description: The user who created the record.
  name: sys_created_by
  type: string
- description: The date and time the record was last updated.
  name: sys_updated_on
  type: string
- description: The user who last updated the record.
  name: sys_updated_by
  type: string
- description: The number of times the record has been modified.
  name: sys_mod_count
  type: integer
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-configuration-item-schema.json
slug: servicenow-configuration-item
source_filename: servicenow-configuration-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://servicenow.com/schemas/servicenow/configuration-item.json\",\n  \"title\": \"ServiceNow Configuration Item\",\n  \"description\": \"A ServiceNow CMDB configuration item record representing a hardware, software, or service component tracked in the Configuration Management Database.\",\n  \"type\": \"object\",\n  \"required\": [\"sys_id\", \"name\", \"sys_class_name\"],\n  \"properties\": {\n    \"sys_id\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[a-f0-9]{32}$\",\n      \"description\": \"The unique 32-character system identifier for the configuration item.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the configuration item.\"\n    },\n    \"sys_class_name\": {\n      \"type\": \"string\",\n      \"description\": \"The CMDB class name identifying the type of CI, such as cmdb_ci_server, cmdb_ci_appl, or cmdb_ci_service.\"\
  \n    },\n    \"category\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The category of the configuration item.\"\n    },\n    \"subcategory\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The subcategory of the configuration item.\"\n    },\n    \"short_description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A brief description of the configuration item.\"\n    },\n    \"operational_status\": {\n      \"type\": \"string\",\n      \"enum\": [\"1\", \"2\", \"3\", \"4\", \"5\", \"6\"],\n      \"description\": \"The operational status: 1=Operational, 2=Non-Operational, 3=Repair in Progress, 4=DR Standby, 5=Ready, 6=Retired.\"\n    },\n    \"install_status\": {\n      \"type\": \"string\",\n      \"enum\": [\"1\", \"2\", \"3\", \"4\", \"5\", \"6\", \"7\", \"8\", \"100\"],\n      \"description\": \"The install status: 1=Installed, 2=In Maintenance, 3=Pending Install, 4=Pending Repair, 5=In Stock, 6=Retired, 7=Stolen,\
  \ 8=Absent, 100=On Order.\"\n    },\n    \"serial_number\": {\n      \"type\": [\"string\", \"null\"],\n      \"maxLength\": 255,\n      \"description\": \"The serial number of the hardware asset.\"\n    },\n    \"asset_tag\": {\n      \"type\": [\"string\", \"null\"],\n      \"maxLength\": 255,\n      \"description\": \"The asset tag identifier.\"\n    },\n    \"ip_address\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The IP address of the CI.\"\n    },\n    \"mac_address\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The MAC address of the CI.\"\n    },\n    \"dns_domain\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The DNS domain of the CI.\"\n    },\n    \"fqdn\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The fully qualified domain name.\"\n    },\n    \"os\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The operating system installed on the CI.\"\n    },\n\
  \    \"os_version\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The version of the operating system.\"\n    },\n    \"os_domain\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The OS domain.\"\n    },\n    \"cpu_type\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The CPU type.\"\n    },\n    \"cpu_count\": {\n      \"type\": [\"integer\", \"null\"],\n      \"minimum\": 0,\n      \"description\": \"The number of CPUs.\"\n    },\n    \"cpu_speed\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"The CPU speed in MHz.\"\n    },\n    \"ram\": {\n      \"type\": [\"integer\", \"null\"],\n      \"minimum\": 0,\n      \"description\": \"The amount of RAM in MB.\"\n    },\n    \"disk_space\": {\n      \"type\": [\"number\", \"null\"],\n      \"minimum\": 0,\n      \"description\": \"The total disk space in GB.\"\n    },\n    \"manufacturer\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"\
  description\": \"The manufacturer of the CI.\"\n    },\n    \"model_id\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The model of the CI.\"\n    },\n    \"model_number\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The model number.\"\n    },\n    \"vendor\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The vendor of the CI.\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The physical location of the CI.\"\n    },\n    \"department\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The department that owns the CI.\"\n    },\n    \"company\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The company that owns the CI.\"\n    },\n    \"assigned_to\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The user assigned to the CI.\"\n    },\n    \"managed_by\": {\n      \"$ref\": \"\
  #/$defs/ReferenceField\",\n      \"description\": \"The user managing the CI.\"\n    },\n    \"owned_by\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The user who owns the CI.\"\n    },\n    \"support_group\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The group responsible for supporting the CI.\"\n    },\n    \"supported_by\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The user providing primary support for the CI.\"\n    },\n    \"discovery_source\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The source that discovered or populated this CI.\"\n    },\n    \"first_discovered\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"When the CI was first discovered.\"\n    },\n    \"last_discovered\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"When the CI was last\
  \ discovered.\"\n    },\n    \"can_print\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the CI can print.\"\n    },\n    \"unverified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the CI is unverified.\"\n    },\n    \"sys_created_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the record was created.\"\n    },\n    \"sys_created_by\": {\n      \"type\": \"string\",\n      \"description\": \"The user who created the record.\"\n    },\n    \"sys_updated_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the record was last updated.\"\n    },\n    \"sys_updated_by\": {\n      \"type\": \"string\",\n      \"description\": \"The user who last updated the record.\"\n    },\n    \"sys_mod_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of times the record has been modified.\"\
  \n    }\n  },\n  \"$defs\": {\n    \"ReferenceField\": {\n      \"type\": [\"object\", \"string\", \"null\"],\n      \"description\": \"A ServiceNow reference field that can be a sys_id string or an object containing a link and value.\",\n      \"properties\": {\n        \"link\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The API URL to the referenced record.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The sys_id of the referenced record.\"\n        },\n        \"display_value\": {\n          \"type\": \"string\",\n          \"description\": \"The display value of the referenced record.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-configuration-item-schema.json
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
title: ServiceNow Configuration Item
---
