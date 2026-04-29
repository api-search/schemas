---
description: The details for a console connection to an instance. A console connection enables you to connect to the serial console or VNC console of an instance for troubleshooting.
layout: schema
name: InstanceConsoleConnection
properties_list:
- description: The OCID of the console connection
  name: id
  type: string
- description: The OCID of the instance the console connection connects to
  name: instanceId
  type: string
- description: The OCID of the compartment
  name: compartmentId
  type: string
- description: The SSH connection string for the console connection
  name: connectionString
  type: string
- description: The SSH public key fingerprint for the console connection
  name: fingerprint
  type: string
- description: The SSH connection string for the VNC console
  name: vncConnectionString
  type: string
- description: The lifecycle state of the console connection
  name: lifecycleState
  type: string
- description: The SSH public key fingerprint of the service host
  name: serviceHostKeyFingerprint
  type: string
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-instance-console-connection-schema.json
slug: oci-compute-instance-console-connection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InstanceConsoleConnection\",\n  \"type\": \"object\",\n  \"description\": \"The details for a console connection to an instance. A console connection enables you to connect to the serial console or VNC console of an instance for troubleshooting.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the console connection\"\n    },\n    \"instanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the instance the console connection connects to\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment\"\n    },\n    \"connectionString\": {\n      \"type\": \"string\",\n      \"description\": \"The SSH connection string for the console connection\"\n    },\n    \"fingerprint\": {\n      \"type\": \"string\",\n      \"description\": \"The SSH public key fingerprint\
  \ for the console connection\"\n    },\n    \"vncConnectionString\": {\n      \"type\": \"string\",\n      \"description\": \"The SSH connection string for the VNC console\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"description\": \"The lifecycle state of the console connection\"\n    },\n    \"serviceHostKeyFingerprint\": {\n      \"type\": \"string\",\n      \"description\": \"The SSH public key fingerprint of the service host\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-instance-console-connection-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: InstanceConsoleConnection
---
