---
description: PutResourcePolicyRequest schema from Amazon Glue API
layout: schema
name: PutResourcePolicyRequest
properties_list:
- description: ''
  name: PolicyInJson
  type: object
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: PolicyHashCondition
  type: object
- description: ''
  name: PolicyExistsCondition
  type: object
- description: ''
  name: EnableHybrid
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-put-resource-policy-request-schema.json
slug: glue-put-resource-policy-request
source_filename: glue-put-resource-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-put-resource-policy-request-schema.json\",\n  \"title\": \"PutResourcePolicyRequest\",\n  \"description\": \"PutResourcePolicyRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PolicyInJson\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyJsonString\"\n        },\n        {\n          \"description\": \"Contains the policy document to set, in JSON format.\"\n        }\n      ]\n    },\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueResourceArn\"\n        },\n        {\n          \"description\": \"Do not use. For internal use only.\"\n        }\n      ]\n    },\n    \"PolicyHashCondition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\
  \n        },\n        {\n          \"description\": \"The hash value returned when the previous policy was set using <code>PutResourcePolicy</code>. Its purpose is to prevent concurrent modifications of a policy. Do not use this parameter if no previous policy has been set.\"\n        }\n      ]\n    },\n    \"PolicyExistsCondition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExistCondition\"\n        },\n        {\n          \"description\": \"A value of <code>MUST_EXIST</code> is used to update a policy. A value of <code>NOT_EXIST</code> is used to create a new policy. If a value of <code>NONE</code> or a null value is used, the call does not depend on the existence of a policy.\"\n        }\n      ]\n    },\n    \"EnableHybrid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnableHybridValues\"\n        },\n        {\n          \"description\": \"<p>If <code>'TRUE'</code>, indicates that you are using both methods to\
  \ grant cross-account access to Data Catalog resources:</p> <ul> <li> <p>By directly updating the resource policy with <code>PutResourePolicy</code> </p> </li> <li> <p>By using the <b>Grant permissions</b> command on the Amazon Web Services Management Console.</p> </li> </ul> <p>Must be set to <code>'TRUE'</code> if you have already used the Management Console to grant cross-account access, otherwise the call fails. Default is 'FALSE'.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PolicyInJson\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-put-resource-policy-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: PutResourcePolicyRequest
---
