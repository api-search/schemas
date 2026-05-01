---
description: Describes a custom domain that's associated with an App Runner service.
layout: schema
name: CustomDomain
properties_list:
- description: ''
  name: DomainName
  type: object
- description: ''
  name: EnableWWWSubdomain
  type: object
- description: ''
  name: CertificateValidationRecords
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-customdomain-schema.json
slug: amazon-app-runner-customdomain
source_filename: amazon-app-runner-customdomain-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CustomDomain\",\n  \"description\": \"Describes a custom domain that's associated with an App Runner service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainName\": {},\n    \"EnableWWWSubdomain\": {},\n    \"CertificateValidationRecords\": {},\n    \"Status\": {}\n  },\n  \"required\": [\n    \"DomainName\",\n    \"EnableWWWSubdomain\",\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-customdomain-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: CustomDomain
---
