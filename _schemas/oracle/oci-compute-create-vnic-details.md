---
description: Contains properties for a VNIC. Used when launching an instance or creating a VNIC attachment.
layout: schema
name: CreateVnicDetails
properties_list:
- description: The OCID of the subnet to create the VNIC in
  name: subnetId
  type: string
- description: A user-friendly name for the VNIC. Does not have to be unique.
  name: displayName
  type: string
- description: Whether the VNIC should be assigned a public IP address. Defaults to whether the subnet is public or private.
  name: assignPublicIp
  type: boolean
- description: Whether the VNIC should be assigned a DNS record. Defaults to true.
  name: assignPrivateDnsRecord
  type: boolean
- description: A private IP address of your choice to assign to the VNIC. Must be an available IP address within the subnet CIDR.
  name: privateIp
  type: string
- description: The hostname for the VNIC primary private IP. Used for DNS.
  name: hostnameLabel
  type: string
- description: A list of the OCIDs of the network security groups to add the VNIC to
  name: nsgIds
  type: array
- description: Whether the source/destination check is disabled on the VNIC. Defaults to false.
  name: skipSourceDestCheck
  type: boolean
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-create-vnic-details-schema.json
slug: oci-compute-create-vnic-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateVnicDetails\",\n  \"type\": \"object\",\n  \"description\": \"Contains properties for a VNIC. Used when launching an instance or creating a VNIC attachment.\",\n  \"properties\": {\n    \"subnetId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the subnet to create the VNIC in\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly name for the VNIC. Does not have to be unique.\"\n    },\n    \"assignPublicIp\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the VNIC should be assigned a public IP address. Defaults to whether the subnet is public or private.\"\n    },\n    \"assignPrivateDnsRecord\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the VNIC should be assigned a DNS record. Defaults to true.\"\n    },\n    \"privateIp\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"A private IP address of your choice to assign to the VNIC. Must be an available IP address within the subnet CIDR.\"\n    },\n    \"hostnameLabel\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname for the VNIC primary private IP. Used for DNS.\"\n    },\n    \"nsgIds\": {\n      \"type\": \"array\",\n      \"description\": \"A list of the OCIDs of the network security groups to add the VNIC to\"\n    },\n    \"skipSourceDestCheck\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the source/destination check is disabled on the VNIC. Defaults to false.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-create-vnic-details-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: CreateVnicDetails
---
