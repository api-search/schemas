---
description: ''
layout: schema
name: DescribeCustomDomainsResponse
properties_list:
- description: ''
  name: DNSTarget
  type: object
- description: ''
  name: ServiceArn
  type: object
- description: ''
  name: CustomDomains
  type: object
- description: ''
  name: VpcDNSTargets
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-describecustomdomainsresponse-schema.json
slug: amazon-app-runner-describecustomdomainsresponse
source_filename: amazon-app-runner-describecustomdomainsresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DescribeCustomDomainsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DNSTarget\": {},\n    \"ServiceArn\": {},\n    \"CustomDomains\": {},\n    \"VpcDNSTargets\": {},\n    \"NextToken\": {}\n  },\n  \"required\": [\n    \"DNSTarget\",\n    \"ServiceArn\",\n    \"CustomDomains\",\n    \"VpcDNSTargets\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-describecustomdomainsresponse-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: DescribeCustomDomainsResponse
---
