---
description: Represents a Cloud DNS managed zone resource, including its DNS name, name servers, visibility, DNSSEC configuration, and associated metadata.
layout: schema
name: Google Cloud DNS Managed Zone
properties_list:
- description: Unique identifier for the resource.
  name: id
  type: string
- description: User-assigned name for this resource.
  name: name
  type: string
- description: The DNS name of this managed zone, for instance example.com.
  name: dnsName
  type: string
- description: A mutable string of at most 1024 characters associated with this resource.
  name: description
  type: string
- description: Delegate your managed zone to these virtual name servers.
  name: nameServers
  type: array
- description: 'The zone''s visibility: public or private.'
  name: visibility
  type: string
- description: DNSSEC configuration for this managed zone.
  name: dnssecConfig
  type: object
- description: The time that this resource was created on the server.
  name: creationTime
  type: string
provider_name: Google Cloud DNS
provider_slug: google-cloud-dns
schema_file: json-schema/dns-managedzone.json
slug: dns-managedzone
source_filename: dns-managedzone.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-search/google-cloud-dns/refs/heads/main/json-schema/dns-managedzone.json\",\n  \"title\": \"Google Cloud DNS Managed Zone\",\n  \"description\": \"Represents a Cloud DNS managed zone resource, including its DNS name, name servers, visibility, DNSSEC configuration, and associated metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the resource.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"User-assigned name for this resource.\"\n    },\n    \"dnsName\": {\n      \"type\": \"string\",\n      \"description\": \"The DNS name of this managed zone, for instance example.com.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A mutable string of at most 1024 characters associated with this resource.\"\
  \n    },\n    \"nameServers\": {\n      \"type\": \"array\",\n      \"description\": \"Delegate your managed zone to these virtual name servers.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"description\": \"The zone's visibility: public or private.\",\n      \"enum\": [\n        \"public\",\n        \"private\"\n      ]\n    },\n    \"dnssecConfig\": {\n      \"type\": \"object\",\n      \"description\": \"DNSSEC configuration for this managed zone.\",\n      \"properties\": {\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies whether DNSSEC is enabled.\",\n          \"enum\": [\n            \"off\",\n            \"on\",\n            \"transfer\"\n          ]\n        },\n        \"kind\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"creationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"The time that this resource was created on the server.\"\n    }\n  },\n  \"required\": [\"name\", \"dnsName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dns/refs/heads/main/json-schema/dns-managedzone.json
tags:
- DNS
- Domain Names
- Google Cloud
- Name Resolution
- Networking
title: Google Cloud DNS Managed Zone
---
