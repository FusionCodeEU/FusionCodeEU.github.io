# pdfcollection v0.4-beta
## General
The purpose of this command-line tool is to control and improve the quality and consistency of collections with Portable Document Format (PDF) files. Even when the collection is a massive unstructured mess. Collections include but are not limited to directories with documents, e-book libraries et cetera. This tool and it's embedded dependencies are all licensed under the MIT license and therefor free for personal and commercial use.

## Download
The current version of this tool is `0.4-beta`. The tool is available for the x64 (64-bit) and x86 (32-bit) architectures of the `windows`, `linux` and `macos` platforms. The binary for `alpine` is x64-only. *If you're not sure which architecture to use, use the x86 version (it works on both).*

**Platform** | **x64**       | **x86**
:----------- |:-------------:| :-----------:
Windows      | [download](/assets/downloads/pdf-collection/v0.4-beta/pdfcollection-v0.4-beta-win-x64.exe) (22mb) | [download](/assets/downloads/pdf-collection/v0.4-beta/pdfcollection-v0.4-beta-win-x86.exe) (18mb)
Linux        | [download](/assets/downloads/pdf-collection/v0.4-beta/pdfcollection-v0.4-beta-linux-x64) (33mb) | [download](/assets/downloads/pdf-collection/v0.4-beta/pdfcollection-v0.4-beta-linux-x86) (32mb)
MacOS        | [download](/assets/downloads/pdf-collection/v0.4-beta/pdfcollection-v0.4-beta-macos-x64) (34mb) | [download](/assets/downloads/pdf-collection/v0.4-beta/pdfcollection-v0.4-beta-macos-x86) (30mb)
Alpine       | [download](/assets/downloads/pdf-collection/v0.4-beta/pdfcollection-v0.4-beta-alpine-x64) (35mb) | *n/a*

*Previous versions are no longer available for download. But the checksums can still be verified on the [previous versions](versions.md) page.*

## Usage
Steps to get started:
1. Download the tool
2. Verify the SHA1 checksum
3. Rename the downloaded binary to `pdfcollection`
4. Run `pdfcollection --help`

### Options
#### General options
* `--directory` The directory of the PDF collection
* `--duplicates` Find duplicate files based on SHA1 hashing
* `--verbose` Amount of information printed (1=less, 2=normal, 3=more, 9=debug)

#### ISBN options
* `--isbn-validate-filenames` Perform ISBN-10 and ISBN-13 validation on filenames
* `--isbn-duplicate-filenames` Cross-checking ISBN filenames with ISBN-10 and ISBN-13

#### Export options (machine readable data)
* `--machine-file` Suppress normal output and write data in chosen format to specified file path
* `--machine-print` Suppress normal output and print machine readable data in chosen format
* `--machine-json` Use JavaScript Object Notation (JSON)
* `--machine-xml` Use Extensible Markup Language (XML)
* `--machine-yaml` Use YAML Ain't Markup Language (YAML)
* `--machine-toml` Use Tom's Obvious, Minimal Language (TOML)

#### Other options
* `--help` Show help guide
* `--version` Show the version of the tool and platform and show (dependency) credits
* `--license` Show tool license

## SHA1 checksums
    611d103708e8280de8e626129b875ce0194b4d26 *pdfcollection-v0.4-beta-alpine-x64
    7211070c115081eae07d41179eaa11f5e6925bb1 *pdfcollection-v0.4-beta-linux-x64
    cc9339c5001699605c6575d1dfa83fc9c657b7c5 *pdfcollection-v0.4-beta-linux-x86
    5c88d0b85db6aac0bd5deff34d32613677bcaf99 *pdfcollection-v0.4-beta-macos-x64
    0a4de8839ab1000eac1a5da4c247998f8c666f48 *pdfcollection-v0.4-beta-macos-x86
    f329210701827a2d1469049f8dd02b710ba3e027 *pdfcollection-v0.4-beta-win-x64.exe
    64ec490bc05a3087760e472c91cf796b3cb165b1 *pdfcollection-v0.4-beta-win-x86.exe

## Changelog
    version 0.4-beta *(October 8th, 2018)*
    * Added `--isbn-duplicate-filenames` for cross-checking ISBN filenames with ISBN-10 and ISBN-13

    version 0.3-beta *(October 7th, 2018)*
    * Added `--duplicates` option for finding identical files (using SHA1 hashing)
    * Added `--machine-toml` for supporting machine readable output in Tom's Obvious, Minimal Language (TOML)

    version 0.2-beta *(October 4th, 2018)*
    * Improved argument consistency
    * Adding machine readable format `xml`
    * Adding machine readable format `yaml`
    * Performance improvements
    * Improved help guide
    * Included credits to dependency authors
    * Included references to dependency licenses

    version 0.1-beta *(October 2th, 2018)*
    * Initial beta version
    * Recursive PDF file detection
    * ISBN filename validation
    * Export data in JSON format

## Future features
    Future features may include:
    * file integrity checking
    * duplicate file locator
    * detection of natural language
    * detection of OCR-usage
    * detection of (potentially dangerous) JavaScript
    * detection of protection
    * detection of wrongly rotated pages
    * OCR
    * e-book ISBN detection
    * e-book cover detection
    * additional machine readable formats

## MIT license
Copyright 2018 - fusioncode.eu

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

*This same MIT license applies to all dependencies. When using the option `--license` all licenses will appear.*
