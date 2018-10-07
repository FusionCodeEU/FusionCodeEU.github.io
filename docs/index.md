## pdfcollection v0.3-beta
The purpose of this command-line tool is to control and improve the quality and consistency of collections with Portable Document Format (PDF) files. Even when the collection is a massive unstructured mess. Collections include but are not limited to directories with documents, e-book libraries et cetera. This tool and it's embedded dependencies are all licensed under the MIT license and therefor free for personal and commercial use.

## Download
The current version of this tool is `0.3-beta`. The tool is available for the x64 (64-bit) and x86 (32-bit) architectures of the `windows`, `linux` and `macos` platforms. The binary for `alpine` is x64-only. *If you're not sure which architecture to use, use the x86 version (it works on both).*

**Platform** | **x64**       | **x86**
:----------- |:-------------:| :-----------:
Windows      | [download](/assets/downloads/pdf-collection/v0.3-beta/pdfcollection-v0.3-beta-win-x64.exe) (22mb) | [download](/assets/downloads/pdf-collection/v0.3-beta/pdfcollection-v0.3-beta-win-x86.exe) (18mb)
Linux        | [download](/assets/downloads/pdf-collection/v0.3-beta/pdfcollection-v0.3-beta-linux-x64) (33mb) | [download](/assets/downloads/pdf-collection/v0.3-beta/pdfcollection-v0.3-beta-linux-x86) (32mb)
MacOS        | [download](/assets/downloads/pdf-collection/v0.3-beta/pdfcollection-v0.3-beta-macos-x64) (34mb) | [download](/assets/downloads/pdf-collection/v0.3-beta/pdfcollection-v0.3-beta-macos-x86) (30mb)
Alpine       | [download](/assets/downloads/pdf-collection/v0.3-beta/pdfcollection-v0.3-beta-alpine-x64) (35mb) | *n/a*

*Previous versions can be found on the [previous versions](versions.md) page.*


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

#### Machine readable data options
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
    fb59603d289701166d0122b0dda373dd96ee1a8d *pdfcollection-v0.3-alpine-x64
    009fccf7c40b6c6d4f1704a7b51d9f0c63bd468a *pdfcollection-v0.3-linux-x64
    ec36c7a13384bf3b5621e04a9bdd6861b296509b *pdfcollection-v0.3-linux-x86
    2bc57a364076117d9d1e3375a6ff6393e9d92993 *pdfcollection-v0.3-macos-x64
    9a56e42113e1888a5beeabe41e73d5b50247201c *pdfcollection-v0.3-macos-x86
    eadb5df28c341c719250205772c36f2d706211c0 *pdfcollection-v0.3-win-x64.exe
    ae35f1ad105b21de09163f6e8a6c6b7af508dfe8 *pdfcollection-v0.3-win-x86.exe

## Changelog
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
