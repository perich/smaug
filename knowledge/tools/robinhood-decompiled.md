# Robinhood App Decompiled

**Repository:** https://github.com/ScriptedAlchemy/robinhood-decompiled

**Language:** Java | **Stars:** 75

## Summary

Complete Java decompile of the Robinhood Android application, organized for code review and security analysis. Includes full source code, resources, native libraries, and audit bundles.

## Repository Structure

### Main Directories

**`app/`** - Full fidelity decompile output
- `app/sources/` - Java code
- `app/resources/` - Android resources, manifest, META-INF, native libs (.so files)
- Canonical complete decompile with native library binaries

**`audit/`** - Audit-oriented review material
- `audit/sources/` - Curated subset of Robinhood-owned code (excludes third-party libs)
- `audit/resources/` - Selected resources for analysis
- `audit/protos/` - Extracted protobuf definitions
- `audit/reports/` - Generated analysis summaries
- `audit/manifest/` - AndroidManifest.xml extracted for quick review
- `audit/meta/` - META-INF artifacts

## Navigation Guide

### Quick Entry Points

| Task | Location |
|------|----------|
| Search code | `app/sources/` |
| Find manifest | `app/resources/AndroidManifest.xml` or `audit/manifest/` |
| Skim permissions/components | `audit/reports/manifest_components.txt` |
| Identify feature areas | `audit/reports/top_packages.txt` |
| Find network endpoints | `audit/reports/url_hosts.txt` |

## Code Organization (Robinhood-owned subset)

**`com/robinhood/android/`** - Main app code (largest area)
- UI features, feature wiring
- Major product areas: transfers, creditcard, equity, crypto, futures, options
- Deep link routing, navigation shell

**`com/robinhood/shared/`** - Shared/business logic
- Trade flows (crypto, ladder)
- Order type models
- Support, security, document flows

**`com/robinhood/librobinhood/`** - Core client libraries
- Data store pattern (dominant subtree)
- Preference-backed storage
- Logging and experiments

**`com/robinhood/rosetta/`** - Schemas and event logging
- Event DTOs and schemas
- Cashier/payment DTOs
- Type converters between domains

**`com/robinhood/store/`** - Feature-scoped stores
- Futures, supportchat, paymentinstrument
- Stripe integration

## Use Cases

- Security analysis of app architecture and data flows
- Identification of API endpoints and backend contracts
- Examination of authentication and token handling
- Review of networking patterns and data transmission
- Understanding of payment processing implementation
