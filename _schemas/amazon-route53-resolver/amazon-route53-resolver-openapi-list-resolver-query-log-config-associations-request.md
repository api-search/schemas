---
description: ListResolverQueryLogConfigAssociationsRequest schema from openapi
layout: schema
name: ListResolverQueryLogConfigAssociationsRequest
properties_list:
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Filters
  type: object
- description: ''
  name: SortBy
  type: object
- description: ''
  name: SortOrder
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-list-resolver-query-log-config-associations-request-schema.json
slug: amazon-route53-resolver-openapi-list-resolver-query-log-config-associations-request
source_filename: amazon-route53-resolver-openapi-list-resolver-query-log-config-associations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-query-log-config-associations-request-schema.json\",\n  \"title\": \"ListResolverQueryLogConfigAssociationsRequest\",\n  \"description\": \"ListResolverQueryLogConfigAssociationsRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of query logging associations that you want to return in the response to a <code>ListResolverQueryLogConfigAssociations</code> request. If you don't specify a value for <code>MaxResults</code>, Resolver returns up to 100 query logging associations. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"<p>For the first <code>ListResolverQueryLogConfigAssociations</code> request, omit this value.</p> <p>If there are more than <code>MaxResults</code> query logging associations that match the values that you specify for <code>Filters</code>, you can submit another <code>ListResolverQueryLogConfigAssociations</code> request to get the next group of associations. In the next request, specify the value of <code>NextToken</code> from the previous response. </p>\"\n        }\n      ]\n    },\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Filters\"\n        },\n        {\n          \"description\": \"<p>An optional specification to return a subset of query logging associations.</p> <note> <p>If you submit a second or subsequent <code>ListResolverQueryLogConfigAssociations</code> request and specify the <code>NextToken</code> parameter,\
  \ you must use the same values for <code>Filters</code>, if any, as in the previous request.</p> </note>\"\n        }\n      ]\n    },\n    \"SortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortByKey\"\n        },\n        {\n          \"description\": \"<p>The element that you want Resolver to sort query logging associations by. </p> <note> <p>If you submit a second or subsequent <code>ListResolverQueryLogConfigAssociations</code> request and specify the <code>NextToken</code> parameter, you must use the same value for <code>SortBy</code>, if any, as in the previous request.</p> </note> <p>Valid values include the following elements:</p> <ul> <li> <p> <code>CreationTime</code>: The ID of the query logging association.</p> </li> <li> <p> <code>Error</code>: If the value of <code>Status</code> is <code>FAILED</code>, the value of <code>Error</code> indicates the cause: </p> <ul> <li> <p> <code>DESTINATION_NOT_FOUND</code>: The specified destination\
  \ (for example, an Amazon S3 bucket) was deleted.</p> </li> <li> <p> <code>ACCESS_DENIED</code>: Permissions don't allow sending logs to the destination.</p> </li> </ul> <p>If <code>Status</code> is a value other than <code>FAILED</code>, <code>ERROR</code> is null.</p> </li> <li> <p> <code>Id</code>: The ID of the query logging association</p> </li> <li> <p> <code>ResolverQueryLogConfigId</code>: The ID of the query logging configuration</p> </li> <li> <p> <code>ResourceId</code>: The ID of the VPC that is associated with the query logging configuration</p> </li> <li> <p> <code>Status</code>: The current status of the configuration. Valid values include the following:</p> <ul> <li> <p> <code>CREATING</code>: Resolver is creating an association between an Amazon VPC and a query logging configuration.</p> </li> <li> <p> <code>CREATED</code>: The association between an Amazon VPC and a query logging configuration was successfully created. Resolver is logging queries that originate in the\
  \ specified VPC.</p> </li> <li> <p> <code>DELETING</code>: Resolver is deleting this query logging association.</p> </li> <li> <p> <code>FAILED</code>: Resolver either couldn't create or couldn't delete the query logging association. Here are two common causes:</p> <ul> <li> <p>The specified destination (for example, an Amazon S3 bucket) was deleted.</p> </li> <li> <p>Permissions don't allow sending logs to the destination.</p> </li> </ul> </li> </ul> </li> </ul>\"\n        }\n      ]\n    },\n    \"SortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\n        },\n        {\n          \"description\": \"<p>If you specified a value for <code>SortBy</code>, the order that you want query logging associations to be listed in, <code>ASCENDING</code> or <code>DESCENDING</code>.</p> <note> <p>If you submit a second or subsequent <code>ListResolverQueryLogConfigAssociations</code> request and specify the <code>NextToken</code> parameter, you must\
  \ use the same value for <code>SortOrder</code>, if any, as in the previous request.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-resolver-query-log-config-associations-request-schema.json
tags:
- DNS
- Hybrid Cloud
- Networking
title: ListResolverQueryLogConfigAssociationsRequest
---
