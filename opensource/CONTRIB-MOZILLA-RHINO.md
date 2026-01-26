# Mozilla Rhino Contributions

> JavaScript Engine — ES2024/ES2025 Feature Implementation

[![Rhino](https://img.shields.io/github/stars/mozilla/rhino?style=flat-square)](https://github.com/mozilla/rhino)

## About Rhino

Rhino is Mozilla's JavaScript engine written in Java. Used for:
- Server-side JavaScript in Java applications
- Salesforce Apex/Flow automation
- Embedded scripting in Java apps
- Testing and automation frameworks

## Merged Contributions

### ES2025 Features

| Feature | Description | Status |
|---------|-------------|--------|
| `Promise.try` | Wraps sync code in promise, catching errors | ✅ Merged |
| `Promise.withResolvers` | Returns { promise, resolve, reject } | ✅ Merged |
| Set Methods | union, intersection, difference, etc. | ✅ Merged |
| ArrayBuffer Transfer | transfer(), transferToFixedLength() | ✅ Merged |
| `Math.f16round` | Round to 16-bit float | ✅ Merged |
| `Error.isError` | Static method for Error checking | ✅ Merged |

### Bug Fixes

| Fix | Issue | Status |
|-----|-------|--------|
| Array.from iterator priority | Spec compliance | ✅ Merged |
| BigInt.asUintN/asIntN | #1573 | ✅ Merged |
| ISO date millisecond rounding | Parsing accuracy | ✅ Merged |

## Impact

Every Rhino contribution affects:
- Enterprise Java applications
- Salesforce automation (millions of orgs)
- Testing frameworks
- Legacy systems with embedded JS

## Links

- [Mozilla Rhino](https://github.com/mozilla/rhino)
- [My Fork](https://github.com/anivar/rhino)
