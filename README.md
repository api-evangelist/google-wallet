# Google Wallet API

The Google Wallet API enables developers to create and manage digital passes including event tickets, boarding passes, loyalty cards, gift cards, offers, transit passes, and generic passes. It provides REST endpoints for creating pass classes (templates) and pass objects (instances), managing issuers, handling media uploads, and generating JWT tokens for save-to-wallet functionality on Android devices and the web.

## Artifacts

- **APIs.yml** - Machine-readable API metadata following the APIs.json specification.
- **OpenAPI** (`openapi/openapi.yml`) - OpenAPI 3.1.0 specification describing the Wallet API endpoints for pass management, issuers, and JWTs.
- **JSON Schema** (`json-schema/google-wallet.json`) - JSON Schema (draft 2020-12) defining pass class and object definitions.
- **JSON-LD** (`json-ld/google-wallet.jsonld`) - JSON-LD context mapping Wallet API terms to schema.org and API-specific vocabularies.

## Key Endpoints

| Method | Path | Description |
|--------|------|-------------|
| POST | `/genericClass` | Create a generic pass class |
| GET | `/genericClass` | List generic pass classes |
| GET | `/genericClass/{resourceId}` | Get a generic pass class |
| POST | `/genericObject` | Create a generic pass object |
| GET | `/genericObject/{resourceId}` | Get a generic pass object |
| POST | `/eventTicketClass` | Create an event ticket class |
| POST | `/loyaltyClass` | Create a loyalty card class |
| GET | `/issuer` | List issuers |
| POST | `/jwt` | Create a save-to-wallet JWT |

## Resources

- [API Reference](https://developers.google.com/wallet/reference/rest)
- [Getting Started](https://developers.google.com/wallet/generic/getting-started/onboarding-guide)
- [REST API Samples](https://github.com/google-wallet/rest-samples)

## Maintainer

Kin Lane - kin@apievangelist.com
