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

**First Run:** [`DuEpuEptX6NLcbCF21P7e_ObZHHzTmDEK5nfKwNzzp9G3rcfwdtEMrN0upbOfEA39QNxc-lk40uU7K6_cDALAQ`](./examples/example1a.signed.jsonld)
**Second Run:** [`ZadU_jcezNhO298exQN0rfuXQnL5WF91HnE_nJ-aGlMV2QWITZg-pc3cPm3dEPKYYnPKsFBgFshMXm3wDfRQAg`](./examples/example1b.signed.jsonld)

JWS signature (No change):

**First Run:** [`wTkLmRbZmU_bG8bchJbFMge9ojAjM9iEQW6fGVcQg7BmlCo0yo1nhEaDpVDBUeGZGbHOUw9WRCcUAOXiPWXCDg`](./examples/example1a.signed.jwt)
**Second Run:** [`wTkLmRbZmU_bG8bchJbFMge9ojAjM9iEQW6fGVcQg7BmlCo0yo1nhEaDpVDBUeGZGbHOUw9WRCcUAOXiPWXCDg`](./examples/example1b.signed.jwt)

# Example 2

### Inputs

|                         | First Run                                       | Second Run                                      | Change?   |
|-------------------------|-------------------------------------------------|-------------------------------------------------|-----------|
| Input document          | [example2a.input](./examples/example2a.input)   | [example2b.input](./examples/example2b.input)   | Change    |
| JSON-LD context URL     | `https://example.com/context2/`                 | `https://example.com/context2/`                 | No change |
| JSON-LD context content | [context2a.jsonld](./contexts/context2a.jsonld) | [context2b.jsonld](./contexts/context2b.jsonld) | Change    |

### Results

Data Integrity signature (No change):

**First Run:** [`DuEpuEptX6NLcbCF21P7e_ObZHHzTmDEK5nfKwNzzp9G3rcfwdtEMrN0upbOfEA39QNxc-lk40uU7K6_cDALAQ`](./examples/example2a.signed.jsonld)
**Second Run:** [`DuEpuEptX6NLcbCF21P7e_ObZHHzTmDEK5nfKwNzzp9G3rcfwdtEMrN0upbOfEA39QNxc-lk40uU7K6_cDALAQ`](./examples/example2b.signed.jsonld)

JWS signature (Change):

**First Run:** [`SDVXIIW48FjeVFLPU6uf3lDEJe_DUfV_iR031kTJHW4PQ_JNHxgDOjd3UW37GxXF_3iwkgkP_5q-AKVt39RyAA`](./examples/example2a.signed.jwt)
**Second Run:** [`7uyXiPMT4cBjPyT5DMvUg1NHKfEP-b5bYlakVar4afrZoRrsUYC8Ochu0zHGQOWbnQ09dPtEFHO7ixFxWZtaCQ`](./examples/example2b.signed.jwt)

# About

This work © 2023 by Markus Sabadello is licensed under CC BY 4.0.
