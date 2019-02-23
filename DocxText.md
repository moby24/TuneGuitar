![](media/image1.wmf){width="1.3680555555555556in"
height="0.3111111111111111in"}

CAGE Code 81205

Cabin Services System (CSS)\
Airline Configuration Database Generator (ACDG) Requirements: ACDG Host

  ------------------ ------------------- ------------------------
  DOCUMENT NUMBER:   RELEASE/REVISION:   RELEASE/REVISION DATE:
  **D620Z012-09**    **B**               
  ------------------ ------------------- ------------------------

> CONTENT OWNER:
>
> **Cabin Systems Core Integration (66-ZB-E421)**
>
> All future revisions to this document must be approved by the content
> owner before release.

EXPORT COMPLIANCE NOTICE

THE INFORMATION CONTAINED HEREIN MAY CONTAIN TECHNICAL DATA\
WITHIN THE DEFINITION OF THE EXPORT ADMINISTRATION\
REGULATIONS, AND AS SUCH MAY BE SUBJECT TO THE EXPORT\
CONTROL LAWS OF THE UNITED STATES.\
TRANSFER OF THIS DATA BY ANY MEANS TO UNAUTHORIZED PERSONS,\
AS DEFINED BY THESE LAWS, WHETHER IN THE UNITED STATES OR\
ABROAD, WITHOUT AN EXPORT LICENSE OR OTHER APPROVAL FROM THE\
U.S. DEPARTMENT OF COMMERCE IS EXPRESSLY PROHIBITED.

**ECCN: 9E991**

The information contained herein is PROPRIETARY to The Boeing Company
and shall not be reproduced or disclosed in whole or in part or used for
any purpose except when the user possesses direct, written authorization
from The Boeing Company.

The information contained herein is PROPRIETARY to The Boeing Company
and shall not be reproduced or disclosed in whole or in part or used for
any purpose except when the user possesses direct, written authorization
from The Boeing Company.

Document Information

+-----------+-----------+-----------+-----------+-----------+-----------+
| **Documen | **Origina | **Contrac |           |           |           |
| t         | l         | t         |           |           |           |
| Type**    | Release   | Number    |           |           |           |
|           | Date**    | (if       |           |           |           |
| Formal    |           | required) |           |           |           |
|           |           | **        |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| **Prepari | **Hardwar |           |           |           |           |
| ng        | e         |           |           |           |           |
| Organizat | and       |           |           |           |           |
| ion       | Software  |           |           |           |           |
| (if       | Used**    |           |           |           |           |
| different |           |           |           |           |           |
| from      | IBM PC    |           |           |           |           |
| owning    | Microsoft |           |           |           |           |
| organizat | Word 2003 |           |           |           |           |
| ion)**    |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| **Locatio |           |           |           |           |           |
| n         |           |           |           |           |           |
| of        |           |           |           |           |           |
| Software  |           |           |           |           |           |
| Files     |           |           |           |           |           |
| (optional |           |           |           |           |           |
| )**       |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| **Boeing  |           |           |           |           |           |
| Web URL   |           |           |           |           |           |
| (optional |           |           |           |           |           |
| )**       |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| **Notes   |           |           |           |           |           |
| and       |           |           |           |           |           |
| Limitatio |           |           |           |           |           |
| ns        |           |           |           |           |           |
| (optional |           |           |           |           |           |
| )**       |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| **Signatu |           |           |           |           |           |
| res       |           |           |           |           |           |
| for       |           |           |           |           |           |
| original  |           |           |           |           |           |
| release** |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| AUTHOR:   |           |           | 66-CB-E42 |           | Mar. 8,   |
|           |           |           | 1         |           | 2013      |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           | Mary-Ann  |           | Org.      |           | Date      |
|           | Micale    |           | Number    |           |           |
|           | *(Signatu |           |           |           |           |
|           | re        |           |           |           |           |
|           | on file)* |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| AUTHOR:   |           |           | 66-CB-E42 |           | 3/8/2013  |
|           |           |           | 1         |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           | Guillermo |           | Org.      |           | Date      |
|           | De Vivero |           | Number    |           |           |
|           | *(Signatu |           |           |           |           |
|           | re        |           |           |           |           |
|           | on file)* |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| REVIEWED  |           |           | 66-CB-E42 |           | Mar. 8,   |
| BY:       |           |           | 1         |           | 2013      |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           | Steve     |           | Org.      |           | Date      |
|           | Diehl     |           | Number    |           |           |
|           | *(Signatu |           |           |           |           |
|           | re        |           |           |           |           |
|           | on file)* |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| REVIEWED  |           |           | 66-CH-R62 |           | 3/8/2013  |
| BY:       |           |           | 4         |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           | Cynthia   |           | Org.      |           | Date      |
|           | McGrath   |           | Number    |           |           |
|           | *(Signatu |           |           |           |           |
|           | re        |           |           |           |           |
|           | on file)* |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| REVIEWED  |           |           | 66-CB-E42 |           | Mar. 8,   |
| BY:       |           |           | 1         |           | 2013      |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           | Martin    |           | Org.      |           | Date      |
|           | Moy       |           | Number    |           |           |
|           | *(Signatu |           |           |           |           |
|           | re        |           |           |           |           |
|           | on file)* |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| REVIEWED  |           |           | 66-CB-E42 |           | Mar. 8,   |
| BY:       |           |           | 1         |           | 2013      |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           | Steve St. |           | Org.      |           | Date      |
|           | Onge      |           | Number    |           |           |
|           | *(Signatu |           |           |           |           |
|           | re        |           |           |           |           |
|           | on file)* |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| APPROVAL: |           |           | 66-CH-R62 |           | 3/8/2013  |
|           |           |           | 4         |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           | Steve     |           | Org.      |           | Date      |
|           | McGinnis  |           | Number    |           |           |
|           | *(Signatu |           |           |           |           |
|           | re        |           |           |           |           |
|           | on file)* |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| APPROVAL: |           |           | 66-CB-E40 |           | 3/11/13   |
|           |           |           | 1         |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           | Mark      |           | Org.      |           | Date      |
|           | Calkins   |           | Number    |           |           |
|           | *(Signatu |           |           |           |           |
|           | re        |           |           |           |           |
|           | on file)* |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| DOCUMENT  |           |           |           |           |           |
| RELEASE:  |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           |           |           | Org.      |           | Date      |
|           |           |           | Number    |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
|           |           |           |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+

**Copyright © 2000 The Boeing Company**

\
Table of Contents

[1.0 Introduction 8](#introduction)

[1.1 Purpose 8](#purpose)

[2.0 General Information 10](#general-information)

[2.1 CDG Core Tool versus ACDG Tool Description
10](#cdg-core-tool-versus-acdg-tool-description)

[2.2 ACDG Tool Overview 12](#acdg-tool-overview)

[2.2.1 ACDG Host 13](#acdg-host)

[2.2.2 ACDG Plug-In 13](#acdg-plug-in)

[2.2.3 External Files 14](#external-files)

[2.3 Document Structure 14](#document-structure)

[3.0 General ACDG Host Requirements 16](#general-acdg-host-requirements)

[3.1 Part Number 16](#part-number)

[3.2 Installation Procedures 16](#installation-procedures)

[3.3 Execution 16](#execution)

[3.4 Operation 16](#operation)

[3.5 Screen Display 17](#screen-display)

[3.6 Components 18](#components)

[3.7 Characteristics/Performance 18](#characteristicsperformance)

[3.8 Load Database Information 19](#load-database-information)

[3.9 PC File Data 19](#pc-file-data)

[3.10 File Management 20](#file-management)

[3.11 Plug-In Interface 20](#plug-in-interface)

[3.12 Plug-In Management 21](#plug-in-management)

[3.13 Keyboard 21](#keyboard)

[3.14 Mouse 21](#mouse)

[3.15 Menu Bar 21](#menu-bar)

[3.16 Data Protection 21](#data-protection)

[3.17 Status Screens 22](#status-screens)

[4.0 Host Screen Requirements 23](#host-screen-requirements)

[4.1 Primary Screen 23](#primary-screen)

[4.2 Sub-Screens 28](#sub-screens)

[4.2.1 File New Screen 28](#file-new-screen)

[4.2.2 File Open Screen 30](#file-open-screen)

[4.2.3 File Save Screen 30](#file-save-screen)

[4.2.4 File SaveAs Screen 30](#file-saveas-screen)

[4.2.5 Configuration Information Screen
32](#configuration-information-screen)

[4.2.6 Plug-In Packages Screen 33](#plug-in-packages-screen)

[4.2.7 Build LSAP Screen 36](#build-lsap-screen)

[4.2.8 Compress Plug-In Package Screen
36](#compress-plug-in-package-screen)

[4.2.9 Import XML Screen 38](#import-xml-screen)

[4.2.10 Export XML Screen 38](#export-xml-screen)

[4.2.11 SDT Conversion Screen 39](#sdt-conversion-screen)

[4.2.12 CDB Consistency Check Screen 39](#cdb-consistency-check-screen)

[4.2.13 Export CDB 40](#export-cdb)

[4.2.14 Help ACDG Screen 40](#help-acdg-screen)

[4.2.15 About ACDG Screen 41](#about-acdg-screen)

[5.0 ACDG Host Screen Error/Warning Dialog Box
42](#acdg-host-screen-errorwarning-dialog-box)

[5.1 ACDG Host Primary Screen 42](#acdg-host-primary-screen)

[6.0 ACDG Host Data Flow Requirements
43](#acdg-host-data-flow-requirements)

[6.1 ACDG Host Primary Screen 43](#acdg-host-primary-screen-1)

[Glossary 52](#glossary)

[References 53](#references)

[Revision Record 54](#revision-record)

[Revision Record 55](#revision-record-1)

List of Figures

[Figure 1.1-1: Documents in Support of the ACDG Tool 9](#_Toc395021793)

[Figure 2.1-1: CDG Core Tool Architecture 11](#_Toc395021794)

[Figure 2.1-2: ACDG Tool Architecture 12](#_Toc395021795)

[Figure 6.0-1: Data Flow Diagram Legend 43](#_Toc395021796)

[Figure 6.1-1: ACDG Host Primary Screen -- File New 44](#_Toc395021797)

[Figure 6.1-2: ACDG Host Primary Screen -- File Open 45](#_Toc395021798)

[Figure 6.1-3: ACDG Host Primary Screen -- File Save 46](#_Toc395021799)

[Figure 6.1-4: ACDG Host Primary Screen -- File Save As
47](#_Toc395021800)

[Figure 6.1-5: ACDG Host Primary Screen -- File Config Info
47](#_Toc395021801)

[Figure 6.1-6: ACDG Host Primary Screen -- File Close
48](#_Toc395021802)

[Figure 6.1-7: ACDG Host Primary Screen -- Exit 49](#_Toc395021803)

[Figure 6.1-8: ACDG Host Primary Screen -- Import XML
50](#_Toc395021804)

[Figure 6.1-9: ACDG Host Tool Primary Screen -- Build LSAP Files
51](#_Toc395021805)

List of Tables

[Table 3.7-1: Performance Times 19](#_Toc395021806)

[Table 4.1-1: ACDG Host Primary Screen -- Components 24](#_Toc395021807)

[Table 4.1-2: ACDG Host Primary Screen -- Menu Tree 25](#_Toc322617781)

[Table 4.1-3: ACDG Host Tool Primary Screen - Behavior
26](#_Toc322618041)

[Table 4.1-4: ACDG Host Primary Screen - Operation Checks
27](#_Toc395021810)

[Table 4.2.1-1: File New Screen - Components 28](#_Hlt122159022)

[Table 4.2.1-2: File New Load Part Number Screen 29](#_Toc346888981)

[Table 4.2.4-1: File SaveAs Screen - Components 31](#_Toc395021813)

[Table 4.2.5-1: Config Info Screen - Components 32](#_Toc395021814)

[Table 4.2.6-1: Plug-In Packages Screen - Components 33](#_Toc395021815)

[Table 4.2.6-2: Plug-In Packages Screens - Behavior 35](#_Toc395021816)

[Table 4.2.6-3: Plug-In Compatibility Matrix Table 35](#_Toc395021817)

[Table 4.2.8-1: Compress Plug-In Package Screen - Components
36](#_Toc395021818)

[Table 4.2.15-1: About ACDG Screen - Components 41](#_Toc395021819)

[Table 5.1-1: Screen Generated Error/Warning Dialog Boxes
42](#_Toc336344533)

Abstract

The Cabin Services System (CSS) for the 787 and 747 airplanes uses two
types of databases to define its functionality and its configuration:
the Health Management Database (HDB) and the Configuration Database
(CDB). The Airline Configuration Database Generator (ACDG ) Tool builds
CDBs and is intended for use by both Boeing and the airlines. The ACDG
Tool comprises the ACDG Host and the ACDG Plug-In. The ACDG Host is the
application which allows the ACDG Plug-In to be used. This document
defines the requirements for the ACDG Host.

1.0 Introduction
================

The Cabin Services System (CSS) for the 787 and 747 airplanes uses two
types of databases to define its functionality and its configuration:
The Health Management Database (HDB) and the Configuration Database
(CDB). The HDB identifies the available screens for the CAPs, defines
cabin functionality, and provides health management information for the
LRUs and peripherals. The CDB is used to build a custom database to
match the airline-unique interior configuration using the functions
defined by the HDB and the Operational Program Software (OPS) installed
in the CSS.

There are two tools available for building the two types of databases.
The first tool is the Configuration Database Generator (CDG) Core Tool.
Provided by Panasonic, the CDG Core Tool gives the user the ability to
build both HDB Loadable Software Airplane Parts (LSAPs) and CDB LSAPs.
The CDG Core Tool is intended for the sole use of Pansonic and Boeing.
Although Boeing has access to the CDG, only Panasonic can modify the
tool itself. The second tool is the Airline Configuration Database
Generator (ACDG) Tool, which is provided by Boeing and which allows the
user to only build CDB LSAPs. The ACDG Tool is intended for use by both
Boeing and the Airlines.

1.1 Purpose 
------------

The ACDG Tool comprises the ACDG Host and the ACDG Plug-In. The ACDG
Host is the application which allows the ACDG Plug-In to be used. The
ACDG Plug-In performs the following functions: Editor, Consistency
Checker, Converter, Report Generator, Importer/Exporter, and Updater.
Included with the ACDG Plug-In is supporting data, such as default data
and library data. The various documents which support the ACDG Tool are
shown in Figure 1.1-1.

The System Data Tables (SDTs) are in the SDT ICD, D620Z012-20. The SDT
ICD defines the system data tables and data ranges as well as the schema
used for importing and exporting data to and from the ACDG Tool.

This document describes the requirements for the ACDG Host. In general,
the requirements for the ACDG Host apply to both the 747 and the 787
models. Note, however, that until the 787 CSS has implemented the ACDG
Host, this document is primarily for the 747 CSS. The applicability of
the requirements to the 787 will be reviewed and updated in future
releases of this document.

[]{#_Toc395021793 .anchor}Figure 1.1-1: Documents in Support of the ACDG
Tool

The following terminology defines the applicability of each provision in
this document:

a\. \'shall\' is used to express a requirement that is binding on the
supplier.

b\. \'will\' is used to express a declaration of intent.

c\. \'should\' and \'may\' are used to express recommended or allowed
actions.

2.0 General Information
=======================

2.1 CDG Core Tool versus ACDG Tool Description
----------------------------------------------

The elements of the CDG Core Tool, which is a ground support engineering
software tool built by Panasonic, are shown in Figure 2.1-1. This tool
contains HDB Tables and CDB Tables, which are used to build HDB LSAPs
and CDB LSAPs.

Figure 2.1-2 illustrates the elements of the ACDG Tool. The ACDG Tool,
built by Boeing, is a ground support engineering software tool which
will be used to build CDB LSAPs. The ACDG Tool also contains
Panasonic-supplied software. The Panasonic software performs consistency
checks on the CDB Tables, builds CDB LSAPs, and exports CDB CSV files.

There are two main table structures which make up the ACDG Tool:

a\. Tables based on the SDT ICD (SDTs)

> The SDTs contain high level physical and functional configuration
> data. They are used to generate the lower level CDB Tables.

b\. CDB Tables

> The CDB Tables in the ACDG Tool are identical to the CDB Tables in the
> CDG Core Tool. These tables are used by both the CDG Core Tool and the
> ACDG Tool to generate CDB LSAPs. The structure of the CDB Tables is
> controlled by Panasonic. If any changes are made to the table
> structure in the CDG Core Tool, then Panasonic will need to supply
> Boeing with updated software for the ACDG Tool.

The Editor, Report Generator, Importer/Exporter, and Consistency Checker
functions all operate at the data level defined in the SDT ICD. The
Converter translates the data from the SDT ICD level to the CDB Tables
level (CSV files).

[]{#_Toc395021794 .anchor}Figure 2.1-1: CDG Core Tool Architecture

![](media/image4.png){width="6.283333333333333in"
height="5.641666666666667in"}

[]{#_Toc395021795 .anchor}Figure 2.1-2: ACDG Tool Architecture

ACDG Tool Overview
------------------

The ACDG Tool is made up of the ACDG Host and ACDG Plug-In. The Host,
which should seldom change, represents the platform for executing the
Plug-In. The Plug-In is designed to be flexible so that it can allow the
user to configure a CDB which incorporates new functionality made in the
HDB. The Host allows the user to manage the Plug-In, including the
loading of the Plug-In itself into the ACDG Tool.

The Plug-In allows Boeing to make updates to the Editor, Consistency
Checker, Importer/Exporter, Report Generator, Converter, and Updater as
well as provide the ability to up-convert data from previous data files.

### ACDG Host

The ACDG Host allows access to the functions and features of the
Plug-In. The ACDG Host is comprised of the following elements:

1\. File Management

> Manages the database files used for building configuration databases.

2\. Plug-In Compressor

> Builds a Plug-In package, which is comprised of all the Plug-In
> functions (i.e., Editor, Reporter, Consistency Checker, etc.).

3\. Plug-In Loader

> Loads the Plug-In to be used with the Host.

4\. SDTs

> Contain the configuration information.

5\. CDB LSAP Generator

> Builds LSAP files from the data contained in CDB Tables using
> Panasonic-supplied software.

6\. CDB Consistency Checker

> Performs data validation at the CDB Table level (i.e., Panasonic
> defined Tables). (This is Panasonic-supplied software).

7\. CDB Tables

> Contains low level configuration data used to build CDB LSAPs. The
> structure of the tables is defined by Panasonic.

8\. CSV Exporter

> Exports CDB CSV files using Panasonic-supplied software.

9\. Help

> Provides Help screens for using the ACDG Tool.

### 2.2.2 ACDG Plug-In

The ACDG Plug-In is composed of the following functions, which utilizes
data from the SDTs.

1\. Editor

> Provides PC-based screens for entering/editing data for the purpose of
> constructing a CDB.

2\. Consistency Checker (SDT)

> Performs integrity and consistency checks on the data entered into the
> ACDG Tool.

3\. Report Generator

> Allows the user to prepare two types of reports: CDB Reports, which
> detail what is configured in a CDB, and Difference Reports, which
> compare the differences between two CDBs.

4\. Converter

> Transforms and distributes the high level physical and functional
> cabin configuration data (i.e., SDT level) to lower level CDB Tables
> (i.e., Panasonic CSV level data). The CDB tables are used to build the
> CDB LSAP.

5\. Importer/Exporter

> Allows the user to directly import configuration data from XML files
> (per the SDT ICD) for use by the ACDG Tool. It also allows the user to
> export the configuration data from the ACDG Tool into XML files. The
> purpose of the Importer/Exporter function is to reduce the amount of
> time required to enter data in a production environment.

6\. Updater

> Automatically modifies older database (that is, PC) files and imports
> XML files so that they can be compatible with the current ACDG
> Plug-In.

7\. Default Data

> Defines the minimal data required for the Editor, Report Generator,
> and Converter to start building a database.

8\. Library Data

> Provides a single source for data which is used across multiple
> functions (e.g., Converter, Report Generator, Editor).

### 2.2.3 External Files

1\. PC Files

> Contains all the data needed to build an LSAP.

2\. XML Zip Files

> Contains the XML files in a zip file format. These files have the
> configuration data which is used in the SDTs.

3\. Plug-In Package

> Contains the software which the Host uses for executing the Plug-In
> functions.

4\. License File

Contains license file \*TBD\*

2.3 Document Structure 
-----------------------

The ACDG Host provides a Graphics User Interface (GUI) which is used to
access the different functions provided in the ACDG Plug-In. It also
provides file management capability for the files being used to revise
or build configuration databases. The ACDG Tool is used for building or
revising the configuration databases and is not loaded on the airplane.

The requirements in this document are organized as follows:

Section 3: General ACDG Host Requirements.

Section 4: Specific Screen Requirements for the GUI.

Section 5: GUI Screen Error and Warning Dialog Boxes.

Section 6: ACDG Host Data Flow Requirements.

3.0 General ACDG Host Requirements
==================================

3.1 Part Number
---------------

a\. ~~The Part Number shall have the following characteristics:~~

> ~~1. At least 1 character~~
>
> ~~2. No more than 16 characters~~

b\. The Boeing and Airline versions shall each be assigned a unique Part
Number.

> 1\. The Boeing Part Number shall be 620Z012-09B.
>
> 2\. The Airline Part Number shall be 620Z012-09A.

c\. The ACDG Host shall pass its Part Number^1^ (as identified in items
b-1 and b-2) above and its version number to the Panasonic DLL during
the Build LSAP process.

d\. The version number shall be per the following format
(major.minor.build.release):

-   *major* is the major release version

-   *minor* is the minor release version

-   *build* is a number that denotes the number of builds that were
    performed

> *release* is the release of that version (typically bugfixes will
> increment this)Note 1: Currently, the part number is reference-only
> information that is used in the Panasonic release notes file.

3.2 Installation Procedures
---------------------------

~~a. An automatic installation procedure shall be provided for the Host
software.~~

### 3.2.1 Software Build Procedures

a\. The ACDG shall be built into the following installation packages:

1\. A Boeing only installation package

2\. An Airline installation package

b\. The Boeing only installation package shall contain all available ACDG
Functions and Features without restriction or licensing.

Note: Licensing is not necessary on a Boeing controlled tool

c\. The Airline installation package shall contain a Boeing defined
subset of available ACDG Functions and Features

### 3.2.2 Software Installation Procedures

a\. The ACDG installation procedure shall automate the extraction and
installation of software components from the installation package to a
users machine

Note: Automate means to perform without any user action. In this case a
user will not extract or copy any required files themselves

a\. The ACDG installation procedure shall allow for user selection of
installation location

b\. The ACDG installation procedure shall package any required external
libraries into the installer to be installed on the users machine as
part of the automated installation process

~~b. The installer shall provide separate installer keys, one for Boeing
and one for the Airlines. See the CSS ACDG Design Group for the specific
installer keys.~~

3.3 Execution
-------------

~~a. The Host software shall run on Windows 10. ~~

~~b. The Host software shall not require special (non-standard)
equipment for operation. ~~

~~Note: non-standard equipment includes external software applications~~
~~and tools~~

a\. The Host software shall execute on the following software
environment:

1\. Windows Operating System with .NET Framework v4.6 minimum

2\. Panasonic DLL's environmental requirements as Defined in 810006-301

b\. The Host software shall execute within the following hardware
environment:

1\. 64-bit x86 CPU architecture

The Host software shall be self-contained, relying only on libraries and
runtimes installed and managed with the Host.

~~c. The Host software ***shall*** be capable of running as a 32 bit
application.~~

~~d. Supporting software used by the Host shall support 32 bit
operations.~~

~~Note: This includes Dynamic Linked Libraries (DLLs) used by the
Host.~~

~~e. The underlying database application that the Host is built upon
shall support 32 bit operations.~~

~~f. (Delete)~~

3.4 Operation
-------------

a\. The Host shall be invoked with a single command.

b\. The Host functions shall be invoked from a menu.

c\. (Deleted)

d\. The Host shall use "pull-down" menus for all operations and menu
selections.

e\. The ACDG Host Primary Screen File New shall operate as defined in
Figure 6.1-1.

f\. The ACDG Host Primary Screen File Open shall operate as defined in
Figure 6.1-2.

g\. The ACDG Host Primary Screen File Save shall operate per Figure
6.1-3.

h\. The ACDG Host Primary Screen File Save As shall operate per Figure
6.1-4.

i\. The ACDG Host Primary Screen Config Info shall operate per Figure
6.1-5.

j\. The ACDG Host Primary Screen File Close shall operate per Figure
6.1-6.

k\. The ACDG Host Primary Screen Exit shall operate per Figure 6.1-7.

l\. The ACDG Host Primary Screen Import XML shall operate per Figure
6.1-8.

m\. The ACDG Host Primary Screen Build LSAP Files shall operate per
Figure 6.1-9.

n\. The Default Starting Path for the following screens shall be \"My
Documents\":\
4.2.2 File Open Screen\
4.2.3 File Save Screen\
4.2.4 File SaveAs Screen\
4.2.6 Plug-In Packages Screen\
4.2.9 Import XML Screen\
4.2.10 Export XML Screen\
4.2.11 SDT Conversion Screen\
4.2.13 Export CDB

3.5 Screen Display
------------------

a\. (Deleted)

b\. (Deleted)

c\. The following ACDG Host screens shall be modal:

> 1\. Plug-In Loader
>
> 2\. Import XML
>
> 3\. Export XML
>
> 4\. SDT Conversion
>
> 5\. CDB Consistency Check
>
> 6\. Export CDB CSV Files
>
> 7\. Compress Plug-In Package

d\. Each Host screen or window shall have a Title Bar at the top.

1.  All screens shall have the ACDG Logo and the word ACDG on the Title
    Bar; unless otherwise stated in Section 4

2.  The Editor (GUI) screens' Tile Bar shall also include the following:

-   The PC File Name and the PC File Revision Number. For example,
    CDB44-0000-0001 (R003).

e\. The Host screens shall allow a user to construct a complete
Configuration Database using only the keyboard, without requiring the
use of a mouse or other equivalent pointing devices. See Paragraph 3.12
for keyboard requirements.

3.6 Components
--------------

The following items shall be elements of the Host Tool:

a\. File Management

b\. CDB LSAP Generator

c\. SDT to CSV Converter

d\. CSV Exporter

e\. Help Screens

f\. Selection/execution of the Plug-In package, which includes the
following Plug-Ins:

1\. XML File Importer/Exporter

2\. Consistency Checker (SDT)

3\. Editor

4\. Report/Difference Report Generator

5\. Converter

g\. CDB Consistency Checker

h\. Plug-In Compressor

3.7 Characteristics/Performance 
--------------------------------

a.. The Host shall build a 665-3 compliant part in no more than 5
minutes.

b\. The Host shall be able to perform the following within the times
listed in Table 3.7-1, based on a typical production airplane
configuration.

[]{#_Toc395021806 .anchor}Table 3.7-1: Performance Times

  **Function**                          **Time (Seconds)^1^**
  ------------------------------------- -----------------------
  File open/close                       30
  File save                             30
  Import/export system tables           60
  Convert system table versions         120
  Consistency check system tables       60
  Configuration report (all sections)   60
  Difference report (all sections)      150

> Notes:
>
> 1\. The times listed above are based on the minimum processor performance
> of Intel® Core-i5® 2520 M processor, 2.5Ghz, 4.00GB of RAM.

3.8 Load Database Information
-----------------------------

a\. Loading a new .PC file shall clear all information from the previous
database (i.e., SDT and CDB table data).

b\. Importing a XML file shall be per D620Z012-17, Table 3.2-1, item 9.

3.9 PC File Data
----------------

a\. The PC file shall contain all the data needed to build an LSAP.

b\. The PC file shall contain the consistency check status.

c\. The PC file shall contain the SDT IVN level.

d\. The PC file shall contain the Plug-In IVN.

e\. The PC file shall contain the database description.

f\. The PC file shall contain the release notes.

g\. The PC file shall identify the airplane model.

h\. The PC file shall contain the ARINC 665-3 LSAP part number.

i\. The PC file shall contain the date/time stamp of when the database
edits were last accepted.

j\. The PC file shall contain a Revision Number.

> 1\. The PC file Revision Number shall start at 1.
>
> 2\. The PC file Revision Number shall increment when data has been
> changed and saved.

k\. The PC file shall contain the Host ACDG Part Number and Version
Number.

l\. The PC file shall contain the Panasonic CDG Tool Part Number

m\. The PC file shall contain the current Plug-in Part Number and Plug-in
Version Number

n\. The ACDG shall update the Tool and Plug-In Part Numbers and Version
Number in the PC file (as identified in items k, l and m) per the
following conditions:

> 1\. Data has changed and Save has been executed.
>
> 2\. Data has been Imported and Save has been executed.
>
> 3\. Save As has been executed.

3.10 File Management
--------------------

a\. The Host shall have a File Management feature with the following
functions: File New, File Open, File Save, File Save As; Config Info,
File Close, and Exit.

b\. The Host shall provide the ability to build a Red Label/Black Label
part number or a Blue Label part number.

c\. The ARINC 665-3 LSAP part number shall default to the Red Label/Black
Label part number.

d\. The PC file name shall

1\. be the corresponding ARINC 665-3 LSAP part number.

2\. have a .pc extension.

3.11 Plug-In Interface
----------------------

a\. The Host shall be able to interface with a Plug-In which incorporates
the intent of the following documents:

1\. D620Z012-13 Cabin Services System (CSS) Airline Configuration
Database Generator (ACDG) Plug-In Requirements: Editor

2\. D620Z012-14 Cabin Services System (CSS) Airline Configuration
Database Generator (ACDG) Plug-In Requirements: Consistency Checker

3\. D620Z012-15 Cabin Services System (CSS) Airline Configuration
Database Generator (ACDG) Plug-In Requirements: Converter

4\. D620Z012-16 Cabin Services System (CSS) Airline Configuration
Database Generator (ACDG) Plug-In Requirements: Report Generator

5\. D620Z012-17 Cabin Services System (CSS) Airline Configuration
Database Generator (ACDG) Plug-In Requirements: Importer/Exporter

6\. D620Z012-19 Cabin Services System (CSS) Airline Configuration
Database Generator (ACDG) Plug-In Requirements: Updater

b\. The Host shall perform software Integrity of the Plug-In each time

> 1\. a Plug-In is added.
>
> 2\. a Plug-In is selected
>
> 3\. the ACDG Tool is started.

3.12 Plug-In Management
-----------------------

a\. The Host shall provide the following items for Plug-In Management:

1\. Add a plug-in

2\. Select a plug-in

3\. Delete a plug-in

4 Model Selector

a\) The Model Selector shall contain the following models: 747-8, 787 and
777.

3.13 Keyboard
-------------

a\. The Host screen shall allow navigation of Host elements using only
the keyboard, without requiring the use of a mouse or other equivalent
pointing devices.

> 1\. The Host shall use standard Windows short-cut keys (Ctrl+Keyboard)
> (e.g., Ctrl-C, Ctrl-V, etc.) and navigation keys (e.g., PgUp, PgDn,
> etc.).
>
> a\) Selected lower level menu commands shall be able to be invoked with
> short-cut keys.

2 All data entry fields and buttons shall be accessible with the Tab key
and appropriate arrow keys.

3\. Accessing fields with the Tab key shall not alter the value contained
in the field.

3.14 Mouse
----------

a\. The ACDG screen shall support mouse input where appropriate (e.g.,
check box and list box selection).

b\. The ACDG screen shall support selection of field text with a mouse.

1\. The left mouse button shall always select or invoke the windows
object pointed to by the mouse pointer when clicked.

3.15 Menu Bar
-------------

a\. The ACDG screen shall display a single menu bar to allow the user to
invoke commands from the keyboard or mouse.

1\. The top level menu commands shall be actuated by toggling the \"Alt\"
key and pressing the appropriate access key shown as an underlined
letter in the menu bar.

2\. Lower level menu items shall be accessible with access keys or by
using the keyboard arrow keys.

3.16 Data Protection
--------------------

~~a. Any underlying tables/databases used to store database information
shall be password protected. ~~

a\. Underlying data storage mechanisms shall allow access to only the
ACDG Tool and users with special administrative permissions

3.17 Status Screens
-------------------

a\. The Status Screen shall have the following characteristics:

1\. The Status Screen shall have a Title Label.

2\. The Status Screen shall have a scrolling message box.

3\. The Status Screen shall have a progression bar that indicates how
much of the current task is completed and how much more there is to
complete.

4\. The Status Screen shall have a View button.

5\. The Status Screen shall have a Save button.

6\. The Status Screen shall have a Print button.

7\. The Status Screen shall have a Cancel/Close button.

b\. The Status Screen will be used for the following menu options. Refer
to reference documents for screen behavior.

1\. IVN Update (D620Z012-19)

2\. Consistency Check (D620Z012-14)

3\. SDT Conversion (D620Z012-15)

4\. Import XML (D620Z012-17)

5\. Export XML (D620Z012-17) NOTE: For Export XML only the Cancel/Close
button will exists.

6\. Export CDB CSV (Section 4.2.13 in this document) NOTE: For Export CDB
CSV Files only the Cancel/Close button will exists.

3.18 External Libraries
-----------------------

a\. The ACDG host shall interface with the Panasonic supplied DLLs as
defined in the 810006-301, INTERFACE CONTROL DOCUMENT for Configuration
Database Generator.

b\. The ACDG Host shall interface with a Boeing licensing tool via a
software library as defined in TBDXXX -- need to create an interface
document (TBD)

3.19 Tool Licensing (TBD -- Provisioned)
----------------------------------------

There is a growing need for the ability to have an airline customer
configure their own database. In order to support Boeing's business
need, the tool will be available as a licensed option. This means that
Boeing needs to control and track the usage of the ACDG tool.

Since CSS is a very flexible system, allowing some customers the usage
of options not available to others, the tool will need to reflect the
configuration of the customers airplanes. For example, the customer
cannot configure an option they have not paid for in the tool.

In order to support the ability to manage the ACDG tool outside the
Boeing company, a feature to support accepting and managing customer
licenses will be added. This includes obtaining a new licenses, updating
an old one and removing/invalidating a license. These capabilities must
be done in a secure and reliable manner, ensuring the information in the
license cannot be compromised or faked.

Note: The licensing feature only applies to the Airline version of the
tool. The Boeing tool will not contain the licensing feature as all
features will be available.

In order to keep the ACDG Tool focused on it's job of creating
databases, a separate licensing tool will be used to manage and control
licenses of Boeing software. This tool also allows the flexibility of
managing multiple Boeing provided tools.

~~The ACDG Tool shall interface with a Boeing licensing tool via a
software library as defined in TBDXXX -- need to create an interface
document~~

Th ACDG Tool shall establish communication with the license tool on
application launch

If communication is not detected between ACDG and the license tool the
ACDG host shall display an appropriate error message in an ACDG pop-up
window

The ACDG Tool shall utilize information provided by the license tool to
determine if the ACDG application is allowed to launch

The ACDG Tool shall utlize information provided from the license tool to
determine which ACDG Functions the user will be allowed to access

If an ACDG Function or Feature is not allowed access to a specific user
ACDG shall prevent a user from accessing the feature and hide it from
the users view

4.0 Host Screen Requirements
============================

The requirements for the Primary Screen (that is, top level screen) of
the Host are described in Section 4.1. This menu structure allows the
user to navigate to the desired features of the Host. The underlined
letter in a menu name defines the applicable hot key. With hot keys, it
is possible to navigate the GUI screens without having to use a mouse.
To use a hot key, the user first needs to select the Alt button on the
keyboard and then select the applicable hot key letter.

The requirements for the sub-screens and windows which are called from
the Host screen are described in Section 4.2.

4.1 Primary Screen
------------------

The Primary Screen of the Host provides the basic menu selection for all
the available features used in building a CDB. These features include
the ability to perform file management, modify databases, generate
reports, run consistency checks, build LSAPs, and select plug-in
packages.

This screen allows the user to navigate to different features of the
Plug-In. Based on what has been loaded into the Host, some menu items
will not be available. For example, if a plug-in has not been loaded
into the tool, then the user will not be allowed to select the menu
items File/Open or File/New.

**Requirements:**

a\. The ACDG Host Primary Screen controls shall be as defined in Table
4.1-1.

b\. The ACDG Host Primary Screen File Menu Tree shall be as defined in
Table 4.1-2.

c\. The behavior of the ACDG Host Primary Screen shall be per Table
4.1-3.

d The operation checks for the ACDG Host Primary Screen shall be per
Table 4.1-4.

[]{#_Toc395021807 .anchor}Table 4.1-1: ACDG Host Primary Screen --
Components

+--------+--------+--------+--------+--------+--------+--------+--------+
| **Item | **Labe | **Type | **Rang | **Deta | **Avai | > **Ta | **Mode |
| \#**   | l**    | **     | e**    | ils**  | labili | b      | l      |
|        |        |        |        |        | ty**   | > Orde | Unique |
|        |        |        |        |        |        | r**    | **     |
+========+========+========+========+========+========+========+========+
|        |        |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 1      | [F]{.u | Menu   | See    |        | Always | 1      |        |
|        | nderli |        | Table  |        | enable |        |        |
|        | ne}ile |        | 4.1-2  |        | d.     |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| **2**  | **[D]{ | Menu   | See    |        | Enable | 2      |        |
|        | .under |        | Table  |        | d      |        |        |
|        | line}a |        | 4.1-2  |        | only   |        |        |
|        | ta**   |        |        |        | when a |        |        |
|        |        |        |        |        | databa |        |        |
|        |        |        |        |        | se     |        |        |
|        |        |        |        |        | has    |        |        |
|        |        |        |        |        | been   |        |        |
|        |        |        |        |        | loaded |        |        |
|        |        |        |        |        | .      |        |        |
|        |        |        |        |        |        |        |        |
|        |        |        |        |        | Otherw |        |        |
|        |        |        |        |        | ise,   |        |        |
|        |        |        |        |        | always |        |        |
|        |        |        |        |        | visibl |        |        |
|        |        |        |        |        | e,     |        |        |
|        |        |        |        |        | not    |        |        |
|        |        |        |        |        | select |        |        |
|        |        |        |        |        | able.  |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| **3**  | **[R]{ | Menu   | See    |        | Enable | 3      |        |
|        | .under |        | Table  |        | d      |        |        |
|        | line}e |        | 4.1-2  |        | when a |        |        |
|        | port** |        |        |        | Plug-i |        |        |
|        |        |        |        |        | n      |        |        |
|        |        |        |        |        | has    |        |        |
|        |        |        |        |        | been   |        |        |
|        |        |        |        |        | select |        |        |
|        |        |        |        |        | ed.    |        |        |
|        |        |        |        |        |        |        |        |
|        |        |        |        |        | Otherw |        |        |
|        |        |        |        |        | ise,   |        |        |
|        |        |        |        |        | always |        |        |
|        |        |        |        |        | visibl |        |        |
|        |        |        |        |        | e,     |        |        |
|        |        |        |        |        | not    |        |        |
|        |        |        |        |        | select |        |        |
|        |        |        |        |        | able.  |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| **4**  | **[U]{ | Menu   | See    |        | Always | 4      |        |
|        | .under |        | Table  |        | enable |        |        |
|        | line}t |        | 4.1-2  |        | d.     |        |        |
|        | ilitie |        |        |        |        |        |        |
|        | s**    |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| **5**  | **[A]{ | Menu   | See    |        | With   | 5      |        |
|        | .under |        | Table  |        | Boeing |        |        |
|        | line}d |        | 4.1-2  |        | ACDG   |        |        |
|        | vanced |        |        |        | Host,  |        |        |
|        | **     |        |        |        | always |        |        |
|        |        |        |        |        | enable |        |        |
|        |        |        |        |        | d.     |        |        |
|        |        |        |        |        |        |        |        |
|        |        |        |        |        | With   |        |        |
|        |        |        |        |        | Airlin |        |        |
|        |        |        |        |        | e      |        |        |
|        |        |        |        |        | ACDG   |        |        |
|        |        |        |        |        | Host,  |        |        |
|        |        |        |        |        | not    |        |        |
|        |        |        |        |        | visibl |        |        |
|        |        |        |        |        | e.     |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| **6**  | **[H]{ | Menu   |        |        | Always | 6      |        |
|        | .under |        |        |        | enable |        |        |
|        | line}e |        |        |        | d.     |        |        |
|        | lp**   |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| **7**  | **Load | Label  |        |        | Always | N/A    |        |
|        | Part   |        |        |        | visibl |        |        |
|        | Number |        |        |        | e,     |        |        |
|        | **     |        |        |        | not    |        |        |
|        |        |        |        |        | editab |        |        |
|        |        |        |        |        | le.    |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| **8**  |        | TextBo |        | **Part | Visibl | N/A    |        |
|        |        | x      |        | Number | e      |        |        |
|        |        |        |        | of the | only   |        |        |
|        |        |        |        | databa | when a |        |        |
|        |        |        |        | se**   | PC     |        |        |
|        |        |        |        |        | file   |        |        |
|        |        |        |        |        | has    |        |        |
|        |        |        |        |        | been   |        |        |
|        |        |        |        |        | loaded |        |        |
|        |        |        |        |        | ,      |        |        |
|        |        |        |        |        | not    |        |        |
|        |        |        |        |        | editab |        |        |
|        |        |        |        |        | le.    |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| **9**  |        | TextBo |        | **PC   | Visibl | N/A    |        |
|        |        | x      |        | File   | e      |        |        |
|        |        |        |        | Revisi | only   |        |        |
|        |        |        |        | on     | when a |        |        |
|        |        |        |        | Number | PC     |        |        |
|        |        |        |        | **^1^  | file   |        |        |
|        |        |        |        |        | has    |        |        |
|        |        |        |        |        | been   |        |        |
|        |        |        |        |        | loaded |        |        |
|        |        |        |        |        | ,      |        |        |
|        |        |        |        |        | not    |        |        |
|        |        |        |        |        | editab |        |        |
|        |        |        |        |        | le.    |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| **10** | **CDB  | Label  |        |        | Always | N/A    |        |
|        | Descri |        |        |        | visibl |        |        |
|        | ption* |        |        |        | e,     |        |        |
|        | *      |        |        |        | not    |        |        |
|        |        |        |        |        | editab |        |        |
|        |        |        |        |        | le.    |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| **11** |        | TextBo |        | **CDB  | Visibl | N/A    |        |
|        |        | x      |        | Descri | e      |        |        |
|        |        |        |        | ption  | only   |        |        |
|        |        |        |        | text** | when a |        |        |
|        |        |        |        |        | PC     |        |        |
|        |        |        |        |        | file   |        |        |
|        |        |        |        |        | has    |        |        |
|        |        |        |        |        | been   |        |        |
|        |        |        |        |        | loaded |        |        |
|        |        |        |        |        | ,      |        |        |
|        |        |        |        |        | not    |        |        |
|        |        |        |        |        | editab |        |        |
|        |        |        |        |        | le.    |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+

Notes:

> 1\. For example, (R003).

[]{#_Toc322617781 .anchor}Table 4.1-2: ACDG Host Primary Screen -- Menu
Tree

+-------------+-------------+-------------+-------------+-------------+
| **Item \#** | **1^st^     | **2^nd^     | **2^nd^     | **Model     |
|             | Menu**      | Menu**      | Menu        | Unique**    |
|             |             |             | Availabilit |             |
|             |             |             | y**         |             |
+=============+=============+=============+=============+=============+
| 1           | File        | File New    | Enabled     |             |
|             |             |             | when a      |             |
|             |             |             | Plug-In has |             |
|             |             |             | been        |             |
|             |             |             | selected.   |             |
|             |             |             |             |             |
|             |             |             | Otherwise,  |             |
|             |             |             | always      |             |
|             |             |             | visible,    |             |
|             |             |             | not         |             |
|             |             |             | selectable. |             |
+-------------+-------------+-------------+-------------+-------------+
| 2           |             | File Open   | Enabled     |             |
|             |             |             | when a      |             |
|             |             |             | Plug-In has |             |
|             |             |             | been        |             |
|             |             |             | selected.   |             |
|             |             |             |             |             |
|             |             |             | Otherwise,  |             |
|             |             |             | always      |             |
|             |             |             | visible,    |             |
|             |             |             | not         |             |
|             |             |             | selectable. |             |
+-------------+-------------+-------------+-------------+-------------+
| 3           |             | File Save   | Enabled     |             |
|             |             |             | only when a |             |
|             |             |             | database    |             |
|             |             |             | has been    |             |
|             |             |             | loaded.     |             |
|             |             |             |             |             |
|             |             |             | Otherwise,  |             |
|             |             |             | always      |             |
|             |             |             | visible,    |             |
|             |             |             | not         |             |
|             |             |             | selectable. |             |
+-------------+-------------+-------------+-------------+-------------+
| 4           |             | File Save   | Enabled     |             |
|             |             | As          | only when a |             |
|             |             |             | database    |             |
|             |             |             | has been    |             |
|             |             |             | loaded.     |             |
|             |             |             |             |             |
|             |             |             | Otherwise,  |             |
|             |             |             | always      |             |
|             |             |             | visible,    |             |
|             |             |             | not         |             |
|             |             |             | selectable. |             |
+-------------+-------------+-------------+-------------+-------------+
| 5           |             | Config Info | Enabled     |             |
|             |             |             | only when a |             |
|             |             |             | database    |             |
|             |             |             | has been    |             |
|             |             |             | loaded.     |             |
|             |             |             |             |             |
|             |             |             | Otherwise,  |             |
|             |             |             | always      |             |
|             |             |             | visible,    |             |
|             |             |             | not         |             |
|             |             |             | selectable. |             |
+-------------+-------------+-------------+-------------+-------------+
| 6           |             | File Close  | Enabled     |             |
|             |             |             | only when a |             |
|             |             |             | database    |             |
|             |             |             | has been    |             |
|             |             |             | loaded.     |             |
|             |             |             |             |             |
|             |             |             | Otherwise,  |             |
|             |             |             | always      |             |
|             |             |             | visible,    |             |
|             |             |             | not         |             |
|             |             |             | selectable. |             |
+-------------+-------------+-------------+-------------+-------------+
| 7           |             | [E]{.underl | Always      |             |
|             |             | ine}xit     | enabled.    |             |
+-------------+-------------+-------------+-------------+-------------+
| 8           | Data        | See         | Enabled     |             |
|             |             | D620Z012-13 | only when a |             |
|             |             | ,           | database    |             |
|             |             | Section 4.0 | has been    |             |
|             |             |             | loaded.     |             |
|             |             |             |             |             |
|             |             |             | Otherwise,  |             |
|             |             |             | always      |             |
|             |             |             | visible,    |             |
|             |             |             | not         |             |
|             |             |             | selectable. |             |
+-------------+-------------+-------------+-------------+-------------+
| 9           | Report      | Report      | Enabled     |             |
|             |             |             | only when a |             |
|             |             |             | database    |             |
|             |             |             | has been    |             |
|             |             |             | loaded.     |             |
|             |             |             |             |             |
|             |             |             | Otherwise,  |             |
|             |             |             | always      |             |
|             |             |             | visible,    |             |
|             |             |             | not         |             |
|             |             |             | selectable. |             |
+-------------+-------------+-------------+-------------+-------------+
| 10          |             | Difference  | Enabled     |             |
|             |             | Report      | when a      |             |
|             |             |             | Plug-In has |             |
|             |             |             | been        |             |
|             |             |             | selected.   |             |
|             |             |             |             |             |
|             |             |             | Otherwise,  |             |
|             |             |             | always      |             |
|             |             |             | visible,    |             |
|             |             |             | not         |             |
|             |             |             | selectable. |             |
+-------------+-------------+-------------+-------------+-------------+
| 11          | Utilities   | Consistency | Enabled     |             |
|             |             | Check       | only when a |             |
|             |             |             | database    |             |
|             |             |             | has been    |             |
|             |             |             | loaded.     |             |
|             |             |             |             |             |
|             |             |             | Otherwise,  |             |
|             |             |             | always      |             |
|             |             |             | visible,    |             |
|             |             |             | not         |             |
|             |             |             | selectable. |             |
+-------------+-------------+-------------+-------------+-------------+
| 12          |             | Build LSAP  | See Table   |             |
|             |             | Files       | 4.1-3.      |             |
+-------------+-------------+-------------+-------------+-------------+
| 13          |             | Plu[g]{.und | Always      |             |
|             |             | erline}-In  | enabled.    |             |
|             |             | Packages    |             |             |
+-------------+-------------+-------------+-------------+-------------+
| 14          | Advanced    | Import XML  | Enabled     |             |
|             |             |             | when a      |             |
|             |             |             | Plug-In has |             |
|             |             |             | been        |             |
|             |             |             | selected.   |             |
|             |             |             |             |             |
|             |             |             | Otherwise,  |             |
|             |             |             | always      |             |
|             |             |             | visible,    |             |
|             |             |             | not         |             |
|             |             |             | selectable. |             |
+-------------+-------------+-------------+-------------+-------------+
| 15          |             | Export XML  | Enabled     |             |
|             |             |             | only when a |             |
|             |             |             | database    |             |
|             |             |             | has been    |             |
|             |             |             | loaded.     |             |
|             |             |             |             |             |
|             |             |             | Otherwise,  |             |
|             |             |             | always      |             |
|             |             |             | visible,    |             |
|             |             |             | not         |             |
|             |             |             | selectable. |             |
+-------------+-------------+-------------+-------------+-------------+
| 16          |             | SDT         | See Table   |             |
|             |             | Conversion  | 4.1-3.      |             |
+-------------+-------------+-------------+-------------+-------------+
| 17          |             | CDB         | See Table   |             |
|             |             | Consistency | 4.1-3.      |             |
|             |             | Check       |             |             |
+-------------+-------------+-------------+-------------+-------------+
| 18          |             | Export CDB  | See Table   |             |
|             |             | CSV Files   | 4.1-3.      |             |
+-------------+-------------+-------------+-------------+-------------+
| 19          | Help        | [H]{.underl | Always      |             |
|             |             | ine}elp     | enabled.    |             |
|             |             | CDG         |             |             |
+-------------+-------------+-------------+-------------+-------------+
| 20          |             | [A]{.underl | Always      |             |
|             |             | ine}bout    | enabled.    |             |
+-------------+-------------+-------------+-------------+-------------+

[]{#_Toc322618041 .anchor}Table 4.1-3: ACDG Host Tool Primary Screen -
Behavior

  **Item \#**   **Tool Behavior**                                                                               **Activated On**                **Result**                                **Model Unique**
  ------------- ----------------------------------------------------------------------------------------------- ------------------------------- ----------------------------------------- ------------------
  1             Imports an XML file                                                                             Import XML                      Build LSAP is disabled.                   
  2                                                                                                                                             SDT Conversion will be disabled.          
  3                                                                                                                                             CDB Consistency Check will be disabled.   
  4                                                                                                                                             Export CDB CSV files will be disabled.    
  5                                                                                                                                             Tool contains unsaved changes.            
  6             Creates a new PC file                                                                           File New                        Build LSAP is disabled.                   
  7                                                                                                                                             SDT Conversion will be disabled.          
  8                                                                                                                                             CDB Consistency Check will be disabled.   
  9                                                                                                                                             Export CDB CSV files will be disabled.    
  10                                                                                                                                            Tool contains unsaved changes.            
  11            Opens a PC file AND Updater is not executed AND Consistency check passed from PC file.          File Open                       CDB Consistency Check will be disabled.   
  12                                                                                                                                            Export CDB CSV files will be disabled.    
  13                                                                                                                                            SDT Conversion will be enabled.           
  14                                                                                                                                            Build LSAP is enabled.                    
  15            Opens a PC file AND Updater is not executed AND Consistency check status failed from PC file.   File Open                       CDB Consistency Check will be disabled.   
  16                                                                                                                                            Export CDB CSV files will be disabled.    
  17                                                                                                                                            SDT Conversion will be disabled.          
  18                                                                                                                                            Build LSAP is disabled.                   
  19            Opens a PC file AND Updater is executed.                                                        File Open                       Build LSAP is disabled.                   
  20                                                                                                                                            SDT Conversion will be disabled.          
  21                                                                                                                                            CDB Consistency Check will be disabled.   
  22                                                                                                                                            Export CDB CSV files will be disabled.    
  23                                                                                                                                            Tool contains unsaved changes.            
  24            Closes the loaded PC file.                                                                      File Close                      Build LSAP is disabled.                   
  25                                                                                                                                            SDT Conversion will be disabled.          
  26                                                                                                                                            CDB Consistency Check will be disabled.   
  27                                                                                                                                            Export CDB CSV files will be disabled.    
  28            Accepts changes in the Editor                                                                   Accept data changes in Editor   Build LSAP is disabled.                   
  29                                                                                                                                            SDT Conversion will be disabled.          
  30                                                                                                                                            CDB Consistency Check will be disabled.   
  31                                                                                                                                            Export CDB CSV files will be disabled.    
  32                                                                                                                                            Tool contains unsaved changes.            
  33            Modifies the database description                                                               Accept changes in Config Info   Tool contains unsaved changes.            
  34            Fails Consistency Check with at least 1 critical error                                          Consistency Check               Build LSAP is disabled.                   
  35                                                                                                                                            SDT Conversion will be disabled.          
  36                                                                                                                                            CDB Consistency Check will be disabled.   
  37            Passes Consistency Check with 0 Critical errors                                                 Consistency Check               Build LSAP is enabled.                    
  38                                                                                                                                            SDT Conversion will be enabled.           
  39            Completes SDT Conversion                                                                        SDT Conversion                  CDB Consistency Check will be enabled.    
  40                                                                                                                                            Export CDB CSV files will be enabled.     
                                                                                                                                                                                          

[]{#_Toc395021810 .anchor}Table 4.1-4: ACDG Host Primary Screen -
Operation Checks

+-------------+-------------+-------------+-------------+-------------+
| **Item \#** | **Consisten | **Activated | **Result**  | **Model     |
|             | cy          | On**        |             | Unique**    |
|             | Check       |             |             |             |
|             | Rule**      |             |             |             |
+=============+=============+=============+=============+=============+
| 1           | Check for   | File New,   | Displays    |             |
|             | unsaved     | File Open,  | warning     |             |
|             | changes.    | File Close, | dialog box  |             |
|             |             | Exit        | per Table   |             |
|             |             |             | 5.1-1, item |             |
|             |             |             | 1.          |             |
+-------------+-------------+-------------+-------------+-------------+
| 2           | Check for   | Build LSAP  | Displays    |             |
|             | unsaved     | Files       | warning     |             |
|             | changes.    |             | dialog box  |             |
|             |             |             | per Table   |             |
|             |             |             | 5.1-1, item |             |
|             |             |             | 9.          |             |
+-------------+-------------+-------------+-------------+-------------+
| 3           | Check if    | File Save   | Displays    |             |
|             | Updater was |             | warning     |             |
|             | executed on |             | dialog box  |             |
|             | file open.  |             | per Table   |             |
|             |             |             | 5.1-1, item |             |
|             |             |             | 2.          |             |
+-------------+-------------+-------------+-------------+-------------+
| 4           | Check if PC | Save file   | Displays    |             |
|             | file name   | AND Browse  | warning     |             |
|             | already     | for folder  | dialog box  |             |
|             | exists in   |             | per Table   |             |
|             | that        |             | 5.1-1, item |             |
|             | location.   |             | 3.          |             |
+-------------+-------------+-------------+-------------+-------------+
| 5           | Check that  | File Open   | See Table   |             |
|             | the file    |             | 2-1 in      |             |
|             | being       | Import XML  | D620Z012-19 |             |
|             | opened is   |             |             |             |
|             | compatible  |             |             |             |
|             | with the    |             |             |             |
|             | currently   |             |             |             |
|             | selected    |             |             |             |
|             | Plug-In.    |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| 6           | (Deleted)   | (Deleted)   | (Deleted)   |             |
+-------------+-------------+-------------+-------------+-------------+
| 7           | Promt the   | File Open   | Displays    |             |
|             | user when   |             | warning     |             |
|             | opening an  | Import XML  | dialog box  |             |
|             | incompatibl |             | per Table   |             |
|             | e           |             | 4-1, item 2 |             |
|             | File. See   |             | in          |             |
|             | Table 2-1   |             | D620Z012-19 |             |
|             | in          |             |             |             |
|             | D620Z012-19 |             |             |             |
|             | for         |             |             |             |
|             | compatibili |             |             |             |
|             | ty.         |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| 8           | (Deleted)   | (Deleted)   | (Deleted)   |             |
+-------------+-------------+-------------+-------------+-------------+
| 9           | Check if    | File Save   | Displays    |             |
|             | the PC File |             | warning     |             |
|             | is          |             | dialog box  |             |
|             | Read-only   |             | per Table   |             |
|             |             |             | 5.1-1, item |             |
|             |             |             | 10.         |             |
+-------------+-------------+-------------+-------------+-------------+

4.2 Sub-Screens
---------------

The ACDG Host sub-screens are described in this section.

The File sub-screens are described in sections 4.2.1 through 4.2.5;
Utilities sub-screens in sections 4.2.6 and 4.2.7; Advanced sub-screens
in sections 4.2.8 through 4.2.13; and Help sub-screens in sections
4.2.14 and 4.2.15.

### 4.2.1 File New Screen

a\. The File New Screen controls shall be as defined in Table 4.2.1-1.

[]{#_Hlt122159022 .anchor}Table 4.2.1-1: File New Screen - Components

+--------+--------+--------+--------+--------+--------+--------+--------+
| **Item | **Labe | **Type | **Rang | **Deta | **Avai | **Tab  | **Mode |
| \#**   | l**    | **     | e**    | ils**  | labili | Order* | l      |
|        |        |        |        |        | ty**   | *      | Unique |
|        |        |        |        |        |        |        | **     |
+========+========+========+========+========+========+========+========+
| 1      | New    | Label  |        | Screen | Always |        |        |
|        | Config |        |        | Title; | visibl |        |        |
|        | uratio |        |        | bold,  | e,     |        |        |
|        | n      |        |        | underl | not    |        |        |
|        | Databa |        |        | ine    | editab |        |        |
|        | se     |        |        |        | le     |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 2      | Load   | TextBo |        |        | Always |        |        |
|        | Part   | x      |        |        | visibl |        |        |
|        | Number |        |        |        | e,     |        |        |
|        |        |        |        |        | not    |        |        |
|        |        |        |        |        | editab |        |        |
|        |        |        |        |        | le     |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 3      | ...    | Button |        | See    | Enable | 1      |        |
|        |        |        |        | Table  | d      |        |        |
|        |        |        |        | 4.2.1- |        |        |        |
|        |        |        |        | 2      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 4      | Config | TextBo | 1 min  |        | Always | 2      |        |
|        | uratio | x      | to 40  |        | editab |        |        |
|        | n      |        | max    |        | le     |        |        |
|        | Databa |        | Charac |        |        |        |        |
|        | se     |        | ters   |        |        |        |        |
|        | Descri |        |        |        |        |        |        |
|        | ption  |        | ASCII  |        |        |        |        |
|        |        |        | charac |        |        |        |        |
|        |        |        | ters\  |        |        |        |        |
|        |        |        | a-z    |        |        |        |        |
|        |        |        | A-Z    |        |        |        |        |
|        |        |        | 0-9 \` |        |        |        |        |
|        |        |        | \~ \^  |        |        |        |        |
|        |        |        | , . :  |        |        |        |        |
|        |        |        | ; ? !  |        |        |        |        |
|        |        |        | \_ \#  |        |        |        |        |
|        |        |        | - + /  |        |        |        |        |
|        |        |        | \* = % |        |        |        |        |
|        |        |        | \$ @   |        |        |        |        |
|        |        |        | \\ \|  |        |        |        |        |
|        |        |        | ) ( \] |        |        |        |        |
|        |        |        | \[ } { |        |        |        |        |
|        |        |        | \[spac |        |        |        |        |
|        |        |        | e\]    |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 5      | OK     | Button |        | See    | Enable | 3      |        |
|        |        |        |        | Figure | d      |        |        |
|        |        |        |        | 6.1-1  |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 6      | Cancel | Button |        | See    | Enable | 4      |        |
|        |        |        |        | Figure | d      |        |        |
|        |        |        |        | 6.1-1  |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+

b\. The File New Load Part Number screen shall be defined in Table
4.2.1-2.

[]{#_Toc346888981 .anchor}Table 4.2.1-2: File New Load Part Number
Screen

+--------+--------+--------+--------+--------+--------+--------+--------+
| **Item | **Labe | **Type | **Rang | **Deta | **Avai | **Tab  | **Mode |
| \#**   | l**    | **     | e**    | ils**  | labili | Order* | l      |
|        |        |        |        |        | ty**   | *      | Unique |
|        |        |        |        |        |        |        | **     |
+========+========+========+========+========+========+========+========+
| 1      | Load   | Label  |        | Screen | Always |        |        |
|        | Part   |        |        | Title; | visibl |        |        |
|        | Number |        |        | bold,  | e,     |        |        |
|        | conten |        |        | underl | not    |        |        |
|        | ts     |        |        | ine    | editab |        |        |
|        |        |        |        |        | le     |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 2      | Select | Label  |        | Headin | Always |        |        |
|        | label  |        |        | g      | visibl |        |        |
|        | type:  |        |        |        | e,     |        |        |
|        |        |        |        |        | not    |        |        |
|        |        |        |        |        | editab |        |        |
|        |        |        |        |        | le     |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 3      | Blue   | Radio  |        |        | Always | 2      |        |
|        | label  | Button |        |        | select |        |        |
|        |        |        |        |        | able;  |        |        |
|        |        |        |        |        | mutual |        |        |
|        |        |        |        |        | ly     |        |        |
|        |        |        |        |        | exclus |        |        |
|        |        |        |        |        | ive    |        |        |
|        |        |        |        |        | with   |        |        |
|        |        |        |        |        | item 4 |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 4      | Red/Bl | Radio  |        |        | Always | 1      |        |
|        | ack    | Button |        |        | select |        |        |
|        | label  |        |        |        | able;  |        |        |
|        |        |        |        |        | mutual |        |        |
|        |        |        |        |        | ly     |        |        |
|        |        |        |        |        | exclus |        |        |
|        |        |        |        |        | ive    |        |        |
|        |        |        |        |        | with   |        |        |
|        |        |        |        |        | item 3 |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 5      | Part   | Label  |        | Headin | Always |        |        |
|        | Number |        |        | g      | visibl |        |        |
|        | Format |        |        |        | e,     |        |        |
|        | :      |        |        |        | not    |        |        |
|        |        |        |        |        | editab |        |        |
|        |        |        |        |        | le     |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 6      | MMMCC- | Label  |        | Sub-he | Always |        |        |
|        | SSSS-S |        |        | ading; | visibl |        |        |
|        | SSS    |        |        | bold   | e,     |        |        |
|        |        |        |        |        | not    |        |        |
|        |        |        |        |        | editab |        |        |
|        |        |        |        |        | le     |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 7      | Field  |        |        | Column |        |        |        |
|        |        |        |        | Headin |        |        |        |
|        |        |        |        | g      |        |        |        |
|        |        |        |        | 1      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 8      | Descri |        |        | Column |        |        |        |
|        | ption  |        |        | Headin |        |        |        |
|        |        |        |        | g      |        |        |        |
|        |        |        |        | 2      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 9      | Charac |        |        | Column |        |        |        |
|        | ters   |        |        | Headin |        |        |        |
|        |        |        |        | g      |        |        |        |
|        |        |        |        | 3      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 10     | MMM    | Textbo | Three  | Column |        | 3      |        |
|        |        | x      | upper  | Headin |        |        |        |
|        |        |        | case   | g      |        |        |        |
|        |        |        | alphan | 1 text |        |        |        |
|        |        |        | umeric | = MMM  |        |        |        |
|        |        |        | charac |        |        |        |        |
|        |        |        | ters   | Column |        |        |        |
|        |        |        |        | Headin |        |        |        |
|        |        |        |        | g      |        |        |        |
|        |        |        |        | 2 text |        |        |        |
|        |        |        |        | =      |        |        |        |
|        |        |        |        | Three  |        |        |        |
|        |        |        |        | upper  |        |        |        |
|        |        |        |        | case   |        |        |        |
|        |        |        |        | alphan |        |        |        |
|        |        |        |        | umeric |        |        |        |
|        |        |        |        | charac |        |        |        |
|        |        |        |        | ters   |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 11     | SSSS   | Textbo | Four   | Column |        | 4      |        |
|        |        | x      | upper  | Headin |        |        |        |
|        |        |        | case   | g      |        |        |        |
|        |        |        | alphan | 1 text |        |        |        |
|        |        |        | umeric | = SSSS |        |        |        |
|        |        |        | charac |        |        |        |        |
|        |        |        | ters   | Column |        |        |        |
|        |        |        | but    | Headin |        |        |        |
|        |        |        | not I, | g      |        |        |        |
|        |        |        | O, Q,  | 2 text |        |        |        |
|        |        |        | or Z   | = Four |        |        |        |
|        |        |        |        | upper  |        |        |        |
|        |        |        |        | case   |        |        |        |
|        |        |        |        | alphan |        |        |        |
|        |        |        |        | umeric |        |        |        |
|        |        |        |        | charac |        |        |        |
|        |        |        |        | ters   |        |        |        |
|        |        |        |        | but    |        |        |        |
|        |        |        |        | not I, |        |        |        |
|        |        |        |        | O, Q,  |        |        |        |
|        |        |        |        | or Z   |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 12     | SSSS   | Textbo | Four   | Column |        | 5      |        |
|        |        | x      | upper  | Headin |        |        |        |
|        |        |        | case   | g      |        |        |        |
|        |        |        | alphan | 1 text |        |        |        |
|        |        |        | umeric | = SSSS |        |        |        |
|        |        |        | charac |        |        |        |        |
|        |        |        | ters   | Column |        |        |        |
|        |        |        | but    | Headin |        |        |        |
|        |        |        | not I, | g      |        |        |        |
|        |        |        | O, Q,  | 2 text |        |        |        |
|        |        |        | or Z   | = Four |        |        |        |
|        |        |        |        | upper  |        |        |        |
|        |        |        |        | case   |        |        |        |
|        |        |        |        | alphan |        |        |        |
|        |        |        |        | umeric |        |        |        |
|        |        |        |        | charac |        |        |        |
|        |        |        |        | ters   |        |        |        |
|        |        |        |        | but    |        |        |        |
|        |        |        |        | not I, |        |        |        |
|        |        |        |        | O, Q,  |        |        |        |
|        |        |        |        | or Z   |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 13     | CC     | TextBo |        | This   | Always |        |        |
|        |        | x      |        | field  | visibl |        |        |
|        |        |        |        | calcul | e,     |        |        |
|        |        |        |        | ates   | not    |        |        |
|        |        |        |        | the CC | editab |        |        |
|        |        |        |        | per    | le     |        |        |
|        |        |        |        | ARINC  |        |        |        |
|        |        |        |        | 665-3  |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 14     | Load   | TextBo |        | This   | Always |        |        |
|        | Part   | x      |        | field  | visibl |        |        |
|        | No.    |        |        | displa | e,     |        |        |
|        |        |        |        | ys     | not    |        |        |
|        |        |        |        | the    | editab |        |        |
|        |        |        |        | Load   | le     |        |        |
|        |        |        |        | Part   |        |        |        |
|        |        |        |        | Number |        |        |        |
|        |        |        |        | per    |        |        |        |
|        |        |        |        | ARINC  |        |        |        |
|        |        |        |        | 665-3  |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 15     | OK     | Button |        | See    | Enable | 6      |        |
|        |        |        |        | Figure | d      |        |        |
|        |        |        |        | 6.1-1  |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 16     | Close  | Button |        | See    | Enable | 7      |        |
|        |        |        |        | Figure | d      |        |        |
|        |        |        |        | 6.1-1  |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+

### 4.2.2 File Open Screen

a\. The File Open Screen shall have the following characteristics:

1\. The Open Screen shall be provided by the Operating System

2\. The Open Screen shall only allow browsing of directory folders and
the selection of .pc files.

3\. The Open Screen shall remember the file path of the parent directory
of the last opened .pc file for the current program session.

4\. The Open Screen's starting file path shall be the Default starting
file path.

### 4.2.3 File Save Screen

a\. The File Save Screen shall have the following characteristics:

1\. The Save Screen shall be provided by the Operating System.

2\. The Save Screen shall only allow browsing of directory folders.

3\. The Save Screen shall remember the file path of the parent directory
of the last opened .pc file for the current program session.

4\. The Save Screen's starting file path shall be the Default starting
file path.

### 4.2.4 File SaveAs Screen

a\. The File SaveAs Screen controls shall be as defined in Table 4.2.4-1.

[]{#_Toc395021813 .anchor}Table 4.2.4-1: File SaveAs Screen - Components

+--------+--------+--------+--------+--------+--------+--------+--------+
| **Item | **Labe | **Type | **Rang | **Deta | **Avai | **Tab  | **Mode |
| \#**   | l**    | **     | e**    | ils**  | labili | Order* | l      |
|        |        |        |        |        | ty**   | *      | Unique |
|        |        |        |        |        |        |        | **     |
+========+========+========+========+========+========+========+========+
| 1      | PC     | Label  |        | Screen | Always |        |        |
|        | File   |        |        | Title; | visibl |        |        |
|        | Save   |        |        | bold,  | e,     |        |        |
|        | As     |        |        | underl | not    |        |        |
|        |        |        |        | ine    | editab |        |        |
|        |        |        |        |        | le     |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 2      | PC     | TextBo |        |        | Always | 1      |        |
|        | File   | x      |        |        | editab |        |        |
|        | Direct |        |        |        | le     |        |        |
|        | ory    |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 3      | ...    | Button |        | A      | Enable | 2      |        |
|        |        |        |        | standa | d      |        |        |
|        |        |        |        | rd     |        |        |        |
|        |        |        |        | Window |        |        |        |
|        |        |        |        | s      |        |        |        |
|        |        |        |        | OS     |        |        |        |
|        |        |        |        | Browse |        |        |        |
|        |        |        |        | For    |        |        |        |
|        |        |        |        | Folder |        |        |        |
|        |        |        |        | screen |        |        |        |
|        |        |        |        | is     |        |        |        |
|        |        |        |        | used   |        |        |        |
|        |        |        |        | to     |        |        |        |
|        |        |        |        | select |        |        |        |
|        |        |        |        | the    |        |        |        |
|        |        |        |        | file   |        |        |        |
|        |        |        |        | direct |        |        |        |
|        |        |        |        | ory.   |        |        |        |
|        |        |        |        |        |        |        |        |
|        |        |        |        | The    |        |        |        |
|        |        |        |        | browse |        |        |        |
|        |        |        |        | r      |        |        |        |
|        |        |        |        | starti |        |        |        |
|        |        |        |        | ng     |        |        |        |
|        |        |        |        | file   |        |        |        |
|        |        |        |        | path   |        |        |        |
|        |        |        |        | shall  |        |        |        |
|        |        |        |        | be the |        |        |        |
|        |        |        |        | Defaul |        |        |        |
|        |        |        |        | t      |        |        |        |
|        |        |        |        | starti |        |        |        |
|        |        |        |        | ng     |        |        |        |
|        |        |        |        | file   |        |        |        |
|        |        |        |        | path.  |        |        |        |
|        |        |        |        |        |        |        |        |
|        |        |        |        | The    |        |        |        |
|        |        |        |        | browse |        |        |        |
|        |        |        |        | r      |        |        |        |
|        |        |        |        | shall  |        |        |        |
|        |        |        |        | rememb |        |        |        |
|        |        |        |        | er     |        |        |        |
|        |        |        |        | the    |        |        |        |
|        |        |        |        | file   |        |        |        |
|        |        |        |        | path   |        |        |        |
|        |        |        |        | of the |        |        |        |
|        |        |        |        | parent |        |        |        |
|        |        |        |        | direct |        |        |        |
|        |        |        |        | ory    |        |        |        |
|        |        |        |        | of the |        |        |        |
|        |        |        |        | last   |        |        |        |
|        |        |        |        | opened |        |        |        |
|        |        |        |        | .pc    |        |        |        |
|        |        |        |        | file   |        |        |        |
|        |        |        |        | for    |        |        |        |
|        |        |        |        | the    |        |        |        |
|        |        |        |        | curren |        |        |        |
|        |        |        |        | t      |        |        |        |
|        |        |        |        | progra |        |        |        |
|        |        |        |        | m      |        |        |        |
|        |        |        |        | sessio |        |        |        |
|        |        |        |        | n.     |        |        |        |
|        |        |        |        |        |        |        |        |
|        |        |        |        | NOTE:  |        |        |        |
|        |        |        |        | additi |        |        |        |
|        |        |        |        | onally |        |        |        |
|        |        |        |        | contai |        |        |        |
|        |        |        |        | ns     |        |        |        |
|        |        |        |        | a Make |        |        |        |
|        |        |        |        | New    |        |        |        |
|        |        |        |        | Folder |        |        |        |
|        |        |        |        | button |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 4      | New    | TextBo |        |        | Always |        |        |
|        | Load   | x      |        |        | visibl |        |        |
|        | Part   |        |        |        | e,     |        |        |
|        | Number |        |        |        | not    |        |        |
|        |        |        |        |        | editab |        |        |
|        |        |        |        |        | le     |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 5      | ...    | Button |        | See    | Enable | 3      |        |
|        |        |        |        | Table  | d      |        |        |
|        |        |        |        | 4.2.1- |        |        |        |
|        |        |        |        | 2      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 6      | Config | TextBo | 1 min  |        | Always | 4      |        |
|        | uratio | x      | to 40  |        | editab |        |        |
|        | n      |        | max    |        | le     |        |        |
|        | Databa |        | Charac |        |        |        |        |
|        | se     |        | ters   |        |        |        |        |
|        | Descri |        |        |        |        |        |        |
|        | ption  |        | ASCII  |        |        |        |        |
|        |        |        | charac |        |        |        |        |
|        |        |        | ters\  |        |        |        |        |
|        |        |        | a-z    |        |        |        |        |
|        |        |        | A-Z    |        |        |        |        |
|        |        |        | 0-9 \` |        |        |        |        |
|        |        |        | \~ \^  |        |        |        |        |
|        |        |        | , . :  |        |        |        |        |
|        |        |        | ; ? !  |        |        |        |        |
|        |        |        | \_ \#  |        |        |        |        |
|        |        |        | - + /  |        |        |        |        |
|        |        |        | \* = % |        |        |        |        |
|        |        |        | \$ @   |        |        |        |        |
|        |        |        | \\ \|  |        |        |        |        |
|        |        |        | ) ( \] |        |        |        |        |
|        |        |        | \[ } { |        |        |        |        |
|        |        |        | \[spac |        |        |        |        |
|        |        |        | e\]    |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 7      | OK     | Button |        | See    | Enable | 5      |        |
|        |        |        |        | Figure | d      |        |        |
|        |        |        |        | 6.1-4  |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 8      | Cancel | Button |        | See    | Enable | 6      |        |
|        |        |        |        | Figure | d      |        |        |
|        |        |        |        | 6.1-4  |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+

### 4.2.5 Configuration Information Screen

a\. The Config Info Screen controls shall be as defined in Table 4.2.5-1.

[]{#_Toc395021814 .anchor}Table 4.2.5-1: Config Info Screen - Components

+--------+--------+--------+--------+--------+--------+--------+--------+
| **Item | **Labe | **Type | **Rang | **Deta | **Avai | **Tab  | **Mode |
| \#**   | l**    | **     | e**    | ils**  | labili | Order* | l      |
|        |        |        |        |        | ty**   | *      | Unique |
|        |        |        |        |        |        |        | **     |
+========+========+========+========+========+========+========+========+
| 1      | [Confi | Label  |        | Screen |        |        |        |
|        | gurati |        |        | Title; |        |        |        |
|        | on     |        |        | bold,  |        |        |        |
|        | Inform |        |        | underl |        |        |        |
|        | ations |        |        | ine    |        |        |        |
|        | ]{.und |        |        |        |        |        |        |
|        | erline |        |        |        |        |        |        |
|        | }      |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 2      | [Confi | Label  |        | Underl | Always |        |        |
|        | gurati |        |        | ine    | visibl |        |        |
|        | on     |        |        |        | e,     |        |        |
|        | Databa |        |        |        | not    |        |        |
|        | se     |        |        |        | editab |        |        |
|        | Descri |        |        |        | le     |        |        |
|        | ption] |        |        |        |        |        |        |
|        | {.unde |        |        |        |        |        |        |
|        | rline} |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 3      | Config | TextBo | 1 min  |        | Always | 1      |        |
|        | uratio | x      | to 40  |        | editab |        |        |
|        | n      |        | max    |        | le     |        |        |
|        | Databa |        | Charac |        |        |        |        |
|        | se     |        | ters   |        |        |        |        |
|        | Descri |        |        |        |        |        |        |
|        | ption  |        | ASCII  |        |        |        |        |
|        |        |        | charac |        |        |        |        |
|        |        |        | ters\  |        |        |        |        |
|        |        |        | a-z    |        |        |        |        |
|        |        |        | A-Z    |        |        |        |        |
|        |        |        | 0-9 \` |        |        |        |        |
|        |        |        | \~ \^  |        |        |        |        |
|        |        |        | , . :  |        |        |        |        |
|        |        |        | ; ? !  |        |        |        |        |
|        |        |        | \_ \#  |        |        |        |        |
|        |        |        | - + /  |        |        |        |        |
|        |        |        | \* = % |        |        |        |        |
|        |        |        | \$ @   |        |        |        |        |
|        |        |        | \\ \|  |        |        |        |        |
|        |        |        | ) ( \] |        |        |        |        |
|        |        |        | \[ } { |        |        |        |        |
|        |        |        | \[spac |        |        |        |        |
|        |        |        | e\]    |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 4      | [Airpl | Label  |        | Displa | Always | 2      |        |
|        | ane    |        |        | ys     | visibl |        |        |
|        | Model] |        |        | the    | e,     |        |        |
|        | {.unde |        |        | airpla | not    |        |        |
|        | rline} |        |        | ne     | editab |        |        |
|        |        |        |        | model  | le     |        |        |
|        |        |        |        | of the |        |        |        |
|        |        |        |        | PC     |        |        |        |
|        |        |        |        | File   |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 5      | [Time  | Label  |        | Displa | Always |        |        |
|        | Stamp] |        |        | ys     | visibl |        |        |
|        | {.unde |        |        | the    | e,     |        |        |
|        | rline} |        |        | creati | not    |        |        |
|        |        |        |        | on     | editab |        |        |
|        |        |        |        | date   | le     |        |        |
|        |        |        |        | and    |        |        |        |
|        |        |        |        | time   |        |        |        |
|        |        |        |        | of the |        |        |        |
|        |        |        |        | PC     |        |        |        |
|        |        |        |        | File   |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 6      | [Revis | Label  |        | Displa | Always |        |        |
|        | ion]{. |        |        | ys     | visibl |        |        |
|        | underl |        |        | the    | e,     |        |        |
|        | ine}   |        |        | revisi | not    |        |        |
|        |        |        |        | on     | editab |        |        |
|        |        |        |        | number | le     |        |        |
|        |        |        |        | of the |        |        |        |
|        |        |        |        | PC     |        |        |        |
|        |        |        |        | File   |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 7      | [CDG   | Label  |        | Displa | Always |        |        |
|        | Part   |        |        | ys     | visibl |        |        |
|        | Number |        |        | the    | e,     |        |        |
|        | ]{.und |        |        | part   | not    |        |        |
|        | erline |        |        | number | editab |        |        |
|        | }      |        |        | of the | le     |        |        |
|        |        |        |        | Panaso |        |        |        |
|        |        |        |        | nic    |        |        |        |
|        |        |        |        | CDG    |        |        |        |
|        |        |        |        | Tool   |        |        |        |
|        |        |        |        | when   |        |        |        |
|        |        |        |        | the PC |        |        |        |
|        |        |        |        | File   |        |        |        |
|        |        |        |        | was    |        |        |        |
|        |        |        |        | create |        |        |        |
|        |        |        |        | d      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 8      | [Plug- | Label  |        | Displa | Always |        |        |
|        | in     |        |        | ys     | visibl |        |        |
|        | Packag |        |        | the    | e,     |        |        |
|        | e      |        |        | plug-i | not    |        |        |
|        | Name]{ |        |        | n      | editab |        |        |
|        | .under |        |        | packag | le     |        |        |
|        | line}  |        |        | e      |        |        |        |
|        |        |        |        | used   |        |        |        |
|        |        |        |        | when   |        |        |        |
|        |        |        |        | the PC |        |        |        |
|        |        |        |        | File   |        |        |        |
|        |        |        |        | was    |        |        |        |
|        |        |        |        | create |        |        |        |
|        |        |        |        | d      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 9      | [Plug- | Label  |        | Displa | Always |        |        |
|        | in     |        |        | ys     | visibl |        |        |
|        | Versio |        |        | the    | e,     |        |        |
|        | n      |        |        | plug-i | not    |        |        |
|        | Number |        |        | n      | editab |        |        |
|        | ]{.und |        |        | versio | le     |        |        |
|        | erline |        |        | n      |        |        |        |
|        | }      |        |        | number |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 10     | [Load  | Label  |        | Displa | Always |        |        |
|        | Part   |        |        | ys     | visibl |        |        |
|        | Number |        |        | the    | e,     |        |        |
|        | ]{.und |        |        | ARINC  | not    |        |        |
|        | erline |        |        | 665-3  | editab |        |        |
|        | }      |        |        | LSAP   | le     |        |        |
|        |        |        |        | part   |        |        |        |
|        |        |        |        | number |        |        |        |
|        |        |        |        | of the |        |        |        |
|        |        |        |        | PC     |        |        |        |
|        |        |        |        | File   |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 11     | [ACDG  | Label  |        | Displa | Always |        |        |
|        | Host   |        |        | ys     | visibl |        |        |
|        | Part   |        |        | the    | e,     |        |        |
|        | Number |        |        | host   | not    |        |        |
|        | ]{.und |        |        | part   | editab |        |        |
|        | erline |        |        | number | le     |        |        |
|        | }      |        |        |        |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 12     | [Produ | Label  |        | Displa | Always |        |        |
|        | ct     |        |        | ys     | visibl |        |        |
|        | Versio |        |        | the    | e,     |        |        |
|        | n      |        |        | produc | not    |        |        |
|        | Number |        |        | t      | editab |        |        |
|        | ]{.und |        |        | versio | le     |        |        |
|        | erline |        |        | n      |        |        |        |
|        | }      |        |        | number |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 13     | OK     | Button |        | See    | Enable | 2      |        |
|        |        |        |        | Figure | d      |        |        |
|        |        |        |        | 6.1-5  |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 14     | Cancel | Button |        | See    | Enable | 3      |        |
|        |        |        |        | Figure | d      |        |        |
|        |        |        |        | 6.1-6  |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+

### 4.2.6 Plug-In Packages Screen

a\. The Plug-In Packages Screen controls shall be as defined in Table
4.2.6-1.

[]{#_Toc395021815 .anchor}Table 4.2.6-1: Plug-In Packages Screen -
Components

+--------+--------+--------+--------+--------+--------+--------+--------+
| **Item | **Labe | **Type | **Rang | **Deta | **Avai | **Tab  | **Mode |
| \#**   | l**    | **     | e**    | ils**  | labili | Order* | l      |
|        |        |        |        |        | ty**   | *      | Unique |
|        |        |        |        |        |        |        | **     |
+========+========+========+========+========+========+========+========+
| 1      | Plug-I | Label  |        | Screen | Always |        |        |
|        | n      |        |        | Title; | visibl |        |        |
|        | Loader |        |        | bold,  | e,     |        |        |
|        |        |        |        | underl | not    |        |        |
|        |        |        |        | ine    | editab |        |        |
|        |        |        |        |        | le     |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 2      | Airpla | DropBo | B787\  |        | Always | 1      |        |
|        | ne     | x      | B747-8 |        | select |        |        |
|        | Model  |        |        |        | able   |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 3      | Select | TextBo |        | Displa | Always |        |        |
|        | ed     | x      |        | ys     | visibl |        |        |
|        | Plug-I |        |        | the    | e,     |        |        |
|        | n      |        |        | name   | not    |        |        |
|        | Packag |        |        | of the | editab |        |        |
|        | e      |        |        | curren | le     |        |        |
|        |        |        |        | tly    |        |        |        |
|        |        |        |        | select |        |        |        |
|        |        |        |        | ed     |        |        |        |
|        |        |        |        | Plug-I |        |        |        |
|        |        |        |        | n      |        |        |        |
|        |        |        |        | Packag |        |        |        |
|        |        |        |        | e      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 4      | Plug-I | ListBo |        | Highli | Always | 2      |        |
|        | n      | x      |        | ght    | select |        |        |
|        | Packag |        |        | the    | able   |        |        |
|        | e      |        |        | curren |        |        |        |
|        |        |        |        | tly    |        |        |        |
|        |        |        |        | select |        |        |        |
|        |        |        |        | ed     |        |        |        |
|        |        |        |        | Plug-I |        |        |        |
|        |        |        |        | n      |        |        |        |
|        |        |        |        | Packag |        |        |        |
|        |        |        |        | e      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 5      | [Time  | Label  |        | Displa | Always |        |        |
|        | Stamp] |        |        | ys     | visibl |        |        |
|        | {.unde |        |        | the    | e,     |        |        |
|        | rline} |        |        | creati | not    |        |        |
|        |        |        |        | on     | editab |        |        |
|        |        |        |        | date   | le     |        |        |
|        |        |        |        | and    |        |        |        |
|        |        |        |        | time   |        |        |        |
|        |        |        |        | of the |        |        |        |
|        |        |        |        | curren |        |        |        |
|        |        |        |        | tly    |        |        |        |
|        |        |        |        | select |        |        |        |
|        |        |        |        | ed     |        |        |        |
|        |        |        |        | Plug-I |        |        |        |
|        |        |        |        | n      |        |        |        |
|        |        |        |        | Packag |        |        |        |
|        |        |        |        | e      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 6      | [Name] | Label  |        | Displa | Always |        |        |
|        | {.unde |        |        | ys     | visibl |        |        |
|        | rline} |        |        | the    | e,     |        |        |
|        |        |        |        | name   | not    |        |        |
|        |        |        |        | of the | editab |        |        |
|        |        |        |        | curren | le     |        |        |
|        |        |        |        | tly    |        |        |        |
|        |        |        |        | select |        |        |        |
|        |        |        |        | ed     |        |        |        |
|        |        |        |        | Plug-I |        |        |        |
|        |        |        |        | n      |        |        |        |
|        |        |        |        | Packag |        |        |        |
|        |        |        |        | e      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 7      | [Descr | Label  |        | Displa | Always |        |        |
|        | iption |        |        | ys     | visibl |        |        |
|        | ]{.und |        |        | the    | e,     |        |        |
|        | erline |        |        | descri | not    |        |        |
|        | }      |        |        | ption  | editab |        |        |
|        |        |        |        | of the | le     |        |        |
|        |        |        |        | curren |        |        |        |
|        |        |        |        | tly    |        |        |        |
|        |        |        |        | select |        |        |        |
|        |        |        |        | ed     |        |        |        |
|        |        |        |        | Plug-I |        |        |        |
|        |        |        |        | n      |        |        |        |
|        |        |        |        | Packag |        |        |        |
|        |        |        |        | e      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 8      | Select | Button |        | See    | Enable | 3      |        |
|        |        |        |        | Table  | d      |        |        |
|        |        |        |        | 4.2.6- |        |        |        |
|        |        |        |        | 2      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 9      | Add    | Button |        | A      | Enable | 4      |        |
|        |        |        |        | standa | d      |        |        |
|        |        |        |        | rd     |        |        |        |
|        |        |        |        | Window |        |        |        |
|        |        |        |        | s      |        |        |        |
|        |        |        |        | OS     |        |        |        |
|        |        |        |        | open   |        |        |        |
|        |        |        |        | file   |        |        |        |
|        |        |        |        | screen |        |        |        |
|        |        |        |        | is     |        |        |        |
|        |        |        |        | used   |        |        |        |
|        |        |        |        | to     |        |        |        |
|        |        |        |        | select |        |        |        |
|        |        |        |        | a      |        |        |        |
|        |        |        |        | Packag |        |        |        |
|        |        |        |        | e      |        |        |        |
|        |        |        |        | File   |        |        |        |
|        |        |        |        | (\*.gz |        |        |        |
|        |        |        |        | )      |        |        |        |
|        |        |        |        |        |        |        |        |
|        |        |        |        | The    |        |        |        |
|        |        |        |        | browse |        |        |        |
|        |        |        |        | r      |        |        |        |
|        |        |        |        | starti |        |        |        |
|        |        |        |        | ng     |        |        |        |
|        |        |        |        | file   |        |        |        |
|        |        |        |        | path   |        |        |        |
|        |        |        |        | shall  |        |        |        |
|        |        |        |        | be the |        |        |        |
|        |        |        |        | Defaul |        |        |        |
|        |        |        |        | t      |        |        |        |
|        |        |        |        | starti |        |        |        |
|        |        |        |        | ng     |        |        |        |
|        |        |        |        | file   |        |        |        |
|        |        |        |        | path.  |        |        |        |
|        |        |        |        |        |        |        |        |
|        |        |        |        | The    |        |        |        |
|        |        |        |        | browse |        |        |        |
|        |        |        |        | r      |        |        |        |
|        |        |        |        | shall  |        |        |        |
|        |        |        |        | rememb |        |        |        |
|        |        |        |        | er     |        |        |        |
|        |        |        |        | the    |        |        |        |
|        |        |        |        | file   |        |        |        |
|        |        |        |        | path   |        |        |        |
|        |        |        |        | of the |        |        |        |
|        |        |        |        | parent |        |        |        |
|        |        |        |        | direct |        |        |        |
|        |        |        |        | ory    |        |        |        |
|        |        |        |        | of the |        |        |        |
|        |        |        |        | last   |        |        |        |
|        |        |        |        | opened |        |        |        |
|        |        |        |        | .pc    |        |        |        |
|        |        |        |        | file   |        |        |        |
|        |        |        |        | for    |        |        |        |
|        |        |        |        | the    |        |        |        |
|        |        |        |        | curren |        |        |        |
|        |        |        |        | t      |        |        |        |
|        |        |        |        | progra |        |        |        |
|        |        |        |        | m      |        |        |        |
|        |        |        |        | sessio |        |        |        |
|        |        |        |        | n.     |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 10     | Delete | Button |        | See    | Enable | 5      |        |
|        |        |        |        | Table  | d      |        |        |
|        |        |        |        | 4.2.6- |        |        |        |
|        |        |        |        | 2      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 11     | Detail | Button |        | See    | Enable | 6      |        |
|        |        |        |        | Table  | d      |        |        |
|        |        |        |        | 4.2.6- |        |        |        |
|        |        |        |        | 2      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 12     | Close  | Button |        |        | Enable | 7      |        |
|        |        |        |        |        | d      |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 13     | [Packa | Label  |        | Displa | Toggle |        |        |
|        | ge     |        |        | ys     | s      |        |        |
|        | Number |        |        | the    | from   |        |        |
|        | ]{.und |        |        | packag | visibl |        |        |
|        | erline |        |        | e      | e      |        |        |
|        | }      |        |        | number | to not |        |        |
|        |        |        |        | of the | visibl |        |        |
|        |        |        |        | curren | e      |        |        |
|        |        |        |        | tly    | per    |        |        |
|        |        |        |        | select | Detail |        |        |
|        |        |        |        | ed     | button |        |        |
|        |        |        |        | Plug-I | select |        |        |
|        |        |        |        | n      | ion    |        |        |
|        |        |        |        | Packag |        |        |        |
|        |        |        |        | e      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 14     | [Platf | Label  |        | Displa | Toggle |        |        |
|        | orm    |        |        | ys     | s      |        |        |
|        | Number |        |        | the    | from   |        |        |
|        | ]{.und |        |        | platfo | visibl |        |        |
|        | erline |        |        | rm     | e      |        |        |
|        | }      |        |        | number | to not |        |        |
|        |        |        |        | of the | visibl |        |        |
|        |        |        |        | curren | e      |        |        |
|        |        |        |        | tly    | per    |        |        |
|        |        |        |        | select | Detail |        |        |
|        |        |        |        | ed     | button |        |        |
|        |        |        |        | Plug-I | select |        |        |
|        |        |        |        | n      | ion    |        |        |
|        |        |        |        | Packag |        |        |        |
|        |        |        |        | e      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 15     | [SDT   | Label  |        | Displa | Toggle |        |        |
|        | IVN]{. |        |        | ys     | s      |        |        |
|        | underl |        |        | the    | from   |        |        |
|        | ine}   |        |        | SDT    | visibl |        |        |
|        |        |        |        | IVN of | e      |        |        |
|        |        |        |        | the    | to not |        |        |
|        |        |        |        | curren | visibl |        |        |
|        |        |        |        | tly    | e      |        |        |
|        |        |        |        | select | per    |        |        |
|        |        |        |        | ed     | Detail |        |        |
|        |        |        |        | Plug-I | button |        |        |
|        |        |        |        | n      | select |        |        |
|        |        |        |        | Packag | ion    |        |        |
|        |        |        |        | e      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 16     | [LSAP  | Label  |        | Displa | Toggle |        |        |
|        | IVN]{. |        |        | ys     | s      |        |        |
|        | underl |        |        | the    | from   |        |        |
|        | ine}   |        |        | LSAP   | visibl |        |        |
|        |        |        |        | IVN of | e      |        |        |
|        |        |        |        | the    | to not |        |        |
|        |        |        |        | curren | visibl |        |        |
|        |        |        |        | tly    | e      |        |        |
|        |        |        |        | select | per    |        |        |
|        |        |        |        | ed     | Detail |        |        |
|        |        |        |        | Plug-I | button |        |        |
|        |        |        |        | n      | select |        |        |
|        |        |        |        | Packag | ion    |        |        |
|        |        |        |        | e      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 17     | [HDB   | Label  |        | Displa | Toggle |        |        |
|        | Part   |        |        | ys     | s      |        |        |
|        | Number |        |        | the    | from   |        |        |
|        | ]{.und |        |        | HDB    | visibl |        |        |
|        | erline |        |        | Part   | e      |        |        |
|        | }      |        |        | Number | to not |        |        |
|        |        |        |        | of the | visibl |        |        |
|        |        |        |        | curren | e      |        |        |
|        |        |        |        | tly    | per    |        |        |
|        |        |        |        | select | Detail |        |        |
|        |        |        |        | ed     | button |        |        |
|        |        |        |        | Plug-I | select |        |        |
|        |        |        |        | n      | ion    |        |        |
|        |        |        |        | Packag |        |        |        |
|        |        |        |        | e      |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+
| 18     | Plug-I | Matrix |        | Displa | Toggle |        |        |
|        | n      |        |        | y      | s      |        |        |
|        | /      |        |        | the    | from   |        |        |
|        | Versio |        |        | versio | visibl |        |        |
|        | n      |        |        | n      | e      |        |        |
|        |        |        |        | of     | to not |        |        |
|        |        |        |        | each   | visibl |        |        |
|        |        |        |        | the    | e      |        |        |
|        |        |        |        | follow | per    |        |        |
|        |        |        |        | ing    | Detail |        |        |
|        |        |        |        | Plug-I | button |        |        |
|        |        |        |        | ns:    | select |        |        |
|        |        |        |        |        | ion    |        |        |
|        |        |        |        | SDT    |        |        |        |
|        |        |        |        | Import |        |        |        |
|        |        |        |        |        |        |        |        |
|        |        |        |        | GUI    |        |        |        |
|        |        |        |        |        |        |        |        |
|        |        |        |        | Consis |        |        |        |
|        |        |        |        | tency  |        |        |        |
|        |        |        |        | Check  |        |        |        |
|        |        |        |        |        |        |        |        |
|        |        |        |        | SDT    |        |        |        |
|        |        |        |        | Conver |        |        |        |
|        |        |        |        | ter    |        |        |        |
|        |        |        |        |        |        |        |        |
|        |        |        |        | Report |        |        |        |
+--------+--------+--------+--------+--------+--------+--------+--------+

b\. The behavior of the Screens shall be per Table 4.2.6-2.

[]{#_Toc395021816 .anchor}Table 4.2.6-2: Plug-In Packages Screens -
Behavior

  **Item \#**   **Screen Behavior**                                                                                          **Activated On**                  **Result**                                              **Model Unique**
  ------------- ------------------------------------------------------------------------------------------------------------ --------------------------------- ------------------------------------------------------- ------------------
  1             Deletion of a currently selected plug-in will cause the tool to select the next available plug-in package.   Plug-In Delete                    Deletes currently selected Plug-In                      
  2             Display only Plug-In packages associated with applicable airplane model.                                     Selected Plug-In airplane model   Limits plug-ins listed                                  
  3             Deleting Plug-In package only allowed if no database is loaded.                                              Plug-In Delete                    Displays warning dialog box per Table 5.1-1, item 4.    
  4             Prompt user when deleting a non-selected Plug-In package.                                                    Plug-In Delete                    Displays warning dialog box per Table 5.1-1, item 5.    
  5             Prompt user when deleting the currently selected Plug-In package.                                            Plug-In Delete                    Displays warning dialog box per Table 5.1-1, item 5.    
  6             A Plug-In cannot be deleted if it is the only Plug-In available.                                             Plug-In Delete                    Displays warning dialog box per Table 5.1-1, item 7.    
  7             Cannot change Plug-In if database is loaded.                                                                 Plug-In Select                    Displays warning dialog box per Table 5.1-1, item 8.    
  8             The lower portion of the screen becomes visible                                                              Detail Button                     Toggles from visible to not visible.                    
  9             Promt the user when adding an incompatible Plug-In package. See Table 4.2.6-3 for compatibility.             Plug-In Add                       Displays warning dialog box per Table 5.1-1, item 10.   

c\. The Host to Plug-In compatibility shall be per Table 4.2.6-3.

[]{#_Toc395021817 .anchor}Table 4.2.6-3: Plug-In Compatibility Matrix
Table

  **Item \#**   **Host IVN**   **Plug-In IVN**   **Model Unique**
  ------------- -------------- ----------------- ------------------
  1             1.12.x.x       2.3               747
  2             1.12.x.x       2.4               747
  3             1.13.x.x       2.5               747
  4             1.13.x.x       2.6               747
  5             1.14.x..x      2.5               747
  6             1.14.x.x       2.6               747
  7             1.14.x.x       1.1               787
  8             1.15.x.x       1.1               777x

### 4.2.7 Build LSAP Screen

Note: The Build LSAP functionality is provided in code (DLL file)
supplied by Panasonic.

a\. The Build LSAP Screen shall have the following characteristics:

1\. The Screen shall have "Release Information" as the Title Label.

2\. The Screen shall have a scrollable, editable text box.

3\. The Status Screen shall have an OK button.

4\. The Status Screen shall have a Cancel button.

> b\. The behavior of the screen shall be as follows:

1\. Opening the Screen shall display the saved Release Information stored
in the PC file.

2\. Pressing OK button shall save, and overwrite, the Release Information
to the PC file data and initiate the SDT Conversion function. (Refer to
Table 6.1-9.)

3\. Pressing Cancel button shall return to the Primary Screen without
saving the Release Information.

### 4.2.8 Compress Plug-In Package Screen

a\. The Compress Plug-In Package Screen controls shall be as defined in
Table 4.2.8-1.

[]{#_Toc395021818 .anchor}Table 4.2.8-1: Compress Plug-In Package Screen
- Components

  **Item \#**   **Label**                         **Type**      **Range**      **Details**                                                                                           **Availability**               **Tab Order**   **Model Unique**
  ------------- --------------------------------- ------------- -------------- ----------------------------------------------------------------------------------------------------- ------------------------------ --------------- ------------------
  1             Compress Plug-In Package          Label                        Screen Title; bold, underline                                                                         Always visible, not editable                   
  2             Plug-In Package Number            TextBox                                                                                                                            Always editable                1               
  3             Airplane Model                    DropListBox   B787, B747-8   Default to B747-8                                                                                     Always selectable              2               
  4             Airline Packaging                 CheckBox                     Default is unchecked                                                                                  Always selectable              3               
  5             Plug-In Package Name              TextBox                                                                                                                            Always editable                4               
  6             HDB Part Number                   TextBox                                                                                                                            Always editable                5               
  7             DLL Directory                     TextBox                                                                                                                            Always editable                6               
  8             ...                               Button                       A standard Windows OS Open File screen is used to select a directory where the dll files are stored   Enabled                        7               
  9             SDT Converter Version             TextBox                      Version number                                                                                        Always editable                8               
  10                                              TextBox                      SDT Converter name and location                                                                       Always editable                9               
  11            ...                               Button                       A standard Windows OS Open File screen is used to select a dll file (\*.dll)                          Enabled                        10              
  12            SDT Consistency Checker Version   TextBox                      Version number                                                                                        Always editable                11              
  13                                              TextBox                      SDT Consistency Checker name and location                                                             Always editable                12              
  14            ...                               Button                       A standard Windows OS Open File screen is used to select a dll file (\*.dll)                          Enabled                        13              
  15            SDT Report Generator Version      TextBox                      Version number                                                                                        Always editable                14              
  16                                              TextBox                      SDT Report Generator name and location                                                                Always editable                15              
  17            ...                               Button                       A standard Windows OS Open File screen is used to select a dll file (\*.dll)                          Enabled                        16              
  18            SDT Importer/Exporter Version     TextBox                      Version number                                                                                        Always editable                17              
  19                                              TextBox                      SDT Importer/Exporter name and location                                                               Always editable                18              
  20            ...                               Button                       A standard Windows OS Open File screen is used to select a dll file (\*.dll)                          Enabled                        19              
  21            SDT Editor Version                TextBox                      Version number                                                                                        Always editable                20              
  22                                              TextBox                      SDT Editor name and location                                                                          Always editable                21              
  23            ...                               Button                       A standard Windows OS Open File screen is used to select a dll file (\*.dll)                          Enabled                        22              
  24            Workspace Directory               TextBox                                                                                                                            Always editable                23              
  25            ...                               Button                       A standard Windows OS Open File screen is used to select the Workspace directory                      Enabled                        24              
  26            HELP file                         TextBox                      Help file name and location                                                                           Always editable                25              
  27            ...                               Button                       A standard Windows OS Open File screen is used to select a Help file (HELP\_ACDG.chm)                 Enabled                        26              
  28            Image file directory              TextBox                      Image file location                                                                                   Always editable                27              
  29            ...                               Button                       A standard Windows OS Browse For Folder screen is used to select the file directory                   Enabled                        28              
  30            Resource directory                TextBox                      Resource location                                                                                     Always editable                29              
  31            ...                               Button                       A standard Windows OS Browse For Folder screen is used to select the directory                        Enabled                        30              
  32            CDG Platform Number               TextBox                                                                                                                            Always editable                31              
  33            System Data Table IVN             TextBox                      Major number                                                                                          Always editable                32              
  34                                              TextBox                      Minor number                                                                                          Always editable                33              
  35                                              TextBox                      SDT IVN name and location                                                                             Always editable                34              
  36            ...                               Button                       A standard Windows OS Open File screen is used to select a database file (\*.accdb)                   Enabled                        35              
  37            CDB IVN                           TextBox                      Major number                                                                                          Always editable                36              
  38                                              TextBox                      Minor number                                                                                          Always editable                37              
  39            Plug-In IVN                       TextBox                      Major number                                                                                          Always editable                38              
  40                                              TextBox                      Minor number                                                                                          Always editable                39              
  41            Description                       TextBox                      Large TextBox                                                                                         Always editable                40              
  42            Compress                          Button                                                                                                                             Enabled                        41              
  43            Close                             Button                                                                                                                             Enabled                        42              

### 4.2.9 Import XML Screen

a\. The Import XML Screen shall have the following characteristics:

1\. The Screen shall be provided by the Operating System.

2\. The Screen shall only allow browsing of directory folders and the
selection of .zip files.

3\. The Screen shall remember the file path of the parent directory of
the last opened .zip file for the current program session.

4\. The Screen's starting file path shall be the Default Import XML
starting file path.

b\. The behavior of the screen shall be as follows:

1\. Pressing the Open button with a ZIP file specified shall start the
Import XML process using the specified Zip file.

2\. Pressing the Cancel button shall return to the Primary Screen without
importing a Zip file.

### 4.2.10 Export XML Screen

a\. The Export XML Screen shall have the following characteristics:

1\. The Screen shall be provided by the Operating System.

2\. The Screen shall only allow browsing of directory folders.

3\. The Screen shall remember the file path of the parent directory where
the last ZIP file was created for the current program session.

4\. The Screen's starting file path shall be the Default Export XML
starting file path.

5\. The Screen shall allow the user to make a New Folder at the specified
directory.

b\. The behavior of the screen shall be as follows:

1\. Pressing the New Folder button shall create a new folder at the
specified directory.

2\. Pressing the Open button with a directory specified shall start the
Export XML process.

3\. Pressing the Cancel button shall return the focus to the Primary
Screen without exporting a Zip file.

### 4.2.11 SDT Conversion Screen

a\. The SDT Conversion Screen shall have the following characteristics:

1\. The Screen shall use the format of the Status Screen (section 3.17)

2\. Pressing the Save button shall open a browser folder provided by the
Operating System.

3\. The browser folder shall remember the file path of the parent
directory of the last opened .zip file for the current program session.

4\. The browser folder's starting file path shall be the Default starting
file path.

### 4.2.12 CDB Consistency Check Screen

Note: The CDB Consistency Check functionality is provided in code (DLL
file) supplied by Panasonic.

a\. The CDB Consistency Check Screen shall have the following
characteristics:

1\. The Screen shall use the format of the Status Screen (section 3.17).

2\. The Screen shall call the Panasonic provided CDG DLL file to start
the CDB Consistency Check process.

b\. The behavior of the screen shall be as follows:

1\. Pressing Cancel button shall stop the CDB Consistency Check and
return to the Primary Screen.

### 4.2.13 Export CDB

Note: The Export CDB functionality is provided in code (DLL file)
supplied by Panasonic.

The Export CDB process uses two screens: the folder browser and the
Status Screen.

> a\. The Export CDB folder browser shall have the following
> characteristics:

1\. The Screen shall be provided by the Operating System.

2\. The Screen shall only allow browsing of directory folders.

3\. The Screen shall remember the file path of the parent directory
chosen for the last export during the current program session.

4\. The Screen's starting file path shall be the Default Export CDB
starting file path.

5\. The Screen shall allow the user to make a New Folder at the specified
directory.

b\. The behavior of the Export CDB folder browser shall be as follows:

1\. Pressing New Folder button will create a new folder at the specified
directory.

2\. Pressing OK button with a directory file specified shall open the
Export CDB Status screen.

3\. Pressing Cancel button shall return to the Primary Screen without
exporting CSV files.

c\. The Export CDB Status Screen shall have the following
characteristics:

1\. The screen shall use the Status Screen (section 3.17) as its base.

2\. The Title Label shall be "Export Status".

3\. The scrolling message box shall display when the host starts and
finishes exporting each CDB table.

4\. The screen shall have only a Close button.

d\. The behaviour of the Export CDB Status Screen shall be as follows:

1\. Pressing Close shall close the Export CDB Status screen and return
the user to the ACDG Host screen.

### 4.2.14 Help ACDG Screen

a\. Shall use a standard Windows OS Help screen.

b\. The Help screen shall display the user manual.

### 4.2.15 About ACDG Screen

a\. The About ACDG Screen controls shall be as defined in Table 4.2.15-1.

[]{#_Toc395021819 .anchor}Table 4.2.15-1: About ACDG Screen - Components

  **Item \#**   **Label**                                                                     **Type**   **Range**                                         **Details**                     **Availability**               **Tab Order**   **Model Unique**
  ------------- ----------------------------------------------------------------------------- ---------- ------------------------------------------------- ------------------------------- ------------------------------ --------------- ------------------
  1             Airline Configuration Database Generator (ACDG)                               Label                                                        Screen Title; bold, underline   Always visible, not editable                   
  2             ACDG Host Part Number                                                         TextBox    Part Number per Section 3.1.b                                                     Always visible, not editable                   
  3             ACDG Host Version                                                             TextBox    The Version Number of the ACDG Host Part Number                                   Always visible, not editable                   
  4             PAC CDG Part Number                                                           TextBox    The Panasonic CDG Part Number                                                                                                    
  5             Copyright © 2012 - \<current year\>The Boeing Company. All rights reserved.   Label                                                                                        Always visible, not editable                   
  6             Close                                                                         Button                                                                                       Enabled                                        

5.0 ACDG Host Screen Error/Warning Dialog Box
=============================================

When an action desired by the user requires further input, a dialog box
with a message will display. A dialog box is a modal window; that is,
the user must take the appropriate action in order to clear the dialog
box and continue.

5.1 ACDG Host Primary Screen 
-----------------------------

The dialog box requirements are described in this section. All dialog
boxes will have a title, action buttons, and message.

The requirements for the dialog boxes shall be per Table 5.1-1.

[]{#_Toc336344533 .anchor}Table 5.1-1: Screen Generated Error/Warning
Dialog Boxes

+-----------+-----------+-----------+-----------+-----------+-----------+
| **Item    | **Error/W | **Message | **Dialog  | **Resulti | **Model   |
| \#**      | arning    | Text**    | Box       | ng        | Unique**  |
|           | Number**  |           | Buttons** | Action**  |           |
+===========+===========+===========+===========+===========+===========+
| 1         | 1         | Do you    | Yes, No   | Yes --    |           |
|           |           | want to   |           | Saves     |           |
|           |           | save the  |           | Data and  |           |
|           |           | PC file?  |           | continues |           |
|           |           |           |           | the       |           |
|           |           |           |           | requested |           |
|           |           |           |           | operation |           |
|           |           |           |           |           |           |
|           |           |           |           | No --     |           |
|           |           |           |           | Executes  |           |
|           |           |           |           | the       |           |
|           |           |           |           | requested |           |
|           |           |           |           | operation |           |
|           |           |           |           | without   |           |
|           |           |           |           | saving    |           |
|           |           |           |           | the file  |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| 2         | 2         | Do you    | OK,       | OK --     |           |
|           |           | want to   | Cancel    | Saves the |           |
|           |           | override  |           | data on   |           |
|           |           | the old   |           | the       |           |
|           |           | PC File?  |           | existing  |           |
|           |           |           |           | PC File.  |           |
|           |           |           |           |           |           |
|           |           |           |           | Cancel -- |           |
|           |           |           |           | Returns   |           |
|           |           |           |           | to Main   |           |
|           |           |           |           | Screen    |           |
|           |           |           |           | without   |           |
|           |           |           |           | saving.   |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| 3         | 3         | Do you    | OK,       | OK --     |           |
|           |           | want to   | Cancel    | Saves the |           |
|           |           | override  |           | data on   |           |
|           |           | the PC    |           | the       |           |
|           |           | File?     |           | existing  |           |
|           |           |           |           | PC File.  |           |
|           |           |           |           |           |           |
|           |           |           |           | Cancel -- |           |
|           |           |           |           | Returns   |           |
|           |           |           |           | to Main   |           |
|           |           |           |           | Screen    |           |
|           |           |           |           | without   |           |
|           |           |           |           | saving.   |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| 4         | 4         | Cannot    | OK        | OK --     |           |
|           |           | delete    |           | Returns   |           |
|           |           | Plug-In   |           | to        |           |
|           |           | package   |           | previous  |           |
|           |           | because a |           | screen    |           |
|           |           | database  |           | without   |           |
|           |           | is open.  |           | deleting. |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| 5         | 5         | You are   | Yes, No   | Yes --    |           |
|           |           | about to  |           | Deletes   |           |
|           |           | Delete    |           | the       |           |
|           |           | Plug-In   |           | plug-In   |           |
|           |           | Package   |           | package.  |           |
|           |           | \[plug-in |           |           |           |
|           |           | name\].   |           | No --     |           |
|           |           | Do you    |           | Returns   |           |
|           |           | want to   |           | to        |           |
|           |           | continue? |           | previous  |           |
|           |           |           |           | screen    |           |
|           |           |           |           | without   |           |
|           |           |           |           | deleting. |           |
|           |           |           |           |           |           |
|           |           |           |           | NOTE: If  |           |
|           |           |           |           | the       |           |
|           |           |           |           | deleted   |           |
|           |           |           |           | plug-in   |           |
|           |           |           |           | package   |           |
|           |           |           |           | was the   |           |
|           |           |           |           | currently |           |
|           |           |           |           | selected  |           |
|           |           |           |           | one, the  |           |
|           |           |           |           | tool      |           |
|           |           |           |           | selects   |           |
|           |           |           |           | the next  |           |
|           |           |           |           | highest   |           |
|           |           |           |           | plug-in   |           |
|           |           |           |           | package.  |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| 6         | (Deleted) | (Deleted) | (Deleted) | (Deleted) |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| 7         | 7         | The last  | Ok        | OK --     |           |
|           |           | Plug-In   |           | Returns   |           |
|           |           | Package   |           | to        |           |
|           |           | cannot be |           | previous  |           |
|           |           | deleted.  |           | screen    |           |
|           |           |           |           | without   |           |
|           |           |           |           | deleting. |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| 8         | 8         | Cannot    | OK        | OK --     |           |
|           |           | change    |           | Returns   |           |
|           |           | Plug-In   |           | to        |           |
|           |           | package   |           | previous  |           |
|           |           | because a |           | screen    |           |
|           |           | database  |           | without   |           |
|           |           | is open.  |           | changing. |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| 9         | 9         | Current   | Yes, No   | See       |           |
|           |           | database  |           | Figure    |           |
|           |           | needs to  |           | 6.1-9.    |           |
|           |           | be saved  |           |           |           |
|           |           | before    |           |           |           |
|           |           | the LSAP  |           |           |           |
|           |           | build     |           |           |           |
|           |           | process   |           |           |           |
|           |           | can be    |           |           |           |
|           |           | performed |           |           |           |
|           |           | .         |           |           |           |
|           |           | Do you    |           |           |           |
|           |           | wish to   |           |           |           |
|           |           | Save?     |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| 10        | 10        | \[file    | OK        | OK --     |           |
|           |           | name\].   |           | Returns   |           |
|           |           | This file |           | to Main   |           |
|           |           | is        |           | Screen    |           |
|           |           | read-only |           | without   |           |
|           |           | .         |           | saving.   |           |
+-----------+-----------+-----------+-----------+-----------+-----------+
| 11        | 11        | \[Plug-In | OK        | OK --     |           |
|           |           | name\] is |           | Returns   |           |
|           |           | not       |           | to        |           |
|           |           | compatibl |           | previous  |           |
|           |           | e         |           | screen    |           |
|           |           | with the  |           | without   |           |
|           |           | host.     |           | adding.   |           |
|           |           | Cannot be |           |           |           |
|           |           | added.    |           |           |           |
+-----------+-----------+-----------+-----------+-----------+-----------+

6.0 ACDG Host Data Flow Requirements
====================================

This section depicts the data flow used in the design requirements
described on Section 4 of this document.

The legend for the shapes in the data flow diagrams are per Figure 6.0-1
below.

[]{#_Toc395021796 .anchor}Figure 6.0-1: Data Flow Diagram Legend

6.1 ACDG Host Primary Screen
----------------------------

The data flow requirements for the Primary Screen (that is, top level
screen) of the ACDG Host are described in this section.

[]{#_Toc395021797 .anchor}Figure 6.1-1: ACDG Host Primary Screen -- File
New

[]{#_Toc395021798 .anchor}Figure 6.1-2: ACDG Host Primary Screen -- File
Open

[]{#_Toc395021799 .anchor}Figure 6.1-3: ACDG Host Primary Screen -- File
Save

[]{#_Toc395021800 .anchor}Figure 6.1-4: ACDG Host Primary Screen -- File
Save As

[]{#_Toc395021801 .anchor}Figure 6.1-5: ACDG Host Primary Screen -- File
Config Info

[]{#_Toc395021802 .anchor}Figure 6.1-6: ACDG Host Primary Screen -- File
Close

[]{#_Toc395021803 .anchor}Figure 6.1-7: ACDG Host Primary Screen -- Exit

[]{#_Toc395021804 .anchor}Figure 6.1-8: ACDG Host Primary Screen --
Import XML

[]{#_Toc395021805 .anchor}Figure 6.1-9: ACDG Host Tool Primary Screen --
Build LSAP Files

Glossary
========

ACDG Airline Configuration Database Generator

CDB Configuration Database

CDG Configuration Database Generator

Config Configuration

CSS Cabin Services System

CSSC CSS Controller

GUI Graphic User Interface

HDB Health Management Database

LRU Line-Replaceable Unit

OPS Operational Program Software

References
==========

The following documents contain the requirements for the Cabin Services
System (CSS) and the Airline Configuration Database Generator (ACDG).

**Boeing Documents**

S417U920 747-8 Intercontinental Cabin Services System (CSS)
Specification Control Drawing (SCD)

S823Z101 Cabin Services System (CSS) Specification Control Drawing (SCD)
(for 787)

D620Z012-11 CSS Functional Requirements

D620Z012-12 Cabin Services System (CSS) Health Management Database (HDB)
Definition

D620Z012-13 Cabin Services System (CSS) Airline Configuration Database
Generator (ACDG) Plug-In Requirements: Editor

D620Z012-14 Cabin Services System (CSS) Airline Configuration Database
Generator (ACDG) Plug-In Requirements: Consistency Checker

D620Z012-15 Cabin Services System (CSS) Airline Configuration Database
Generator (ACDG) Plug-In Requirements: Converter

D620Z012-16 Cabin Services System (CSS) Airline Configuration Database
Generator (ACDG) Plug-In Requirements: Report Generator

D620Z012-17 Cabin Services System (CSS) Airline Configuration Database
Generator (ACDG) Plug-In Requirements: Importer/Exporter

D620Z012-18 Cabin Services System (CSS) Airline Configuration Database
Generator (ACDG) Default Data and Library Data

D620Z012-19 Cabin Services System (CSS) Airline Configuration Database
Generator (ACDG) Plug-In Requirements: Updater

D620Z012-20 Cabin Services System (CSS) Configuration Database Generator
(CDG) System Data Tables ICD

**Panasonic Documents**

810006-301 INTERFACE CONTROL DOCUMENT for Configuration Database
Generator

Revision Record
===============

  ------------------------------ ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -- ------------- -- ----------------
  **Revision Letter**            **A **                                                                                                                                                                                                                                                                                                         
  **Changes in this Revision**   This document is a complete revision. It was revised to include the Emergency Evacuation function to support the Master Change for BEJ RCO66. All other changes between this revision and the previous revision (Rev New) are function refinements/clarifications and editorial changes.                       
  **Signatures**                                                                                                                                                                                                                                                                                                                                
  AUTHOR:                                                                                                                                                                                                                                                                                                                      66-CB-E401       Aug. 5/14
                                 Mary-Ann Micale *(Signature on file)*                                                                                                                                                                                                                                                         Org. Number      Date
  REVIEWED BY:                                                                                                                                                                                                                                                                                                                 66-CB-E401       8/6/2014
                                 Steve Diehl *(Signature on file)*                                                                                                                                                                                                                                                             Org. Number      Date
  REVIEWED BY:                                                                                                                                                                                                                                                                                                                 66-CB-E401       8/6/2014
                                 Cynthia Meyer *(Signature on file)*                                                                                                                                                                                                                                                           Org. Number      Date
  REVIEWED BY:                                                                                                                                                                                                                                                                                                                 66-CB-E401       8/6/2014
                                 Martin Moy *(Signature on file)*                                                                                                                                                                                                                                                              Org. Number      Date
  REVIEWED BY:                                                                                                                                                                                                                                                                                                                 66-CB-E401       8/6/14
                                 Steve St. Onge *(Signature on file)*                                                                                                                                                                                                                                                          Org. Number      Date
  APPROVAL:                                                                                                                                                                                                                                                                                                                    66-CH-R624       8/6/14
                                 Steve McGinnis *(Signature on file)*                                                                                                                                                                                                                                                          Org. Number      Date
  APPROVAL:                                                                                                                                                                                                                                                                                                                    66-CB-E401       8/6/14
                                 Sujen Luu *(Signature on file)*                                                                                                                                                                                                                                                               Org. Number      Date
  DOCUMENT RELEASE:              Tanya G. Goody                                                                                                                                                                                                                                                                                9M-ST-EUBO       August 8, 2014
                                                                                                                                                                                                                                                                                                                               Org. Number      Date
                                                                                                                                                                                                                                                                                                                                                
  ------------------------------ ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -- ------------- -- ----------------

Revision Record
===============

  ------------------------------ --------------------------------------- -- ------------- -- ------
  **Revision Letter**            **B **                                                      
  **Changes in this Revision**   This document is a complete revision.                       
  **Signatures**                                                                             
  AUTHOR:                                                                   66-CB-E401       
                                 Mary-Ann Micale *(Signature on file)*      Org. Number      Date
  REVIEWED BY:                                                              66-CB-E401       
                                 Steve Diehl *(Signature on file)*          Org. Number      Date
  REVIEWED BY:                                                              66-CB-E401       
                                 Cynthia Meyer *(Signature on file)*        Org. Number      Date
  REVIEWED BY:                                                              66-CB-E401       
                                 Martin Moy *(Signature on file)*           Org. Number      Date
  REVIEWED BY:                                                              66-CB-E401       
                                 Steve St. Onge *(Signature on file)*       Org. Number      Date
  APPROVAL:                                                                 66-CH-R624       
                                 Steve McGinnis *(Signature on file)*       Org. Number      Date
  APPROVAL:                                                                 66-CB-E401       
                                 Sujen Luu *(Signature on file)*            Org. Number      Date
  DOCUMENT RELEASE:                                                                          
                                                                            Org. Number      Date
                                                                                             
  ------------------------------ --------------------------------------- -- ------------- -- ------
