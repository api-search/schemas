---
description: Information about a deployment error.
layout: schema
name: ErrorInformation
properties_list:
- description: ''
  name: code
  type: object
- description: ''
  name: message
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-error-information-schema.json
slug: amazon-codedeploy-error-information
source_filename: amazon-codedeploy-error-information-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-error-information-schema.json\",\n  \"title\": \"ErrorInformation\",\n  \"description\": \"Information about a deployment error.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorCode\"\n        },\n        {\n          \"description\": \"<p>For more information, see <a href=\\\"https://docs.aws.amazon.com/codedeploy/latest/userguide/error-codes.html\\\">Error Codes for CodeDeploy</a> in the <a href=\\\"https://docs.aws.amazon.com/codedeploy/latest/userguide\\\">CodeDeploy User Guide</a>.</p> <p>The error code:</p> <ul> <li> <p>APPLICATION_MISSING: The application was missing. This error code is most likely raised if the application is deleted after the deployment is created, but before it\
  \ is started.</p> </li> <li> <p>DEPLOYMENT_GROUP_MISSING: The deployment group was missing. This error code is most likely raised if the deployment group is deleted after the deployment is created, but before it is started.</p> </li> <li> <p>HEALTH_CONSTRAINTS: The deployment failed on too many instances to be successfully deployed within the instance health constraints specified.</p> </li> <li> <p>HEALTH_CONSTRAINTS_INVALID: The revision cannot be successfully deployed within the instance health constraints specified.</p> </li> <li> <p>IAM_ROLE_MISSING: The service role cannot be accessed.</p> </li> <li> <p>IAM_ROLE_PERMISSIONS: The service role does not have the correct permissions.</p> </li> <li> <p>INTERNAL_ERROR: There was an internal error.</p> </li> <li> <p>NO_EC2_SUBSCRIPTION: The calling account is not subscribed to Amazon EC2.</p> </li> <li> <p>NO_INSTANCES: No instances were specified, or no instances can be found.</p> </li> <li> <p>OVER_MAX_INSTANCES: The maximum number of\
  \ instances was exceeded.</p> </li> <li> <p>THROTTLED: The operation was throttled because the calling account exceeded the throttling limits of one or more Amazon Web Services services.</p> </li> <li> <p>TIMEOUT: The deployment has timed out.</p> </li> <li> <p>REVISION_MISSING: The revision ID was missing. This error code is most likely raised if the revision is deleted after the deployment is created, but before it is started.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorMessage\"\n        },\n        {\n          \"description\": \"An accompanying error message.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-error-information-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ErrorInformation
---
