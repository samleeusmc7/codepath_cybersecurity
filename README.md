# Project 7 - WordPress Pentesting

Time spent: **12** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) Vulnerability Name or ID : WPVDB ID 7945
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [X] GIF Walkthrough: https://imgur.com/mBhEwaf
  - [X] Steps to recreate: 
    - Create a new post and in the title type in
    - <"beginnig tag">a href = " " onmouseover = "alert('XSS!'); ">exploit 1 (xss)<"end tag">
    - Make sure to put the beginning and end tags (<"a"> <"/a">)
    - Do not add the quotes for the tags
    - Then view the post and hover over the title of the post and the XSS attack will occur
  - [ ] Affected source code:
2. (Required) Vulnerability Name or ID WPVDB ID 7979
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [X] GIF Walkthrough: https://imgur.com/6vrcc1Z 
  - [X] Steps to recreate: 
    - Create a new page and in the title type in <BODY ONLOAD=alert('XSS')>
    - Then view the page and the XSS attack will occur
  - [ ] Affected source code:
3. (Required) Vulnerability Name or ID WPVDB 8111
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.3
  - [X] GIF Walkthrough: https://imgur.com/4dcmb4n
  - [X] Steps to recreate: 
    - Create a new page and in the title type in <"beginning tag">a href="INSERT AN IMAGE "><img class="alignnone size-full wp-image-38" src=" INSERT AN IMAGE " alt=" NAME OF IMAGE " onmouseover = "alert('XSS ATTACK!')" width="259" height="194" /><"end tag">
    - Make sure to put the beginning and end tags (<"a"> <"/a">)
    - Do not add the quotes for the tags
    - Then hover over the image and the XSS attack will occur
  - [ ] Affected source code:

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [2019] [Samul Lee]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
