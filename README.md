# VerixID

> **A mathematical witness for digital files.**

VerixID provides cryptographic proof of file integrity and proof of existence without requiring the original file to be uploaded or stored.

Only a mathematical fingerprint of the file is processed.

**Verify, don't trust.**

---

## What is VerixID?

VerixID is a cryptographic verification service for digital files.

It helps establish that a specific digital file existed in a specific state at a specific time.

The verification is based on mathematics rather than trust in a central authority.

VerixID uses deterministic cryptographic methods so that verification can be independently reproduced and checked.

### In simple terms

If a file changes, its cryptographic fingerprint changes.

VerixID records that fingerprint together with a timestamp and cryptographic signature.

Later, the file can be hashed again and the result can be compared with the recorded proof.

If the fingerprints match, the file is unchanged from the recorded state.

---

## Why VerixID?

Digital files are easy to copy, modify, rename, or redistribute.

In many situations, the important question is not:

> "Where is my file stored?"

but:

> "Can I prove what this file was and when it existed?"

VerixID addresses this problem without taking custody of the original file.

This makes it useful when file privacy matters as much as verification.

---

## Zero-Custody

**The original file never needs to leave the user's device.**

VerixID does not require the original file to be uploaded, stored, or viewed by the verification system.

The file is processed locally to produce a cryptographic fingerprint.

Only the required cryptographic data is submitted for recording and verification.

### VerixID does not:

- Store user files
- Host user files
- Inspect file contents
- Reconstruct files from hashes
- Require blockchain
- Use AI to perform verification
- Require identity verification for basic file integrity verification

---

## How It Works

The basic process is simple:

```text
File
  │
  ▼
SHA-256
  │
  ▼
Cryptographic fingerprint
  │
  ├── Timestamp
  ├── Record ID
  └── Digital signature
          │
          ▼
     Verification record
          │
          ▼
   Independent verification
