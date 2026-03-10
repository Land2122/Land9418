# Land9418

> **Python source-level code protection.** Rename identifiers, encrypt strings, flatten control flow, inject dead code, embed license validators, and add forensic watermarks — all producing valid, immediately runnable Python.

[![Python 3.9+](https://img.shields.io/badge/python-3.9%2B-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Tests](https://img.shields.io/badge/tests-119%20passing-brightgreen.svg)]()
[![Version](https://img.shields.io/badge/version-4.0.0-blue.svg)]()

---

## What Land does

Land9418 is an AST-level source-code protection toolkit for Python. It transforms Python source through up to five layered obfuscation passes, then optionally embeds a self-contained license validator and a forensic watermark. The output is syntactically valid Python.

```
Source .py  →  NameCollector  →  ASTTransformer  →  ControlFlowFlattener  →  DeadCodeInjector  →  Protected .py
```

**What it is:** A tool for protecting proprietary Python code you distribute to customers, embed in products, or deploy to untrusted environments.

---

## Edition comparison

| Feature | Demo | Full |
|---------|:----:|:----:|
| Single-file protection | ✓ | ✓ |
| Light level (rename + encrypt) | ✓ | ✓ |
| Medium level (+ int-split + CF-flatten) | ✗ | ✓ |
| Heavy level (+ dead code injection) | ✗ | ✓ |
| Multi-file project protection | ✗ | ✓ |
| Cross-file rename consistency | ✗ | ✓ |
| Deterministic seed (reproducible builds) | ✗ | ✓ |
| HMAC-SHA256 license generation | ✗ | ✓ |
| Ed25519 license generation | ✗ | ✓ |
| Hardware binding | ✗ | ✓ |
| Forensic watermarking | ✗ | ✓ |
| JSON + Markdown protection report | ✓ | ✓ |
| DOT dependency graph | ✓ | ✓ |
| PNG dependency graph | ✗ | ✓ |
| Build fingerprint | ✓ | ✓ |
| Compatibility analyser | ✓ | ✓ |
| Protection score | ✓ | ✓ |
| Diff viewer | ✓ | ✓ |

Run `land editions` at any time to print this table in your terminal.

---
