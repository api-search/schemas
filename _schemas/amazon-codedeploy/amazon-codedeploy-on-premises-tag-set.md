---
description: Information about groups of on-premises instance tags.
layout: schema
name: OnPremisesTagSet
properties_list:
- description: ''
  name: onPremisesTagSetList
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-on-premises-tag-set-schema.json
slug: amazon-codedeploy-on-premises-tag-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-on-premises-tag-set-schema.json\",\n  \"title\": \"OnPremisesTagSet\",\n  \"description\": \"Information about groups of on-premises instance tags.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"onPremisesTagSetList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OnPremisesTagSetList\"\n        },\n        {\n          \"description\": \"A list that contains other lists of on-premises instance tag groups. For an instance to be included in the deployment group, it must be identified by all of the tag groups in the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-on-premises-tag-set-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: OnPremisesTagSet
---
