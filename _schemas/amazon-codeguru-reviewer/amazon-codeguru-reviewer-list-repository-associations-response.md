---
description: ListRepositoryAssociationsResponse schema from Amazon CodeGuru Reviewer
layout: schema
name: ListRepositoryAssociationsResponse
properties_list:
- description: ''
  name: RepositoryAssociationSummaries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-list-repository-associations-response-schema.json
slug: amazon-codeguru-reviewer-list-repository-associations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-list-repository-associations-response-schema.json\",\n  \"title\": \"ListRepositoryAssociationsResponse\",\n  \"description\": \"ListRepositoryAssociationsResponse schema from Amazon CodeGuru Reviewer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RepositoryAssociationSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryAssociationSummaries\"\n        },\n        {\n          \"description\": \"A list of repository associations that meet the criteria of the request.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> value to include in a future <code>ListRecommendations</code>\
  \ request. When the results of a <code>ListRecommendations</code> request exceed <code>maxResults</code>, this value can be used to retrieve the next page of results. This value is <code>null</code> when there are no more results to return. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-list-repository-associations-response-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: ListRepositoryAssociationsResponse
---
