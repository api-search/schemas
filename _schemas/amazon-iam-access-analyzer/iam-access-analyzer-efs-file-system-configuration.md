---
description: <p>The proposed access control configuration for an Amazon EFS file system. You can propose a configuration for a new Amazon EFS file system or an existing Amazon EFS file system that you own by specifying the Amazon EFS policy. For more information, see <a href="https://docs.aws.amazon.com/efs/latest/ug/using-fs.html">Using file systems in Amazon EFS</a>.</p> <ul> <li> <p>If the configuration is for an existing Amazon EFS file system and you do not specify the Amazon EFS policy, then the access preview uses the existing Amazon EFS policy for the file system.</p> </li> <li> <p>If the access preview is for a new resource and you do not specify the policy, then the access preview assumes an Amazon EFS file system without a policy.</p> </li> <li> <p>To propose deletion of an existing Amazon EFS file system policy, you can specify an empty string for the Amazon EFS policy.</p> </li> </ul>
layout: schema
name: EfsFileSystemConfiguration
properties_list:
- description: ''
  name: fileSystemPolicy
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-efs-file-system-configuration-schema.json
slug: iam-access-analyzer-efs-file-system-configuration
source_filename: iam-access-analyzer-efs-file-system-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-efs-file-system-configuration-schema.json\",\n  \"title\": \"EfsFileSystemConfiguration\",\n  \"description\": \"<p>The proposed access control configuration for an Amazon EFS file system. You can propose a configuration for a new Amazon EFS file system or an existing Amazon EFS file system that you own by specifying the Amazon EFS policy. For more information, see <a href=\\\"https://docs.aws.amazon.com/efs/latest/ug/using-fs.html\\\">Using file systems in Amazon EFS</a>.</p> <ul> <li> <p>If the configuration is for an existing Amazon EFS file system and you do not specify the Amazon EFS policy, then the access preview uses the existing Amazon EFS policy for the file system.</p> </li> <li> <p>If the access preview is for a new resource and you do not specify the policy,\
  \ then the access preview assumes an Amazon EFS file system without a policy.</p> </li> <li> <p>To propose deletion of an existing Amazon EFS file system policy, you can specify an empty string for the Amazon EFS policy.</p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileSystemPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EfsFileSystemPolicy\"\n        },\n        {\n          \"description\": \"The JSON policy definition to apply to the Amazon EFS file system. For more information on the elements that make up a file system policy, see <a href=\\\"https://docs.aws.amazon.com/efs/latest/ug/access-control-overview.html#access-control-manage-access-intro-resource-policies\\\">Amazon EFS Resource-based policies</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-efs-file-system-configuration-schema.json
tags:
- Access Control
- Compliance
- IAM
- Policy Management
- Security
title: EfsFileSystemConfiguration
---
