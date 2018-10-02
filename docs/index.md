## Purpose
The purpose of this tool is to control and improve the quality and consistency of PDF file collections. For example directory structures containing PDF documents, PDF ebook libraries et cetera. This command-line tool is free for personal and commercial use. 

## Features
Currently the tool only allows for detecting the PDF files in a directory and validate International Standard Book Number (ISBN) in filenames using the `--isbn-validate-filenames` argument. Future features may include language, OCR and JS detection. 

## Usage
1. Download the tool for your platform and architecture
2. Verify the checksum with the corresponding checksum below
3. Rename the downloaded binary to `pdfcollection`
4. Run `pdfcollection --help` for information regarding all arguments such as `--directory`, `--verbose` and `--isbn-validate-filenames`

## Download
This tool is originally written using node.js and compiled for different platforms and architectures using [zeit/pkg](https://github.com/zeit/pkg). The current version is `0.1-beta` and is available for `windows`, `linux`, `macosx` and `alpine`.

Platform     | x64 (64-bit)  | x86 (32-bit)
:----------- |:-------------:| -----------:
Windows      | [download](/assets/downloads/pdf-collection/v0.1-beta/pdfcollection-v0.1-beta-win-x64.exe) | [download](/assets/downloads/pdf-collection/v0.1-beta/pdfcollection-v0.1-beta-win-x86.exe)
Linux        | [download](/assets/downloads/pdf-collection/v0.1-beta/pdfcollection-v0.1-beta-linux-x64) | [download](/assets/downloads/pdf-collection/v0.1-beta/pdfcollection-v0.1-beta-linux-x86)
MacOS        | [download](/assets/downloads/pdf-collection/v0.1-beta/pdfcollection-v0.1-beta-macos-x64) | [download](/assets/downloads/pdf-collection/v0.1-beta/pdfcollection-v0.1-beta-macos-x86)
Alpine       | [download](/assets/downloads/pdf-collection/v0.1-beta/pdfcollection-v0.1-beta-alpine-x64) | n/a

## Checksums
    d6a82459a145b59c530a462952f2de37ba746eb2 pdfcollection-v0.1-beta-alpine-x64
    a1729ef81cff8c81c525c18dbcb352780a97ba39 pdfcollection-v0.1-beta-linux-x64
    ddb773a6d4c8f4a883a48b1da37fecc53b6f617c pdfcollection-v0.1-beta-linux-x86
    58c87c31e3b9e205d44d907d8f05cda384263bfa pdfcollection-v0.1-beta-macos-x64
    c9cf168560779beb7fbad53d77f8e20fda941865 pdfcollection-v0.1-beta-macos-x86
    400faf5222ade2928793e345a4551fd5caffd2dd pdfcollection-v0.1-beta-win-x64.exe
    c4988eb35d0ab5de39644bf02b5a8949574febb4 pdfcollection-v0.1-beta-win-x86.exe
	
## Changelog

version 0.1-beta *(October 2th, 2018)*

* Initial beta version with only with main feature to validate ISBN in filenames