---
description: StartResourceEvaluationRequest schema
layout: schema
name: StartResourceEvaluationRequest
properties_list:
- description: ''
  name: ResourceDetails
  type: object
- description: ''
  name: EvaluationContext
  type: object
- description: ''
  name: EvaluationMode
  type: object
- description: ''
  name: EvaluationTimeout
  type: object
- description: ''
  name: ClientToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-start-resource-evaluation-request-schema.json
slug: config-start-resource-evaluation-request
source_filename: config-start-resource-evaluation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-start-resource-evaluation-request-schema.json\",\n  \"title\": \"StartResourceEvaluationRequest\",\n  \"description\": \"StartResourceEvaluationRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceDetails\"\n        },\n        {\n          \"description\": \"Returns a <code>ResourceDetails</code> object.\"\n        }\n      ]\n    },\n    \"EvaluationContext\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationContext\"\n        },\n        {\n          \"description\": \"Returns an <code>EvaluationContext</code> object.\"\n        }\n      ]\n    },\n    \"EvaluationMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationMode\"\
  \n        },\n        {\n          \"description\": \"The mode of an evaluation. The valid values for this API are <code>DETECTIVE</code> and <code>PROACTIVE</code>.\"\n        }\n      ]\n    },\n    \"EvaluationTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationTimeout\"\n        },\n        {\n          \"description\": \"The timeout for an evaluation. The default is 900 seconds. You cannot specify a number greater than 3600. If you specify 0, Config uses the default.\"\n        }\n      ]\n    },\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"<p>A client token is a unique, case-sensitive string of up to 64 ASCII characters. To make an idempotent API request using one of these actions, specify a client token in the request.</p> <note> <p>Avoid reusing the same client token for other API requests. If you retry a request\
  \ that completed successfully using the same client token and the same parameters, the retry succeeds without performing any further actions. If you retry a successful request using the same client token, but one or more of the parameters are different, other than the Region or Availability Zone, the retry fails with an IdempotentParameterMismatch error.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceDetails\",\n    \"EvaluationMode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-start-resource-evaluation-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: StartResourceEvaluationRequest
---
