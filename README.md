# Referalli OpenAPI

The [Referalli API](https://referalli.com/docs) described as OpenAPI 3.1, plus a Postman collection.

| File | What it is |
| --- | --- |
| `openapi.json`, `openapi.yaml` | The full API: every operation, schema, error response and webhook event |
| `*.postman_collection.json` | A Postman collection of every operation, using `{{baseUrl}}` (default `https://referalli.com`) and a bearer `{{apiKey}}` |

The live spec for the API version you are calling is always served at `https://referalli.com/v1/openapi.json`. Versioned copies are attached to this repository's releases.

## Use it

- **Postman:** Import → the collection file, then set the `apiKey` collection variable to a test key (`rk_test_…`) from **Settings → API keys**.
- **Code generation:** point your generator at `openapi.yaml`. Official SDKs already exist for JavaScript, Python, Ruby, Go, PHP, Swift and Kotlin: see [github.com/Referalli](https://github.com/Referalli).

This repository is generated from the Referalli monorepo: see [CONTRIBUTING.md](https://github.com/Referalli/.github/blob/main/CONTRIBUTING.md).

MIT licensed.
