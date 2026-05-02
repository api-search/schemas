---
description: Represents the base type for Microsoft Entra ID directory objects. Every identity-related object in Microsoft Entra ID, including users, groups, devices, service principals, applications, organizational contacts, and directory roles, inherits from directoryObject. It provides a common set of properties and navigation relationships that all directory entities share, enabling uniform operations such as listing, getting, checking membership, and querying deletions across diverse object types.
layout: schema
name: Microsoft Graph Directory Object
properties_list:
- description: The unique identifier for the directory object. A GUID assigned by Microsoft Entra ID. Read-only.
  name: id
  type: string
- description: The OData entity type of the directory object, indicating whether it is a user, group, device, service principal, application, or other entity type.
  name: '@odata.type'
  type: string
- description: Date and time when this object was deleted. Always null when the object has not been deleted. Read-only.
  name: deletedDateTime
  type:
  - string
  - 'null'
provider_name: Microsoft Graph
provider_slug: microsoft-graph
schema_file: json-schema/microsoft-graph-directory-object-schema.json
slug: microsoft-graph-directory-object
source_filename: microsoft-graph-directory-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.api.gov/microsoft-graph/directory-object\",\n  \"title\": \"Microsoft Graph Directory Object\",\n  \"description\": \"Represents the base type for Microsoft Entra ID directory objects. Every identity-related object in Microsoft Entra ID, including users, groups, devices, service principals, applications, organizational contacts, and directory roles, inherits from directoryObject. It provides a common set of properties and navigation relationships that all directory entities share, enabling uniform operations such as listing, getting, checking membership, and querying deletions across diverse object types.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the directory object. A GUID assigned by Microsoft Entra ID. Read-only.\",\n      \"readOnly\": true,\n      \"examples\": [\n      \
  \  \"87d349ed-44d7-43e1-9a83-5f2406dee5bd\"\n      ]\n    },\n    \"@odata.type\": {\n      \"type\": \"string\",\n      \"description\": \"The OData entity type of the directory object, indicating whether it is a user, group, device, service principal, application, or other entity type.\",\n      \"examples\": [\n        \"#microsoft.graph.user\",\n        \"#microsoft.graph.group\",\n        \"#microsoft.graph.device\",\n        \"#microsoft.graph.servicePrincipal\",\n        \"#microsoft.graph.application\",\n        \"#microsoft.graph.orgContact\",\n        \"#microsoft.graph.directoryRole\"\n      ]\n    },\n    \"deletedDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when this object was deleted. Always null when the object has not been deleted. Read-only.\",\n      \"readOnly\": true\n    }\n  },\n  \"$defs\": {\n    \"DirectoryObjectCollection\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"A collection of directory objects returned from a list operation, with optional OData pagination.\",\n      \"properties\": {\n        \"@odata.context\": {\n          \"type\": \"string\",\n          \"description\": \"The OData context URL for the collection.\"\n        },\n        \"@odata.nextLink\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to retrieve the next page of results, if the results are paged.\"\n        },\n        \"@odata.count\": {\n          \"type\": \"integer\",\n          \"description\": \"The total count of objects matching the request, if requested with $count=true.\",\n          \"minimum\": 0\n        },\n        \"value\": {\n          \"type\": \"array\",\n          \"description\": \"The list of directory objects in this page of results.\",\n          \"items\": {\n            \"$ref\": \"#\"\n          }\n        }\n      },\n      \"required\": [\n        \"value\"\n      ]\n    },\n    \"CheckMemberGroupsRequest\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Request body for the checkMemberGroups action, which checks for membership in a specified list of group IDs.\",\n      \"required\": [\n        \"groupIds\"\n      ],\n      \"properties\": {\n        \"groupIds\": {\n          \"type\": \"array\",\n          \"description\": \"A collection of group IDs to check membership against.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"maxItems\": 20\n        }\n      }\n    },\n    \"GetMemberObjectsRequest\": {\n      \"type\": \"object\",\n      \"description\": \"Request body for the getMemberObjects action, which returns all the IDs of the groups, administrative units, and directory roles that the object is a member of.\",\n      \"required\": [\n        \"securityEnabledOnly\"\n      ],\n      \"properties\": {\n        \"securityEnabledOnly\": {\n          \"type\": \"boolean\",\n          \"description\"\
  : \"True to specify that only security groups that the entity is a member of should be returned; false to specify that all groups and directory roles should be returned.\"\n        }\n      }\n    },\n    \"GetByIdsRequest\": {\n      \"type\": \"object\",\n      \"description\": \"Request body for the getByIds action, which returns the directory objects specified in a list of IDs. Supports returning up to 1000 objects per request.\",\n      \"required\": [\n        \"ids\"\n      ],\n      \"properties\": {\n        \"ids\": {\n          \"type\": \"array\",\n          \"description\": \"A collection of IDs for which to return objects.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"maxItems\": 1000\n        },\n        \"types\": {\n          \"type\": \"array\",\n          \"description\": \"A collection of resource types that specifies the set of resource collections to search. If not specified, the default\
  \ is directoryObject, which contains all of the resource types defined in the directory.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"examples\": [\n            [\"user\", \"group\"]\n          ]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-graph/refs/heads/main/json-schema/microsoft-graph-directory-object-schema.json
tags:
- Azure AD
- Collaboration
- Contacts
- Documents
- Email
- Graph
- Identity
- Microsoft
- Office 365
- Presentations
- Productivity
- Spreadsheets
- T1
- Tasks
title: Microsoft Graph Directory Object
---
