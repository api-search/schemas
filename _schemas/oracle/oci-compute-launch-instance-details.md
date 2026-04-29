---
description: Instance launch details. Use this to provide the necessary configuration when launching a new compute instance.
layout: schema
name: LaunchInstanceDetails
properties_list:
- description: The OCID of the compartment to create the instance in
  name: compartmentId
  type: string
- description: The availability domain of the instance (e.g., Uocm:PHX-AD-1)
  name: availabilityDomain
  type: string
- description: A user-friendly name for the instance. Does not have to be unique. Avoid entering confidential information.
  name: displayName
  type: string
- description: The shape of the instance. The shape determines the number of CPUs and amount of memory allocated to the instance.
  name: shape
  type: string
- description: Custom metadata key/value pairs for the instance. Common keys include ssh_authorized_keys and user_data.
  name: metadata
  type: object
- description: Additional metadata key/value pairs that can contain nested JSON.
  name: extendedMetadata
  type: object
- description: A fault domain is a grouping of hardware and infrastructure within an availability domain. Specify the fault domain to place the instance in, or let the system choose one for you.
  name: faultDomain
  type: string
- description: Whether to enable in-transit encryption for the data volume's paravirtualized attachment
  name: isPvEncryptionInTransitEnabled
  type: boolean
- description: The OCID of the capacity reservation to launch the instance into
  name: capacityReservationId
  type: string
- description: The OCID of the dedicated VM host to place the instance on
  name: dedicatedVmHostId
  type: string
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-launch-instance-details-schema.json
slug: oci-compute-launch-instance-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LaunchInstanceDetails\",\n  \"type\": \"object\",\n  \"description\": \"Instance launch details. Use this to provide the necessary configuration when launching a new compute instance.\",\n  \"properties\": {\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment to create the instance in\"\n    },\n    \"availabilityDomain\": {\n      \"type\": \"string\",\n      \"description\": \"The availability domain of the instance (e.g., Uocm:PHX-AD-1)\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly name for the instance. Does not have to be unique. Avoid entering confidential information.\"\n    },\n    \"shape\": {\n      \"type\": \"string\",\n      \"description\": \"The shape of the instance. The shape determines the number of CPUs and amount of memory allocated to the instance.\"\n    },\n\
  \    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Custom metadata key/value pairs for the instance. Common keys include ssh_authorized_keys and user_data.\"\n    },\n    \"extendedMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Additional metadata key/value pairs that can contain nested JSON.\"\n    },\n    \"faultDomain\": {\n      \"type\": \"string\",\n      \"description\": \"A fault domain is a grouping of hardware and infrastructure within an availability domain. Specify the fault domain to place the instance in, or let the system choose one for you.\"\n    },\n    \"isPvEncryptionInTransitEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable in-transit encryption for the data volume's paravirtualized attachment\"\n    },\n    \"capacityReservationId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the capacity reservation to launch the instance into\"\n    },\n    \"dedicatedVmHostId\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the dedicated VM host to place the instance on\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-launch-instance-details-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: LaunchInstanceDetails
---
