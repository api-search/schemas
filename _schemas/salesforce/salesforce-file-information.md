---
description: ''
layout: schema
name: FileInformation
properties_list:
- description: ''
  name: checksum
  type: string
- description: ''
  name: contentHubRepository
  type: '[''string'', ''null'']'
- description: ''
  name: contentModifiedDate
  type: string
- description: ''
  name: contentSize
  type: integer
- description: ''
  name: contentUrl
  type: '[''string'', ''null'']'
- description: ''
  name: createdDate
  type: string
- description: ''
  name: description
  type: '[''string'', ''null'']'
- description: ''
  name: downloadUrl
  type: string
- description: ''
  name: externalDocumentUrl
  type: '[''string'', ''null'']'
- description: ''
  name: externalFilePermissionInformation
  type: '[''string'', ''null'']'
- description: ''
  name: fileAsset
  type: '[''string'', ''null'']'
- description: ''
  name: fileExtension
  type: string
- description: ''
  name: fileType
  type: string
- description: ''
  name: flashRenditionStatus
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: isFileAsset
  type: boolean
- description: ''
  name: isInMyFileSync
  type: boolean
- description: ''
  name: isMajorVersion
  type: boolean
- description: ''
  name: mimeType
  type: string
- description: ''
  name: moderationFlags
  type: '[''string'', ''null'']'
- description: ''
  name: modifiedDate
  type: string
- description: ''
  name: motif
  type: object
- description: ''
  name: mySubscription
  type: '[''string'', ''null'']'
- description: ''
  name: name
  type: string
- description: ''
  name: origin
  type: string
- description: ''
  name: owner
  type: object
- description: ''
  name: pageCount
  type: integer
- description: ''
  name: parentFolder
  type: '[''string'', ''null'']'
- description: ''
  name: pdfRenditionStatus
  type: string
- description: ''
  name: publishStatus
  type: string
- description: ''
  name: renditionUrl
  type: string
- description: ''
  name: renditionUrl240By180
  type: string
- description: ''
  name: renditionUrl720By480
  type: string
- description: ''
  name: repositoryFileId
  type: '[''string'', ''null'']'
- description: ''
  name: repositoryFileUrl
  type: '[''string'', ''null'']'
- description: ''
  name: sharingOption
  type: string
- description: ''
  name: sharingPrivacy
  type: string
- description: ''
  name: sharingRole
  type: string
- description: ''
  name: systemModstamp
  type: string
- description: ''
  name: textPreview
  type: '[''string'', ''null'']'
- description: ''
  name: thumb120By90RenditionStatus
  type: string
- description: ''
  name: thumb240By180RenditionStatus
  type: string
- description: ''
  name: thumb720By480RenditionStatus
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: topics
  type: object
- description: ''
  name: type
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: versionNumber
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-file-information-schema.json
slug: salesforce-file-information
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"checksum\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"contentHubRepository\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"contentModifiedDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"contentSize\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"contentUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"description\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"A sample description.\"\n    },\n    \"downloadUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"externalDocumentUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\"\
  : \"https://www.example.com\"\n    },\n    \"externalFilePermissionInformation\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"fileAsset\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"fileExtension\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"fileType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"flashRenditionStatus\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"isFileAsset\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"isInMyFileSync\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"isMajorVersion\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"mimeType\": {\n      \"type\": \"string\",\n      \"example\"\
  : \"example_value\"\n    },\n    \"moderationFlags\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"motif\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"color\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"largeIconUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"mediumIconUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"smallIconUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"svgIconUrl\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"color\",\n       \
  \ \"largeIconUrl\",\n        \"mediumIconUrl\",\n        \"smallIconUrl\",\n        \"svgIconUrl\"\n      ]\n    },\n    \"mySubscription\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"origin\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"owner\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"additionalLabel\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"communityNickname\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"companyName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"firstName\": {\n  \
  \        \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"isActive\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"isInThisCommunity\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"motif\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"color\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"largeIconUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"mediumIconUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n\
  \            \"smallIconUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"svgIconUrl\": {\n              \"type\": \"['string', 'null']\",\n              \"example\": \"https://www.example.com\"\n            }\n          },\n          \"required\": [\n            \"color\",\n            \"largeIconUrl\",\n            \"mediumIconUrl\",\n            \"smallIconUrl\",\n            \"svgIconUrl\"\n          ]\n        },\n        \"mySubscription\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        },\n        \"outOfOffice\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"message\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n\
  \            \"message\"\n          ]\n        },\n        \"photo\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"fullEmailPhotoUrl\": {\n              \"type\": \"string\",\n              \"example\": \"user@example.com\"\n            },\n            \"largePhotoUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"mediumPhotoUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"photoVersionId\": {\n              \"type\": \"string\",\n              \"example\": \"500123\"\n            },\n            \"smallPhotoUrl\": {\n              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            },\n            \"standardEmailPhotoUrl\": {\n              \"type\": \"string\",\n              \"example\": \"user@example.com\"\n            },\n            \"url\": {\n\
  \              \"type\": \"string\",\n              \"example\": \"https://www.example.com\"\n            }\n          },\n          \"required\": [\n            \"fullEmailPhotoUrl\",\n            \"largePhotoUrl\",\n            \"mediumPhotoUrl\",\n            \"photoVersionId\",\n            \"smallPhotoUrl\",\n            \"standardEmailPhotoUrl\",\n            \"url\"\n          ]\n        },\n        \"reputation\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"title\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"Example Title\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"userType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n    \
  \  \"required\": [\n        \"additionalLabel\",\n        \"communityNickname\",\n        \"companyName\",\n        \"displayName\",\n        \"firstName\",\n        \"id\",\n        \"isActive\",\n        \"isInThisCommunity\",\n        \"lastName\",\n        \"motif\",\n        \"mySubscription\",\n        \"name\",\n        \"outOfOffice\",\n        \"photo\",\n        \"reputation\",\n        \"title\",\n        \"type\",\n        \"url\",\n        \"userType\"\n      ]\n    },\n    \"pageCount\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"parentFolder\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"pdfRenditionStatus\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"publishStatus\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"renditionUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n\
  \    \"renditionUrl240By180\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"renditionUrl720By480\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"repositoryFileId\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"500123\"\n    },\n    \"repositoryFileUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"sharingOption\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"sharingPrivacy\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"sharingRole\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"systemModstamp\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"textPreview\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"thumb120By90RenditionStatus\"\
  : {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"thumb240By180RenditionStatus\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"thumb720By480RenditionStatus\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"topics\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"currentPageUrl\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"nextPageUrl\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"topics\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"required\": [\n        \"currentPageUrl\"\
  ,\n        \"nextPageUrl\",\n        \"topics\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"versionNumber\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"checksum\",\n    \"contentHubRepository\",\n    \"contentModifiedDate\",\n    \"contentSize\",\n    \"contentUrl\",\n    \"createdDate\",\n    \"description\",\n    \"downloadUrl\",\n    \"externalDocumentUrl\",\n    \"externalFilePermissionInformation\",\n    \"fileAsset\",\n    \"fileExtension\",\n    \"fileType\",\n    \"flashRenditionStatus\",\n    \"id\",\n    \"isFileAsset\",\n    \"isInMyFileSync\",\n    \"isMajorVersion\",\n    \"mimeType\",\n    \"moderationFlags\",\n    \"modifiedDate\",\n    \"motif\",\n    \"mySubscription\",\n    \"name\",\n    \"origin\",\n    \"owner\",\n    \"pageCount\"\
  ,\n    \"parentFolder\",\n    \"pdfRenditionStatus\",\n    \"publishStatus\",\n    \"renditionUrl\",\n    \"renditionUrl240By180\",\n    \"renditionUrl720By480\",\n    \"repositoryFileId\",\n    \"repositoryFileUrl\",\n    \"sharingOption\",\n    \"sharingPrivacy\",\n    \"sharingRole\",\n    \"systemModstamp\",\n    \"textPreview\",\n    \"thumb120By90RenditionStatus\",\n    \"thumb240By180RenditionStatus\",\n    \"thumb720By480RenditionStatus\",\n    \"title\",\n    \"topics\",\n    \"type\",\n    \"url\",\n    \"versionNumber\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FileInformation\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-file-information-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: FileInformation
---
