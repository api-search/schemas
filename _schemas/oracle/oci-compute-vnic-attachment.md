---
description: Represents the attachment between an instance and a VNIC. Each instance has a primary VNIC attachment created during launch.
layout: schema
name: VnicAttachment
properties_list:
- description: The OCID of the VNIC attachment
  name: id
  type: string
- description: The OCID of the instance
  name: instanceId
  type: string
- description: The OCID of the compartment
  name: compartmentId
  type: string
- description: The availability domain of the instance
  name: availabilityDomain
  type: string
- description: A user-friendly name for the attachment
  name: displayName
  type: string
- description: The OCID of the VNIC
  name: vnicId
  type: string
- description: The OCID of the subnet of the VNIC
  name: subnetId
  type: string
- description: Which physical network interface card (NIC) the VNIC uses. 0 for the primary VNIC.
  name: nicIndex
  type: integer
- description: The Oracle-assigned VLAN tag of the VNIC attachment
  name: vlanTag
  type: integer
- description: The OCID of the VLAN to create the VNIC in
  name: vlanId
  type: string
- description: The lifecycle state of the VNIC attachment
  name: lifecycleState
  type: string
- description: The date and time the VNIC attachment was created
  name: timeCreated
  type: string
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-vnic-attachment-schema.json
slug: oci-compute-vnic-attachment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VnicAttachment\",\n  \"type\": \"object\",\n  \"description\": \"Represents the attachment between an instance and a VNIC. Each instance has a primary VNIC attachment created during launch.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the VNIC attachment\"\n    },\n    \"instanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the instance\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment\"\n    },\n    \"availabilityDomain\": {\n      \"type\": \"string\",\n      \"description\": \"The availability domain of the instance\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly name for the attachment\"\n    },\n    \"vnicId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID\
  \ of the VNIC\"\n    },\n    \"subnetId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the subnet of the VNIC\"\n    },\n    \"nicIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"Which physical network interface card (NIC) the VNIC uses. 0 for the primary VNIC.\"\n    },\n    \"vlanTag\": {\n      \"type\": \"integer\",\n      \"description\": \"The Oracle-assigned VLAN tag of the VNIC attachment\"\n    },\n    \"vlanId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the VLAN to create the VNIC in\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"description\": \"The lifecycle state of the VNIC attachment\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the VNIC attachment was created\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-vnic-attachment-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: VnicAttachment
---
