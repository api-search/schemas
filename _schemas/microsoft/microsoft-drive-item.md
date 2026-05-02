---
description: Represents a file, folder, or other item stored in a OneDrive or SharePoint document library. All file system objects in OneDrive and SharePoint are returned as driveItem resources.
layout: schema
name: Microsoft OneDrive DriveItem
properties_list:
- description: Unique identifier of the item within the drive
  name: id
  type: string
- description: The name of the item (filename and extension)
  name: name
  type: string
- description: Provides a user-visible description of the item
  name: description
  type:
  - string
  - 'null'
- description: Size of the item in bytes
  name: size
  type:
  - integer
  - 'null'
- description: URL that displays the resource in the browser
  name: webUrl
  type:
  - string
  - 'null'
- description: WebDAV compatible URL for the item
  name: webDavUrl
  type:
  - string
  - 'null'
- description: Date and time of item creation in UTC
  name: createdDateTime
  type: string
- description: Date and time the item was last modified in UTC
  name: lastModifiedDateTime
  type: string
- description: eTag for the entire item (metadata + content)
  name: eTag
  type:
  - string
  - 'null'
- description: eTag for the content of the item
  name: cTag
  type:
  - string
  - 'null'
- description: ''
  name: createdBy
  type: object
- description: ''
  name: lastModifiedBy
  type: object
- description: ''
  name: parentReference
  type: object
- description: File metadata, if the item is a file
  name: file
  type:
  - object
  - 'null'
- description: Folder metadata, if the item is a folder
  name: folder
  type:
  - object
  - 'null'
- description: Image metadata, if the item is an image
  name: image
  type:
  - object
  - 'null'
- description: Video metadata, if the item is a video
  name: video
  type:
  - object
  - 'null'
- description: Indicates the item has been shared with others
  name: shared
  type:
  - object
  - 'null'
- description: Information about the deleted state of the item
  name: deleted
  type:
  - object
  - 'null'
provider_name: Microsoft
provider_slug: microsoft
schema_file: json-schema/microsoft-drive-item-schema.json
slug: microsoft-drive-item
source_filename: microsoft-drive-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://learn.microsoft.com/en-us/graph/schemas/microsoft/drive-item.json\",\n  \"title\": \"Microsoft OneDrive DriveItem\",\n  \"description\": \"Represents a file, folder, or other item stored in a OneDrive or SharePoint document library. All file system objects in OneDrive and SharePoint are returned as driveItem resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the item within the drive\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the item (filename and extension)\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Provides a user-visible description of the item\"\n    },\n    \"size\": {\n      \"type\": [\"integer\", \"null\"],\n      \"format\": \"int64\",\n      \"\
  description\": \"Size of the item in bytes\",\n      \"readOnly\": true\n    },\n    \"webUrl\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URL that displays the resource in the browser\",\n      \"readOnly\": true\n    },\n    \"webDavUrl\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"WebDAV compatible URL for the item\",\n      \"readOnly\": true\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time of item creation in UTC\",\n      \"readOnly\": true\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the item was last modified in UTC\",\n      \"readOnly\": true\n    },\n    \"eTag\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"eTag for the entire item (metadata + content)\",\n\
  \      \"readOnly\": true\n    },\n    \"cTag\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"eTag for the content of the item\",\n      \"readOnly\": true\n    },\n    \"createdBy\": {\n      \"$ref\": \"#/$defs/IdentitySet\"\n    },\n    \"lastModifiedBy\": {\n      \"$ref\": \"#/$defs/IdentitySet\"\n    },\n    \"parentReference\": {\n      \"$ref\": \"#/$defs/ItemReference\"\n    },\n    \"file\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"File metadata, if the item is a file\",\n      \"properties\": {\n        \"mimeType\": {\n          \"type\": \"string\",\n          \"description\": \"The MIME type for the file\"\n        },\n        \"hashes\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"sha1Hash\": {\n              \"type\": [\"string\", \"null\"],\n              \"description\": \"SHA1 hash for the contents of the file\"\n            },\n            \"sha256Hash\": {\n              \"type\"\
  : [\"string\", \"null\"],\n              \"description\": \"SHA256 hash for the contents of the file\"\n            },\n            \"quickXorHash\": {\n              \"type\": [\"string\", \"null\"],\n              \"description\": \"A proprietary hash of the file for change detection\"\n            }\n          }\n        },\n        \"processingMetadata\": {\n          \"type\": [\"boolean\", \"null\"],\n          \"description\": \"Indicates whether the file is still being processed to extract metadata\"\n        }\n      }\n    },\n    \"folder\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Folder metadata, if the item is a folder\",\n      \"properties\": {\n        \"childCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of children contained immediately within this container\"\n        },\n        \"view\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"sortBy\": {\n              \"type\":\
  \ \"string\",\n              \"description\": \"The method by which the folder should be sorted\"\n            },\n            \"sortOrder\": {\n              \"type\": \"string\",\n              \"enum\": [\"ascending\", \"descending\"]\n            },\n            \"viewType\": {\n              \"type\": \"string\",\n              \"description\": \"The type of view that should be used\"\n            }\n          }\n        }\n      }\n    },\n    \"image\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Image metadata, if the item is an image\",\n      \"properties\": {\n        \"height\": {\n          \"type\": \"integer\"\n        },\n        \"width\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"video\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Video metadata, if the item is a video\",\n      \"properties\": {\n        \"duration\": {\n          \"type\": \"integer\",\n          \"description\": \"Duration\
  \ in milliseconds\"\n        },\n        \"height\": {\n          \"type\": \"integer\"\n        },\n        \"width\": {\n          \"type\": \"integer\"\n        },\n        \"bitrate\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"shared\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Indicates the item has been shared with others\",\n      \"properties\": {\n        \"owner\": {\n          \"$ref\": \"#/$defs/IdentitySet\"\n        },\n        \"scope\": {\n          \"type\": \"string\",\n          \"enum\": [\"anonymous\", \"organization\", \"users\"],\n          \"description\": \"The scope of how the item is shared\"\n        },\n        \"sharedDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"sharedBy\": {\n          \"$ref\": \"#/$defs/IdentitySet\"\n        }\n      }\n    },\n    \"deleted\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Information\
  \ about the deleted state of the item\",\n      \"properties\": {\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"Represents the state of the deleted item\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"IdentitySet\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"A keyed collection of identity resources\",\n      \"properties\": {\n        \"user\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"displayName\": {\n              \"type\": \"string\"\n            },\n            \"id\": {\n              \"type\": \"string\"\n            },\n            \"email\": {\n              \"type\": [\"string\", \"null\"]\n            }\n          }\n        },\n        \"application\": {\n          \"type\": [\"object\", \"null\"],\n          \"properties\": {\n            \"displayName\": {\n              \"type\": \"string\"\n            },\n            \"id\": {\n              \"type\": \"string\"\
  \n            }\n          }\n        },\n        \"device\": {\n          \"type\": [\"object\", \"null\"],\n          \"properties\": {\n            \"displayName\": {\n              \"type\": \"string\"\n            },\n            \"id\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"ItemReference\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Provides information necessary to address a driveItem\",\n      \"properties\": {\n        \"driveId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the drive instance\"\n        },\n        \"driveType\": {\n          \"type\": \"string\",\n          \"enum\": [\"personal\", \"business\", \"documentLibrary\"]\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the item in the drive\"\n        },\n        \"name\": {\n          \"type\": [\"string\", \"null\"],\n\
  \          \"description\": \"The name of the item being referenced\"\n        },\n        \"path\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Path to navigate to the item\"\n        },\n        \"shareId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"A unique identifier for a shared resource\"\n        },\n        \"siteId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"For SharePoint, the identifier of the site\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/json-schema/microsoft-drive-item-schema.json
tags: []
title: Microsoft OneDrive DriveItem
---
