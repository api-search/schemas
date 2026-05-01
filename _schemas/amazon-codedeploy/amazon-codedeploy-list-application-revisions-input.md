---
description: Represents the input of a <code>ListApplicationRevisions</code> operation.
layout: schema
name: ListApplicationRevisionsInput
properties_list:
- description: ''
  name: applicationName
  type: object
- description: ''
  name: sortBy
  type: object
- description: ''
  name: sortOrder
  type: object
- description: ''
  name: s3Bucket
  type: object
- description: ''
  name: s3KeyPrefix
  type: object
- description: ''
  name: deployed
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-list-application-revisions-input-schema.json
slug: amazon-codedeploy-list-application-revisions-input
source_filename: amazon-codedeploy-list-application-revisions-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-application-revisions-input-schema.json\",\n  \"title\": \"ListApplicationRevisionsInput\",\n  \"description\": \" Represents the input of a <code>ListApplicationRevisions</code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \" The name of an CodeDeploy application associated with the IAM user or Amazon Web Services account. \"\n        }\n      ]\n    },\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationRevisionSortBy\"\n        },\n        {\n          \"description\": \"<p>The column name to use to sort the list results:</p> <ul> <li> <p>\
  \ <code>registerTime</code>: Sort by the time the revisions were registered with CodeDeploy.</p> </li> <li> <p> <code>firstUsedTime</code>: Sort by the time the revisions were first used in a deployment.</p> </li> <li> <p> <code>lastUsedTime</code>: Sort by the time the revisions were last used in a deployment.</p> </li> </ul> <p> If not specified or set to null, the results are returned in an arbitrary order. </p>\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\n        },\n        {\n          \"description\": \"<p> The order in which to sort the list results: </p> <ul> <li> <p> <code>ascending</code>: ascending order.</p> </li> <li> <p> <code>descending</code>: descending order.</p> </li> </ul> <p>If not specified, the results are sorted in ascending order.</p> <p>If set to null, the results are sorted in an arbitrary order.</p>\"\n        }\n      ]\n    },\n    \"s3Bucket\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/S3Bucket\"\n        },\n        {\n          \"description\": \"<p> An Amazon S3 bucket name to limit the search for revisions. </p> <p> If set to null, all of the user's buckets are searched. </p>\"\n        }\n      ]\n    },\n    \"s3KeyPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Key\"\n        },\n        {\n          \"description\": \" A key prefix for the set of Amazon S3 objects to limit the search for revisions. \"\n        }\n      ]\n    },\n    \"deployed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListStateFilterAction\"\n        },\n        {\n          \"description\": \"<p> Whether to list revisions based on whether the revision is the target revision of a deployment group: </p> <ul> <li> <p> <code>include</code>: List revisions that are target revisions of a deployment group.</p> </li> <li> <p> <code>exclude</code>: Do not list revisions\
  \ that are target revisions of a deployment group.</p> </li> <li> <p> <code>ignore</code>: List all revisions.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"An identifier returned from the previous <code>ListApplicationRevisions</code> call. It can be used to return the next set of applications in the list.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-list-application-revisions-input-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ListApplicationRevisionsInput
---
