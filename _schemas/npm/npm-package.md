---
description: A full npm package document (packument) representing all metadata for a package in the npm registry, including every published version, distribution tags, maintainers, and repository information.
layout: schema
name: npm Package Document
properties_list:
- description: The package name, used as the CouchDB document identifier.
  name: _id
  type: string
- description: The CouchDB document revision identifier.
  name: _rev
  type: string
- description: 'The name of the package. Must follow npm naming rules: lowercase, no spaces, may contain hyphens and dots.'
  name: name
  type: string
- description: A short description of the package, used in search results.
  name: description
  type: string
- description: A mapping of distribution tag names to version strings. The 'latest' tag is always present and points to the most recently published non-prerelease version.
  name: dist-tags
  type: object
- description: A mapping of semver version strings to version-specific metadata objects.
  name: versions
  type: object
- description: A mapping of version strings to ISO 8601 timestamps indicating when each version was published. Includes special keys 'created' and 'modified'.
  name: time
  type: object
- description: List of current package maintainers with publish access.
  name: maintainers
  type: array
- description: ''
  name: author
  type: object
- description: ''
  name: repository
  type: object
- description: The README content for the package, typically from the latest version.
  name: readme
  type: string
- description: The filename of the README file.
  name: readmeFilename
  type: string
- description: The URL of the package homepage.
  name: homepage
  type: string
- description: Keywords associated with the package for search discovery.
  name: keywords
  type: array
- description: Issue tracker information for reporting bugs.
  name: bugs
  type: object
- description: The SPDX license identifier for the package.
  name: license
  type: string
- description: A mapping of npm usernames to boolean values indicating users who have starred this package.
  name: users
  type: object
provider_name: npm
provider_slug: npm
schema_file: json-schema/npm-package-schema.json
slug: npm-package
source_filename: npm-package-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://npmjs.com/schemas/npm/package.json\",\n  \"title\": \"npm Package Document\",\n  \"description\": \"A full npm package document (packument) representing all metadata for a package in the npm registry, including every published version, distribution tags, maintainers, and repository information.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"dist-tags\", \"versions\"],\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"The package name, used as the CouchDB document identifier.\"\n    },\n    \"_rev\": {\n      \"type\": \"string\",\n      \"description\": \"The CouchDB document revision identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the package. Must follow npm naming rules: lowercase, no spaces, may contain hyphens and dots.\",\n      \"pattern\": \"^(@[a-z0-9-~][a-z0-9-._~]*/)?[a-z0-9-~][a-z0-9-._~]*$\"\
  ,\n      \"maxLength\": 214\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A short description of the package, used in search results.\"\n    },\n    \"dist-tags\": {\n      \"type\": \"object\",\n      \"description\": \"A mapping of distribution tag names to version strings. The 'latest' tag is always present and points to the most recently published non-prerelease version.\",\n      \"required\": [\"latest\"],\n      \"properties\": {\n        \"latest\": {\n          \"type\": \"string\",\n          \"description\": \"The latest stable version of the package.\"\n        }\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"versions\": {\n      \"type\": \"object\",\n      \"description\": \"A mapping of semver version strings to version-specific metadata objects.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/PackageVersion\"\n      }\n    },\n    \"time\": {\n      \"type\":\
  \ \"object\",\n      \"description\": \"A mapping of version strings to ISO 8601 timestamps indicating when each version was published. Includes special keys 'created' and 'modified'.\",\n      \"properties\": {\n        \"created\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the package was first created in the registry.\"\n        },\n        \"modified\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the package was last modified.\"\n        }\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\",\n        \"format\": \"date-time\"\n      }\n    },\n    \"maintainers\": {\n      \"type\": \"array\",\n      \"description\": \"List of current package maintainers with publish access.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Person\"\n      }\n    },\n    \"author\": {\n      \"$ref\": \"#/$defs/Person\"\n    },\n    \"repository\"\
  : {\n      \"$ref\": \"#/$defs/Repository\"\n    },\n    \"readme\": {\n      \"type\": \"string\",\n      \"description\": \"The README content for the package, typically from the latest version.\"\n    },\n    \"readmeFilename\": {\n      \"type\": \"string\",\n      \"description\": \"The filename of the README file.\"\n    },\n    \"homepage\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the package homepage.\"\n    },\n    \"keywords\": {\n      \"type\": \"array\",\n      \"description\": \"Keywords associated with the package for search discovery.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"bugs\": {\n      \"type\": \"object\",\n      \"description\": \"Issue tracker information for reporting bugs.\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the issue tracker.\"\n        },\n        \"email\"\
  : {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Email address for bug reports.\"\n        }\n      }\n    },\n    \"license\": {\n      \"type\": \"string\",\n      \"description\": \"The SPDX license identifier for the package.\"\n    },\n    \"users\": {\n      \"type\": \"object\",\n      \"description\": \"A mapping of npm usernames to boolean values indicating users who have starred this package.\",\n      \"additionalProperties\": {\n        \"type\": \"boolean\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"PackageVersion\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata for a specific published version of a package.\",\n      \"required\": [\"name\", \"version\", \"dist\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the package.\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"The\
  \ semver version string.\",\n          \"pattern\": \"^[0-9]+\\\\.[0-9]+\\\\.[0-9]+(-[a-zA-Z0-9.]+)?(\\\\+[a-zA-Z0-9.]+)?$\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A short description of the package.\"\n        },\n        \"main\": {\n          \"type\": \"string\",\n          \"description\": \"The entry point module for the package.\"\n        },\n        \"module\": {\n          \"type\": \"string\",\n          \"description\": \"The ES module entry point.\"\n        },\n        \"types\": {\n          \"type\": \"string\",\n          \"description\": \"The TypeScript type declarations entry point.\"\n        },\n        \"exports\": {\n          \"description\": \"Package exports map for conditional module resolution.\",\n          \"oneOf\": [\n            { \"type\": \"string\" },\n            { \"type\": \"object\" }\n          ]\n        },\n        \"scripts\": {\n          \"type\": \"object\",\n          \"description\"\
  : \"A mapping of script names to shell commands.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"dependencies\": {\n          \"type\": \"object\",\n          \"description\": \"Runtime dependencies as a mapping of package names to semver ranges.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"devDependencies\": {\n          \"type\": \"object\",\n          \"description\": \"Development dependencies as a mapping of package names to semver ranges.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"peerDependencies\": {\n          \"type\": \"object\",\n          \"description\": \"Peer dependencies as a mapping of package names to semver ranges.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"optionalDependencies\": {\n          \"type\"\
  : \"object\",\n          \"description\": \"Optional dependencies as a mapping of package names to semver ranges.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"engines\": {\n          \"type\": \"object\",\n          \"description\": \"Runtime environment requirements as a mapping of engine names to semver ranges.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"bin\": {\n          \"description\": \"Executable files to install into PATH.\",\n          \"oneOf\": [\n            { \"type\": \"string\" },\n            {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"type\": \"string\"\n              }\n            }\n          ]\n        },\n        \"author\": {\n          \"$ref\": \"#/$defs/Person\"\n        },\n        \"maintainers\": {\n          \"type\": \"array\",\n          \"description\": \"List of\
  \ maintainers for this version.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Person\"\n          }\n        },\n        \"contributors\": {\n          \"type\": \"array\",\n          \"description\": \"List of contributors.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Person\"\n          }\n        },\n        \"repository\": {\n          \"$ref\": \"#/$defs/Repository\"\n        },\n        \"license\": {\n          \"type\": \"string\",\n          \"description\": \"The SPDX license identifier.\"\n        },\n        \"keywords\": {\n          \"type\": \"array\",\n          \"description\": \"Keywords associated with this version.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"dist\": {\n          \"$ref\": \"#/$defs/Distribution\"\n        },\n        \"deprecated\": {\n          \"type\": \"string\",\n          \"description\": \"Deprecation message if this version is deprecated.\"\n        },\n      \
  \  \"_npmVersion\": {\n          \"type\": \"string\",\n          \"description\": \"The version of npm used to publish this package version.\"\n        },\n        \"_nodeVersion\": {\n          \"type\": \"string\",\n          \"description\": \"The version of Node.js used to publish this package version.\"\n        },\n        \"_npmUser\": {\n          \"$ref\": \"#/$defs/Person\"\n        },\n        \"_hasShrinkwrap\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this version includes a shrinkwrap file.\"\n        }\n      }\n    },\n    \"Person\": {\n      \"type\": \"object\",\n      \"description\": \"A person object representing a user, author, maintainer, or contributor.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the person.\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The\
  \ email address of the person.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The personal URL or website of the person.\"\n        }\n      }\n    },\n    \"Repository\": {\n      \"type\": \"object\",\n      \"description\": \"Source code repository information.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The version control system type, typically 'git'.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"description\": \"The URL of the source code repository.\"\n        },\n        \"directory\": {\n          \"type\": \"string\",\n          \"description\": \"The directory within the repository where the package lives, for monorepos.\"\n        }\n      }\n    },\n    \"Distribution\": {\n      \"type\": \"object\",\n      \"description\": \"Distribution metadata for a published version, including integrity\
  \ hashes and tarball location.\",\n      \"required\": [\"shasum\", \"tarball\"],\n      \"properties\": {\n        \"shasum\": {\n          \"type\": \"string\",\n          \"description\": \"The SHA-1 checksum of the tarball.\",\n          \"pattern\": \"^[a-f0-9]{40}$\"\n        },\n        \"tarball\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL where the tarball can be downloaded.\"\n        },\n        \"integrity\": {\n          \"type\": \"string\",\n          \"description\": \"The Subresource Integrity (SRI) hash of the tarball, typically using SHA-512.\",\n          \"pattern\": \"^sha512-\"\n        },\n        \"fileCount\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of files in the tarball.\",\n          \"minimum\": 1\n        },\n        \"unpackedSize\": {\n          \"type\": \"integer\",\n          \"description\": \"The total unpacked size of the tarball in bytes.\",\n   \
  \       \"minimum\": 0\n        },\n        \"npm-signature\": {\n          \"type\": \"string\",\n          \"description\": \"The npm registry signature for the package version.\"\n        },\n        \"signatures\": {\n          \"type\": \"array\",\n          \"description\": \"Cryptographic signatures for the package version.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"required\": [\"keyid\", \"sig\"],\n            \"properties\": {\n              \"keyid\": {\n                \"type\": \"string\",\n                \"description\": \"The identifier of the signing key.\"\n              },\n              \"sig\": {\n                \"type\": \"string\",\n                \"description\": \"The signature value.\"\n              }\n            }\n          }\n        },\n        \"attestations\": {\n          \"type\": \"object\",\n          \"description\": \"Sigstore provenance attestations for the package version.\",\n          \"properties\": {\n  \
  \          \"url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"URL to fetch the full attestation bundle.\"\n            },\n            \"provenance\": {\n              \"type\": \"object\",\n              \"description\": \"Provenance attestation summary.\",\n              \"properties\": {\n                \"predicateType\": {\n                  \"type\": \"string\",\n                  \"format\": \"uri\",\n                  \"description\": \"The SLSA predicate type URI.\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/npm/refs/heads/main/json-schema/npm-package-schema.json
tags:
- Packages
- JavaScript
- Node.js
- Package Management
- Registry
- Security
title: npm Package Document
---
