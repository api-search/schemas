---
description: Points to a remote domain with which you are setting up a trust relationship. Conditional forwarders are required in order to set up a trust relationship with another domain.
layout: schema
name: ConditionalForwarder
properties_list:
- description: ''
  name: RemoteDomainName
  type: object
- description: ''
  name: DnsIpAddrs
  type: object
- description: ''
  name: ReplicationScope
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-conditional-forwarder-schema.json
slug: amazon-directory-service-conditional-forwarder
source_filename: amazon-directory-service-conditional-forwarder-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-conditional-forwarder-schema.json\",\n  \"title\": \"ConditionalForwarder\",\n  \"description\": \"Points to a remote domain with which you are setting up a trust relationship. Conditional forwarders are required in order to set up a trust relationship with another domain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RemoteDomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemoteDomainName\"\n        },\n        {\n          \"description\": \"The fully qualified domain name (FQDN) of the remote domains pointed to by the conditional forwarder.\"\n        }\n      ]\n    },\n    \"DnsIpAddrs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsIpAddrs\"\n        },\n        {\n          \"\
  description\": \"The IP addresses of the remote DNS server associated with RemoteDomainName. This is the IP address of the DNS server that your conditional forwarder points to.\"\n        }\n      ]\n    },\n    \"ReplicationScope\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplicationScope\"\n        },\n        {\n          \"description\": \"The replication scope of the conditional forwarder. The only allowed value is <code>Domain</code>, which will replicate the conditional forwarder to all of the domain controllers for your Amazon Web Services directory.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-conditional-forwarder-schema.json
tags:
- Active Directory
- Authentication
- Directory Services
- Identity Management
title: ConditionalForwarder
---
