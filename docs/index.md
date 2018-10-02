## Purpose
The purpose of this tool is to control and improve the quality and consistency of collections with PDF files. For example directories with documents, e-book libraries et cetera. This command-line tool licensed under the MIT license and therefor free for personal and commercial use.

## Current features
Currently the tool supports recursive PDF file detection,  International Standard Book Number (ISBN) filename validation using the `--isbn-validate-filenames` argument and exporting results into a machine readable format like JavaScript Object Notation (JSON) using the `--machine` argument.

This tool is originally written in JavaScript (node.js) and compiled for different platforms and architectures using [zeit/pkg](https://github.com/zeit/pkg).

## Download
The current version of this tool is `0.1-beta`. The tool is available for the x64 (64-bit) and x86 (32-bit)  architectures of the `windows`, `linux` and `macos` platform. The binary for `alpine` is x64-only.

**Platform**     | **x64 (64-bit)**  | **x86 (32-bit)**
:----------- |:-------------:| -----------:
Windows      | [download](/assets/downloads/pdf-collection/v0.1-beta/pdfcollection-v0.1-beta-win-x64.exe) | [download](/assets/downloads/pdf-collection/v0.1-beta/pdfcollection-v0.1-beta-win-x86.exe)
Linux        | [download](/assets/downloads/pdf-collection/v0.1-beta/pdfcollection-v0.1-beta-linux-x64) | [download](/assets/downloads/pdf-collection/v0.1-beta/pdfcollection-v0.1-beta-linux-x86)
MacOS        | [download](/assets/downloads/pdf-collection/v0.1-beta/pdfcollection-v0.1-beta-macos-x64) | [download](/assets/downloads/pdf-collection/v0.1-beta/pdfcollection-v0.1-beta-macos-x86)
Alpine       | [download](/assets/downloads/pdf-collection/v0.1-beta/pdfcollection-v0.1-beta-alpine-x64) | *n/a*

## Usage
1. Download the tool for your platform and architecture
2. Verify the sha1 checksum with one below
3. Rename the downloaded binary to `pdfcollection`
4. Run `pdfcollection --help` for information regarding  arguments such as `--directory`, `--verbose`, `--machine` and `--isbn-validate-filenames`

## Checksums (sha1)
    d6a82459a145b59c530a462952f2de37ba746eb2 pdfcollection-v0.1-beta-alpine-x64
    a1729ef81cff8c81c525c18dbcb352780a97ba39 pdfcollection-v0.1-beta-linux-x64
    ddb773a6d4c8f4a883a48b1da37fecc53b6f617c pdfcollection-v0.1-beta-linux-x86
    58c87c31e3b9e205d44d907d8f05cda384263bfa pdfcollection-v0.1-beta-macos-x64
    c9cf168560779beb7fbad53d77f8e20fda941865 pdfcollection-v0.1-beta-macos-x86
    400faf5222ade2928793e345a4551fd5caffd2dd pdfcollection-v0.1-beta-win-x64.exe
    c4988eb35d0ab5de39644bf02b5a8949574febb4 pdfcollection-v0.1-beta-win-x86.exe

## Changelog

version 0.1-beta *(October 2th, 2018)*

* Initial beta version (only PDF file detect and ISBN filename validation

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
* other machine readable formats such as XML, CSV or SQL
