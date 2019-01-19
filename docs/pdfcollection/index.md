# pdfcollection
## General
The purpose of this command-line tool is to control and improve the quality and consistency of collections with Portable Document Format (PDF) files. Even when the collection is a massive unstructured mess. Collections include but are not limited to directories with documents, e-book libraries et cetera. This tool and it's embedded dependencies are all licensed under the MIT license and therefor free for personal and commercial use.

## Download
The current version of this tool is `0.5.0 (beta)`. The tool is available for the platforms `windows`, `linux` and `macos` for the architectures x64 (64-bit) and x86 (32-bit). The `alpine`-platform is x64-only. *If you're not sure which architecture to use, use the x86 version (it works on both).*

**Platform** | **x64**       | **x86**
:----------- |:-------------:| :-----------:
Windows      | [download](/docs/pdfcollection/downloads/0.5.0/win/x64/pdfcollection.zip) | [download](/docs/pdfcollection/downloads/0.5.0/win/x86/pdfcollection.zip)
Linux        | [download](/docs/pdfcollection/downloads/0.5.0/linux/x64/pdfcollection.zip) | [download](/docs/pdfcollection/downloads/0.5.0/linux/x86/pdfcollection.zip)
MacOS        | [download](/docs/pdfcollection/downloads/0.5.0/macos/x64/pdfcollection.zip) | [download](/docs/pdfcollection/downloads/0.5.0/macos/x86/pdfcollection.zip)
Alpine       | [download](/docs/pdfcollection/downloads/0.5.0/alpine/x64/pdfcollection.zip) | *n/a*

*Previous versions are no longer available for download. But the checksums can still be verified on the [checksum](/docs/pdfcollection/checksums) page.*

## Get started
1. Download the tool
2. Verify the SHA1 checksum
3. Run `pdfcollection --help` to get started

### Options
#### Detection
* `--directory` The directory of the PDF collection (recursive scan)
* `--duplicates` Find duplicate files based on SHA1 hashing
* `--isbn-file-validate` Validate ISBN-10 or ISBN-13 in filenames
* `--isbn-file-duplicate` Find duplicate ISBN filenames (cross-check ISBN-10 and ISBN-13)
* `--mime` Validate magic-byte (mime-type) and warns about small file sizes

#### Exporting
* `--output-file` Write results to chosen data format
* `--data-json` Use JavaScript Object Notation (JSON)
* `--data-xml` Use Extensible Markup Language (XML)
* `--data-yaml` Use YAML Ain't Markup Language (YAML)
* `--data-toml` Use Tom's Obvious, Minimal Language (TOML)

#### Other
* `--help` Help guide
* `--quiet` Suppress console output
* `--version` Version and credits
* `--license` Licenses of tool and dependencies

## Verify your downloads
Below are the SHA1 hashes of the compiled and compressed files.

    4911590344ed1109e8aa41099dcb542238eb1a47 - 0.5.0/alpine/x64/pdfcollection.zip
    0f47f7a81abc17deeb41e5b2950f199d6504c13c - 0.5.0/linux/x64/pdfcollection.zip
    3b94a3ffad08c09a7e005e490837cfce0a7fea90 - 0.5.0/linux/x86/pdfcollection.zip
    4d04e640f7a724bffa1ee780239bc1f88748798f - 0.5.0/macos/x64/pdfcollection.zip
    60cb2eef39630336b8abc8f723db5f6706b8a03e - 0.5.0/macos/x86/pdfcollection.zip
    269a6f4eab8bd9afe15d6bcc94a85e2d6cc0762e - 0.5.0/win/x64/pdfcollection.zip
    124b10cb7c27def303a10da0e3323b7adbd75080 - 0.5.0/win/x86/pdfcollection.zip

## Changelog
    version 0.5.0 (beta) *(January 19th, 2019)*
    * Added functionality to detect incorrect magic-bytes (mime-types) and small file sizes
    * Renamed several options (always see `--help` for the latest)
    * Several minor bugfixes
    * Performance improvements
    * Updated dependencies
    * Improved documentation

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
Future features may or may not include:

    * file integrity/corruption checking
    * PDF/A validation
    * additional methods of locating (possible) duplicate files
    * detection of natural language
    * detection of OCR-usage
    * detection of (potentially dangerous) JavaScript
    * detection of PDF protection
    * OCR
    * fuzzy scan detection
    * automatic page rotation
    * automatic page dewarping
    * detection of wrongly rotated pages
    * barcode detection
    * e-book ISBN detection
    * e-book cover detection
    * additional machine readable formats (like CSON)
    * additional export formats like (TXT, HTML, PDF, CSV or XLS)
    * spelling checker

## MIT license
Copyright 2018-2019 - fusioncode.eu

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

*This same MIT license applies to all dependencies. When using the option `--license` all licenses will appear.*
