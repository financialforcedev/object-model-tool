object-model-tool
=================

An extensible tool to generate object-model/ERD diagrams from salesforce metadata.

![Screenshot of the created artifact](/img/example.png)

Introduction
------------

This tool was created to generate object-model/ERD Diagrams for custom objects in salesforce. There was a requirement for external diagrams that could not be filled by the internal salesforce schema builder or any other tool that I could find.

As a result, I built an extensible, lightweight tool to generate and orginize object diagrams by functional area. The tool has multiple possible configurations and additional functionality can be built on top of the existing framework with ease.

Summary
-------

This tool is a command line utility (that also has an ant entry point). The output it produces is contained within a 'htmlcharts' folder. The utility reads salesforce metadata, either locally or from a salesforce org, and parses this information into object-model/ERD charts. These charts are provided in html format along with several helper files (javascript, css, etc). The charts can be arranged by 'functional area', in other words, split down into logical groups for easy digestion.

Key Features
------------

* Multiple processor configurations for different use cases.
* Shows relationships between objects.
* Can Provide draggable charts in html format.
* Can Provide draggable charts split by functional area in html format.
* Can provide a list of custom objects and fields in CSV format.

Build & Run
-----------

To build the utility, check out the master branch, navigate to the **'root folder/objectmodelutil'** and from your console, type **'ant'** (this assumes you have ant installed).

To run the utility, type **'ant run'** after building. The default run command in **'build.xml'** points at the **'demo'** folder and performs a local retreive of metadata, arranging the output into functional areas specified in **'demo/testareas.xml'**.

Reporting Issues & Enhancements
-------------------------------

Please report any issues / suggest any enhancements using github. Suggestions / bug reports are welcome as are extensions containing additional functionality.

License
-------

Copyright (c) 2014, FinancialForce.com, inc
All rights reserved.

Redistribution and use in source and binary forms, with or without modification, 
are permitted provided that the following conditions are met:
- Redistributions of source code must retain the above copyright notice, 
     this list of conditions and the following disclaimer.
- Redistributions in binary form must reproduce the above copyright notice, 
     this list of conditions and the following disclaimer in the documentation 
     and/or other materials provided with the distribution.
- Neither the name of the FinancialForce.com, inc nor the names of its contributors 
     may be used to endorse or promote products derived from this software without 
     specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND 
 ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES 
 OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL 
 THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, 
 EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
 OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
 OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

**jsPlumb** is distributed under the GPLv2 and MIT Licenses: [jsPlumb](http://www.jsplumb.org)

**jQuery** is distributed under the MIT License: [jQuery](http://jquery.com)