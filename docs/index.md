## Purpose
The purpose of this tool is to control and improve the quality and consistency of collections with PDF files. Even when the collection is a massive unstructured mess. Collections include but are not limited to directories with documents, e-book libraries et cetera. This command-line tool and it's embedded dependencies are all licensed under the MIT license and therefor free for personal and commercial use.

## Download
The current version of this tool is `0.2-beta`. The tool is available for the x64 (64-bit) and x86 (32-bit) architectures of the `windows`, `linux` and `macos` platforms. The binary for `alpine` is x64-only. *If you're not sure which architecture to use, use the x86 version (it works on both).*

**Platform** | **x64**       | **x86**
:----------- |:-------------:| :-----------:
Windows      | [download](/assets/downloads/pdf-collection/v0.2-beta/pdfcollection-v0.2-beta-win-x64.exe) (22mb) | [download](/assets/downloads/pdf-collection/v0.2-beta/pdfcollection-v0.2-beta-win-x86.exe) (18mb)
Linux        | [download](/assets/downloads/pdf-collection/v0.2-beta/pdfcollection-v0.2-beta-linux-x64) (33mb) | [download](/assets/downloads/pdf-collection/v0.2-beta/pdfcollection-v0.2-beta-linux-x86) (32mb)
MacOS        | [download](/assets/downloads/pdf-collection/v0.2-beta/pdfcollection-v0.2-beta-macos-x64) (34mb) | [download](/assets/downloads/pdf-collection/v0.2-beta/pdfcollection-v0.2-beta-macos-x86) (30mb)
Alpine       | [download](/assets/downloads/pdf-collection/v0.2-beta/pdfcollection-v0.2-beta-alpine-x64) (35mb) | *n/a*

*Older versions can be found on the [older versions](versions.md) page.*


## Usage
Steps to get started:
1. Download the tool
2. Verify the SHA1 checksum
3. Rename the downloaded binary to `pdfcollection`
4. Run `pdfcollection --help`

### Options
Currently the tool supports recursive PDF file detection starting from the path specified in the `--directory=...` argument. International Standard Book Number (ISBN) filename validation using the `--isbn-validate-filenames` argument and exporting the invalid ISBN filepaths into one of the following machine readable data formats:
* JavaScript Object Notation (JSON) using `--machine-json`
* Extensible Markup Language (XML) using `--machine-xml`
* YAML Ain't Markup Language (YAML) using `--machine-yaml`

Choosing a machine readable data format will only work combination with the argument `--machine-print` or `--machine-file=...`.

Furthermore the options `--verbose`, `--version`, `--license` and `--help` are available. See `--help` for more information regarding the use of this tool.

## SHA1 checksums
    f413d23b304e7e30ffa98c58c6888e9b244587dc *pdfcollection-v0.2-beta-alpine-x64
    a8956a8ed424601d494a3fab0867fb0f524943e6 *pdfcollection-v0.2-beta-linux-x64
    706924ae70bd9384809a165c9ac0d5bd38859dec *pdfcollection-v0.2-beta-linux-x86
    b0276ee075dc80533d001b3aa59fae3eef4c8e58 *pdfcollection-v0.2-beta-macos-x64
    ef481e63898af0658b9564b411a964e50f0a25a3 *pdfcollection-v0.2-beta-macos-x86
    2e6c802ce202822da9cfc20ab4d854f0f636131a *pdfcollection-v0.2-beta-win-x64.exe
    6f7c0faaa44071c1515509907fd3e753b5794774 *pdfcollection-v0.2-beta-win-x86.exe


## Changelog
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
