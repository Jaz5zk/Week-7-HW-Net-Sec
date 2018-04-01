# Week-7-HW-Net-Sec
# Project 7 - WordPress Pentesting  

Report  1. (Required) Authenticated Short code Tags
  - [X] Summary:     Cross Site Scripting Attack Authenticated Short code Tags
- Vulnerability types:  Cross Site Scripting
- Tested in version:  WP 4.2   
- Fixed in version:   WP 4.3
- [X] GIF Walkthrough: <img src="https://github.com/Jaz5zk/Week-7-HW-Net-Sec/blob/master/AuthenticatedShortCodeTags.gif" width="800">    
- [X] Steps to recreate:   create a page with a mouseover alert and it causes an attack to fail 
- [X] Affected source code:   
TEST!!![caption width="1" caption='<a href="' ">]</a><a href="http://onMouseOver='alert(1)'">Click me</a>
  
[Link1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 

1. (Required) Unauthenticated Genericons Cross-Site Scripting  
- [X] Summary:    Did a cross site scripting attack by throwing an on error
- Vulnerability types:     Cross site Scripting
- Tested in version:    4.2 
- Fixed in version:    4.2.2
- [X] GIF Walkthrough:    
- [X] Steps to recreate:    Go to the example page and edit in this alert: http://www.example.com/wp-content/themes/twentyfifteen/genericons/example.html#1<img/ src=1 onerror= alert(1)>
which will cause an error once the page is visited
-	[X] Affected source code:     
http://www.example.com/wp-content/themes/twentyfifteen/genericons/example.html#1<img/ src=1 onerror= alert(1)>

[Link1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 

1. (Required) Authenticated Stored Cross site scripting in youtube URL embedds  
- [X] Summary:      create a bad youtube url that throws an error through cross site scripting
- Vulnerability types:   Cross site scripting  
- Tested in version:     4.2
- Fixed in version:    4.2.13
- [X] GIF Walkthrough:    
- [X] Steps to recreate:   Copy youtube url given through the blog page you can access after running wpscan in your kali vm. This blog will have a youtube url that you embed into the sample page to cause an error. 
- [X] Affected source code: 
https://youtube[.]com/watch?v=abc<svg onload=alert(1)>
    
- [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 

1. (Optional) Vulnerability Name or ID   - [ ] Summary:      - Vulnerability types:     - Tested in version:     - Fixed in version:    - [ ] GIF Walkthrough:    - [ ] Steps to recreate:    - [ ] Affected source code:     - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 1. (Optional) Vulnerability Name or ID   - [ ] Summary:      - Vulnerability types:     - Tested in version:     - Fixed in version:    - [ ] GIF Walkthrough:    - [ ] Steps to recreate:    - [ ] Affected source code:     - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)   ## Assets  List any additional assets, such as scripts or files  ## Resources  - [WordPress Source Browser](https://core.trac.wordpress.org/browser/) - [WordPress Developer Reference](https://developer.wordpress.org/reference/)  GIFs created with [LiceCap](http://www.cockos.com/licecap/).  ## Notes  Describe any challenges encountered while doing the work  ## License      Copyright [yyyy] [name of copyright owner]      Licensed under the Apache License, Version 2.0 (the "License");     you may not use this file except in compliance with the License.     You may obtain a copy of the License at          http://www.apache.org/licenses/LICENSE-2.0      Unless required by applicable law or agreed to in writing, software     distributed under the License is distributed on an "AS IS" BASIS,     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.     See the License for the specific language governing permissions and     limitations under the License.
