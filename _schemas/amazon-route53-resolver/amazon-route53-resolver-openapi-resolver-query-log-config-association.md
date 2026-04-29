---
description: In the response to an <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_AssociateResolverQueryLogConfig.html">AssociateResolverQueryLogConfig</a>, <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_DisassociateResolverQueryLogConfig.html">DisassociateResolverQueryLogConfig</a>, <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_GetResolverQueryLogConfigAssociation.html">GetResolverQueryLogConfigAssociation</a>, or <a href="https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_ListResolverQueryLogConfigAssociations.html">ListResolverQueryLogConfigAssociations</a>, request, a complex type that contains settings for a specified association between an Amazon VPC and a query logging configuration.
layout: schema
name: ResolverQueryLogConfigAssociation
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: ResolverQueryLogConfigId
  type: object
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Error
  type: object
- description: ''
  name: ErrorMessage
  type: object
- description: ''
  name: CreationTime
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-resolver-query-log-config-association-schema.json
slug: amazon-route53-resolver-openapi-resolver-query-log-config-association
source_filename: amazon-route53-resolver-openapi-resolver-query-log-config-association-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-resolver-query-log-config-association-schema.json\",\n  \"title\": \"ResolverQueryLogConfigAssociation\",\n  \"description\": \"In the response to an <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_AssociateResolverQueryLogConfig.html\\\">AssociateResolverQueryLogConfig</a>, <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_DisassociateResolverQueryLogConfig.html\\\">DisassociateResolverQueryLogConfig</a>, <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_GetResolverQueryLogConfigAssociation.html\\\">GetResolverQueryLogConfigAssociation</a>, or <a href=\\\"https://docs.aws.amazon.com/Route53/latest/APIReference/API_route53resolver_ListResolverQueryLogConfigAssociations.html\\\
  \">ListResolverQueryLogConfigAssociations</a>, request, a complex type that contains settings for a specified association between an Amazon VPC and a query logging configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the query logging association.\"\n        }\n      ]\n    },\n    \"ResolverQueryLogConfigId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the query logging configuration that a VPC is associated with.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon VPC that is associated with the query logging configuration.\"\n        }\n   \
  \   ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverQueryLogConfigAssociationStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the specified query logging association. Valid values include the following:</p> <ul> <li> <p> <code>CREATING</code>: Resolver is creating an association between an Amazon VPC and a query logging configuration.</p> </li> <li> <p> <code>CREATED</code>: The association between an Amazon VPC and a query logging configuration was successfully created. Resolver is logging queries that originate in the specified VPC.</p> </li> <li> <p> <code>DELETING</code>: Resolver is deleting this query logging association.</p> </li> <li> <p> <code>FAILED</code>: Resolver either couldn't create or couldn't delete the query logging association.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Error\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverQueryLogConfigAssociationError\"\
  \n        },\n        {\n          \"description\": \"<p>If the value of <code>Status</code> is <code>FAILED</code>, the value of <code>Error</code> indicates the cause:</p> <ul> <li> <p> <code>DESTINATION_NOT_FOUND</code>: The specified destination (for example, an Amazon S3 bucket) was deleted.</p> </li> <li> <p> <code>ACCESS_DENIED</code>: Permissions don't allow sending logs to the destination.</p> </li> </ul> <p>If the value of <code>Status</code> is a value other than <code>FAILED</code>, <code>Error</code> is null. </p>\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolverQueryLogConfigAssociationErrorMessage\"\n        },\n        {\n          \"description\": \"Contains additional information about the error. If the value or <code>Error</code> is null, the value of <code>ErrorMessage</code> also is null.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/Rfc3339TimeString\"\n        },\n        {\n          \"description\": \"The date and time that the VPC was associated with the query logging configuration, in Unix time format and Coordinated Universal Time (UTC).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-resolver-query-log-config-association-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ResolverQueryLogConfigAssociation
---
