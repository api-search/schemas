---
description: IP address block. This is often the address block of the DNS server used for your self-managed domain.
layout: schema
name: IpRoute
properties_list:
- description: ''
  name: CidrIp
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-ip-route-schema.json
slug: amazon-directory-service-ip-route
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-ip-route-schema.json\",\n  \"title\": \"IpRoute\",\n  \"description\": \"IP address block. This is often the address block of the DNS server used for your self-managed domain. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CidrIp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CidrIp\"\n        },\n        {\n          \"description\": \"IP address block using CIDR format, for example 10.0.0.0/24. This is often the address block of the DNS server used for your self-managed domain. For a single IP address use a CIDR address block with /32. For example 10.0.0.0/32.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n\
  \          \"description\": \"Description of the address block.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-ip-route-schema.json
tags:
- Active Directory
- Authentication
- AWS
- Directory Services
- Identity Management
title: IpRoute
---
