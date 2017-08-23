# Project 7 - WordPress Pentesting

Time spent: **14** hours spent in total

> Objective: Find, analyze, recreate, and document **three vulnerabilities** affecting an old version of WordPress (4.2)

## Pentesting Report

1. Title: WordPress 3.3-4.7.4 - Large File Upload Error XSS
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.7.5
  - [X] GIF Walkthrough: http://imgur.com/a/E5McW
  - [X] Steps to recreate: Add a script on the backend of the website and have it triggered over a basic event such as File Upload. 
  - [X] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
2.Title: WordPress 2.5.0-4.7.4 - Filesystem Credentials Dialog CSRF 
  - [X] Summary: 
    - Vulnerability types: User Authentication
    - Tested in version: 4.2
    - Fixed in version: 4.7.5
  - [X] GIF Walkthrough: http://imgur.com/a/ebCfI
  - [X] Steps to recreate: Using your BURP Client, the sessionID can easily be decoded using the decoder and can be repeated into an admin session status using the encoder and repeater.
  - [X] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/home.php)
3. Title: WordPress <= 4.2.3 - wp_untrash_post_comments SQL Injection 
  - [X] Summary: 
    - Vulnerability types: SQL Injection
    - Tested in version: 4.2
    - Fixed in version: 4.3
  - [X] GIF Walkthrough: http://imgur.com/a/Ffspv
  - [X] Steps to recreate: Go into the Login page and a Brute Force Attack using SQL Injection is possbile because of lack of attempt count on the home page.
  - [X] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/home.php)

## Assets

Kali Linux

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Lots of Technical Adjustments needed to be made for Windows Set up.

## License

    Copyright [2017] [Aman Luthra]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
