---
description: Guest operating system identity information from VMware Tools
layout: schema
name: GuestIdentityInfo
properties_list:
- description: Guest OS full name
  name: name
  type: string
- description: Guest OS family
  name: family
  type: string
- description: ''
  name: full_name
  type: object
- description: Guest hostname
  name: host_name
  type: string
- description: Primary IP address of the guest
  name: ip_address
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-guest-identity-info-schema.json
slug: vmware-vsphere-guest-identity-info
source_filename: vmware-vsphere-guest-identity-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GuestIdentityInfo\",\n  \"type\": \"object\",\n  \"description\": \"Guest operating system identity information from VMware Tools\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Guest OS full name\"\n    },\n    \"family\": {\n      \"type\": \"string\",\n      \"description\": \"Guest OS family\"\n    },\n    \"full_name\": {\n      \"type\": \"object\"\n    },\n    \"host_name\": {\n      \"type\": \"string\",\n      \"description\": \"Guest hostname\"\n    },\n    \"ip_address\": {\n      \"type\": \"string\",\n      \"description\": \"Primary IP address of the guest\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-guest-identity-info-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: GuestIdentityInfo
---
