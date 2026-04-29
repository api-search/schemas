---
description: An object that represents the DNS service discovery information for your virtual node.
layout: schema
name: DnsServiceDiscovery
properties_list:
- description: ''
  name: hostname
  type: object
- description: ''
  name: ipPreference
  type: object
- description: ''
  name: responseType
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-dnsservicediscovery-schema.json
slug: amazon-app-mesh-dnsservicediscovery
source_filename: amazon-app-mesh-dnsservicediscovery-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DnsServiceDiscovery\",\n  \"description\": \"An object that represents the DNS service discovery information for your virtual node.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hostname\": {},\n    \"ipPreference\": {},\n    \"responseType\": {}\n  },\n  \"required\": [\n    \"hostname\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-dnsservicediscovery-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: DnsServiceDiscovery
---
