---
description: A sampling rule that services use to decide whether to instrument a request. Rule fields can match properties of the service, or properties of a request. The service can ignore rules that don't match its properties.
layout: schema
name: SamplingRule
properties_list:
- description: ''
  name: RuleName
  type: object
- description: ''
  name: RuleARN
  type: object
- description: ''
  name: ResourceARN
  type: object
- description: ''
  name: Priority
  type: object
- description: ''
  name: FixedRate
  type: object
- description: ''
  name: ReservoirSize
  type: object
- description: ''
  name: ServiceName
  type: object
- description: ''
  name: ServiceType
  type: object
- description: ''
  name: Host
  type: object
- description: ''
  name: HTTPMethod
  type: object
- description: ''
  name: URLPath
  type: object
- description: ''
  name: Version
  type: object
- description: ''
  name: Attributes
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-sampling-rule-schema.json
slug: xray-sampling-rule
source_filename: xray-sampling-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceARN\",\n    \"Priority\",\n    \"FixedRate\",\n    \"ReservoirSize\",\n    \"ServiceName\",\n    \"ServiceType\",\n    \"Host\",\n    \"HTTPMethod\",\n    \"URLPath\",\n    \"Version\"\n  ],\n  \"properties\": {\n    \"RuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleName\"\n        },\n        {\n          \"description\": \"The name of the sampling rule. Specify a rule by either name or ARN, but not both.\"\n        }\n      ]\n    },\n    \"RuleARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ARN of the sampling rule. Specify a rule by either name or ARN, but not both.\"\n        }\n      ]\n    },\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"Matches\
  \ the ARN of the Amazon Web Services resource on which the service runs.\"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Priority\"\n        },\n        {\n          \"description\": \"The priority of the sampling rule.\"\n        }\n      ]\n    },\n    \"FixedRate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FixedRate\"\n        },\n        {\n          \"description\": \"The percentage of matching requests to instrument, after the reservoir is exhausted.\"\n        }\n      ]\n    },\n    \"ReservoirSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservoirSize\"\n        },\n        {\n          \"description\": \"A fixed number of matching requests to instrument per second, prior to applying the fixed rate. The reservoir is not used directly by services, but applies to all services using the rule collectively.\"\n        }\n      ]\n\
  \    },\n    \"ServiceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceName\"\n        },\n        {\n          \"description\": \"Matches the <code>name</code> that the service uses to identify itself in segments.\"\n        }\n      ]\n    },\n    \"ServiceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceType\"\n        },\n        {\n          \"description\": \"Matches the <code>origin</code> that the service uses to identify its type in segments.\"\n        }\n      ]\n    },\n    \"Host\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Host\"\n        },\n        {\n          \"description\": \"Matches the hostname from a request URL.\"\n        }\n      ]\n    },\n    \"HTTPMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HTTPMethod\"\n        },\n        {\n          \"description\": \"Matches the HTTP method of a request.\"\n\
  \        }\n      ]\n    },\n    \"URLPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/URLPath\"\n        },\n        {\n          \"description\": \"Matches the path from a request URL.\"\n        }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version of the sampling rule format (<code>1</code>).\"\n        }\n      ]\n    },\n    \"Attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeMap\"\n        },\n        {\n          \"description\": \"Matches attributes derived from the request.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A sampling rule that services use to decide whether to instrument a request. Rule fields can match properties of the service, or properties of a request. The service can ignore rules that don't match its properties.\",\n  \"$schema\"\
  : \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SamplingRule\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-sampling-rule-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-sampling-rule-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: SamplingRule
---
