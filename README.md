json-ld-is-not-just-json
========================

## Example 1

### Inputs

|                         | First Run                                       | Second Run                                      | Change?   |
|-------------------------|-------------------------------------------------|-------------------------------------------------|-----------|
| Input document          | [example1a.input](./examples/example1a.input)   | [example1b.input](./examples/example1b.input)   | No change |
| JSON-LD context URL     | `https://example.com/context1/`                 | `https://example.com/context1/`                 | No change |
| JSON-LD context content | [context1a.jsonld](./contexts/context1a.jsonld) | [context1b.jsonld](./contexts/context1b.jsonld) | Change    |

### Results

Data Integrity signature (Change):

**First Run:** [`QchIyphG9P3fGakQaHfzSx13u9QVr31x2JPSlJqtx125kFcYETidAJypjfkiRpYR8nfAa7JUZd8eljLMg-DZDg`](./examples/example1a.signed.jsonld)
**Second Run:** [`n8xH4Gj-mLG9VfdMqdUxDxsY0Tbrd_gcB9qmiPC7A2UMyNwu4DbriMCo4HzBKFPMN4T789DruH611Btn2PnIBg`](./examples/example1b.signed.jsonld)

JWS signature (No change):

**First Run:** [`Oemy6FevVedL8S-UhsIAYgYwnLCMvyUAxZYSRMN3jFYGdotOt2MG0Ucvdn7TuSkXrTks8r2F2LNVcbyHQj95Bw`](./examples/example1a.signed.jwt)
**Second Run:** [`Oemy6FevVedL8S-UhsIAYgYwnLCMvyUAxZYSRMN3jFYGdotOt2MG0Ucvdn7TuSkXrTks8r2F2LNVcbyHQj95Bw`](./examples/example1b.signed.jwt)

# Example 2

### Inputs

|                         | First Run                                       | Second Run                                      | Change?   |
|-------------------------|-------------------------------------------------|-------------------------------------------------|-----------|
| Input document          | [example2a.input](./examples/example2a.input)   | [example2b.input](./examples/example2b.input)   | Change    |
| JSON-LD context URL     | `https://example.com/context2a/`                | `https://example.com/context2b/`                | Change    |
| JSON-LD context content | [context2a.jsonld](./contexts/context2a.jsonld) | [context2b.jsonld](./contexts/context2b.jsonld) | Change    |

### Results

Data Integrity signature (No change):

**First Run:** [`QchIyphG9P3fGakQaHfzSx13u9QVr31x2JPSlJqtx125kFcYETidAJypjfkiRpYR8nfAa7JUZd8eljLMg-DZDg`](./examples/example2a.signed.jsonld)
**Second Run:** [`QchIyphG9P3fGakQaHfzSx13u9QVr31x2JPSlJqtx125kFcYETidAJypjfkiRpYR8nfAa7JUZd8eljLMg-DZDg`](./examples/example2b.signed.jsonld)

JWS signature (Change):

**First Run:** [`TOXXNqWdUt-s26Qi31ZfQxw96dH8pSyzx5ptlzIhTH3i09rJlnHZ2I1dcCQFHuwxvnEsU7qPqTfv6nYVuowaDw`](./examples/example2a.signed.jwt)
**Second Run:** [`ZGC7SmO0wcEjfbXR_08N8tgec3gGnl0njisJ98pl_Ry6zg9jd-AZFUpnnFwmvLD6o7OQyVGpIbHQGHZ0ixajCA`](./examples/example2b.signed.jwt)

# About

This work © 2023 by Markus Sabadello is licensed under CC BY 4.0.
