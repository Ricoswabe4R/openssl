# Welcome to the OpenSSL Project

[![OpenSSL Logo]][www.openssl.org]

[![GitHub Actions CI Badge]][GitHub Actions CI]
![Nightly OS Zoo CI Badge](https://github.com/openssl/openssl/actions/workflows/os-zoo.yml/badge.svg)
![Provider Compatibility](https://github.com/openssl/openssl/actions/workflows/provider-compatibility.yml/badge.svg)
![QUIC Interop](https://github.com/openssl/openssl/actions/workflows/run_quic_interop.yml/badge.svg)
![Daily Checks](https://github.com/openssl/openssl/actions/workflows/run-checker-daily.yml/badge.svg)

OpenSSL is a robust, commercial-grade, and full-featured Open Source Toolkit for the **TLS** (formerly SSL), **DTLS**, and **QUIC** protocols. It is built on a general-purpose cryptographic library that can also be used independently. The toolkit includes a cryptographic module validated to conform with **FIPS standards**.

OpenSSL originated from the SSLeay library, developed by **Eric A. Young** and **Tim J. Hudson**.

The official home page of the OpenSSL Project is [www.openssl.org].

---

## 📚 Table of Contents

- [Overview](#overview)
- [Download](#download)
- [Build and Install](#build-and-install)
- [Documentation](#documentation)
- [License](#license)
- [Support](#support)
- [Contributing](#contributing)
- [Legalities](#legalities)

---

## 🔍 Overview

The OpenSSL toolkit consists of:

- **libssl**: Implements all TLS protocol versions up to **TLSv1.3** ([RFC 8446]), DTLS protocol versions up to **DTLSv1.2** ([RFC 6347]), and the **QUIC version 1** protocol ([RFC 9000]).
- **libcrypto**: A full-strength general-purpose cryptographic library, which serves as the foundation for TLS implementations but can also be used independently.
- **openssl**: A command-line tool that provides a versatile set of cryptographic utilities for:
  - Key parameter generation
  - X.509 certificates, CSRs, and CRLs
  - Message digests
  - Encryption and decryption
  - SSL/TLS/DTLS client and server tests
  - QUIC client tests
  - S/MIME signed/encrypted email handling
  - And more...

---

## 📥 Download

### For Production Use
- Official release source code tarballs are available at [openssl-library.org/source](https://openssl-library.org/source/).
- Precompiled binaries for various platforms are provided by third-party vendors. Refer to the [Binaries] page on our wiki for more details.

### For Testing and Development
- Clone the public GitHub mirror for access to the full project history:
  ```bash
  git clone https://github.com/openssl/openssl.git
  ```
- If contributing, fork the repository and clone your fork:
  ```bash
  git clone https://github.com/<your-username>/openssl.git
  ```

All development is done via GitHub pull requests. See the [Contributing](#contributing) section for details.

---

## ⚙️ Build and Install

Refer to the [INSTALL](INSTALL.md) file for detailed instructions on building and installing OpenSSL. Additional platform-specific notes can be found in:

- [Notes for UNIX-like platforms](NOTES-UNIX.md)
- [Notes for Android platforms](NOTES-ANDROID.md)
- [Notes for Windows platforms](NOTES-WINDOWS.md)
- [Notes for DOS with DJGPP](NOTES-DJGPP.md)
- [Notes for OpenVMS](NOTES-VMS.md)
- [Notes on Perl](NOTES-PERL.md)
- [Notes on Valgrind](NOTES-VALGRIND.md)

For upgrading to OpenSSL 3.x, see the [ossl-guide-migration(7ossl)] manual page.

---

## 📖 Documentation

### Readme Files
- [QUIC Protocol Information](README-QUIC.md)
- [Provider Architecture Details](README-PROVIDERS.md)
- [FIPS Module Usage](README-FIPS.md)
- [Legacy Engine Architecture](README-ENGINES.md)

### OpenSSL Guide
Introductory and tutorial content is available in the [OpenSSL Guide].

### Manual Pages
Access the manual pages for various OpenSSL versions:
- [Master Branch Documentation](https://docs.openssl.org/master/)
- [Version 3.5](https://docs.openssl.org/3.5/)
- [Version 3.4](https://docs.openssl.org/3.4/)
- [Version 3.3](https://docs.openssl.org/3.3/)
- [Version 3.2](https://docs.openssl.org/3.2/)
- [Version 3.0](https://docs.openssl.org/3.0/)

### Demos
Explore source code demos in the [demos subfolder](./demos).

---

## 📜 License

OpenSSL is licensed under the **Apache License 2.0**, allowing free use for both commercial and non-commercial purposes, provided the conditions are met. For details, see the [LICENSE.txt](LICENSE.txt) file.

---

## 🤝 Support

For support and inquiries, refer to the [SUPPORT](SUPPORT.md) file to determine the appropriate channel for your needs.

---

## 🌟 Contributing

If you'd like to contribute to OpenSSL, review the [CONTRIBUTING](CONTRIBUTING.md) file for guidelines on submitting pull requests and patches.

---

## ⚖️ Legalities

Cryptographic software may be subject to export or use restrictions in some countries. Seek legal advice if you are unsure about compliance with local laws.

---

## © Copyright

- **1998-2025**: The OpenSSL Project Authors
- **1995-1998**: Eric A. Young and Tim J. Hudson

All rights reserved.

---

<!-- Links -->

[www.openssl.org]: https://www.openssl.org "OpenSSL Homepage"
[GitHub Actions CI Badge]: https://github.com/openssl/openssl/workflows/GitHub%20CI/badge.svg "GitHub Actions CI Status"
[GitHub Actions CI]: https://github.com/openssl/openssl/actions?query=workflow%3A%22GitHub+CI%22 "GitHub Actions CI"
[Binaries]: https://github.com/openssl/openssl/wiki/Binaries "OpenSSL Binary Downloads"
[OpenSSL Guide]: https://docs.openssl.org/master/man7/ossl-guide-introduction "OpenSSL Guide Introduction"
[ossl-guide-migration(7ossl)]: https://docs.openssl.org/master/man7/ossl-guide-migration "OpenSSL Migration Guide"
[RFC 8446]: https://tools.ietf.org/html/rfc8446
[RFC 6347]: https://tools.ietf.org/html/rfc6347
[RFC 9000]: https://tools.ietf.org/html/rfc9000
