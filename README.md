# DICOMWeb
Information about DICOMWeb - API's, implementations, etc.  Pull requests are welcome!!

DICOM
=====

* [WG 27 meeting minutes](http://medical.nema.org/DICOM/minutes/WG-27/)
* [DICOM Strategy](http://medical.nema.org/dicom/geninfo/Strategy.pdf)
* [DICOM Standard Documents](http://dicom.nema.org/medical/dicom/current/)
* [HCIntegrations DICOMWeb site](http://dicomweb.hcintegrations.ca/#/home)
* [Presentation by Brad Genereaux](http://www.slideshare.net/IntegratorBrad/dicomweb)
* [Presentation by Jim Philbin](http://medical.nema.org/dicom/CP/Conference-2013/Presentations/Post-Conf-Day-1/D1-0935F-Philbin-by-Tarbox-Image%20Access%20Everywhere.pptx)

Service Implementations
=======================

dcm4chee
--------
* License: Open Source (Mozilla)
* Version: ?
* Last Updated: April 11, 2015
* Status: Alpha
* URL: https://github.com/dcm4che/dcm4chee-arc-cdi
* Note: Last official release was May 7, 2014 - trunk may have more functionality

APIs supported:
* QIDO-RS - Studies
  * Not standards compliant - returns fields by name, not group/element
* QIDO-RS - Series
  * ?
* QIDO-RS - Instances
  * ?
* WADO-RS - Retrieve Study
  * Does not support application/json
* WADO-RS - Retrieve Series
  * ?
* WADO-RS - Retrieve Instance
  * ?
* WADO-RS - Retrieve Frames
  * ?
* WADO-RS - Retrieve Bulkdata
  * ?
* WADO-RS - Retrieve Metadata
  * Not supported
* STOW-RS
  * ?

orthanc
-------
* Core License: Open Source (GPLv3)
* Plugin License: Open Source (AGPL)
* Version:
* Last Updated: April 10, 2015
* Status: Alpha
* Core URL: http://www.orthanc-server.com/
* Plugin URL: https://bitbucket.org/sjodogne/orthanc-dicomweb/src/db07057d77ad00c60f030c83b9a970cf2cc62783?at=default

APIs supported:

* QIDO-RS - Studies
  * Does not support relational queries
  * Does not support fuzzy matching
* QIDO-RS - Series
* QIDO-RS - Instances
* WADO-RS - Retrieve Study
  * Does not support transfer syntaxes
  * Does not support application/json
* WADO-RS - Retrieve Series
  * Does not support transfer syntaxes
* WADO-RS - Retrieve Instance
  * Does not support transfer syntaxes
* WADO-RS - Retrieve Frames
  * Not supported
* WADO-RS - Retrieve Bulkdata
  * Not supported
* WADO-RS - Retrieve Metadata
  * Not supported
* STOW-RS

SimpleQIDOService
-----------------
* License: Open Source (MIT)
* Version: N/A
* Last Updated: April 10, 2015
* Status: Alpha/Prototype
* URL :https://github.com/chafey/SimpleQIDOService

APIs supported:

* QIDO-RS - Studies
  * Does not support relational queries
  * Does not support application/dicom+xml response
  * Does not support fuzzy matching
  * Does not support includefield=all
  * Limited support for wildcard matching
  * Does not support sequence elements
* QIDO-RS - Series
  * Limited support for wildcard matching
* QIDO-RS - Instances
  * Limited support for wildcard matching

Medical Connections
-------------------
* License: Commercial
* Version: ?
* Status: Alpha
* URL: http://www.medicalconnections.co.uk/DICOM_Web_Services

API's Supported:
* QIDO-RS - Studies
  * Does not support TimezoneOffsetFromUTC
  * Does not support fuzzy matching
* QIDO-RS - Series
* QIDO-RS - Instances
* WADO-RS - Retrieve Study
  * Does not support transfer syntaxes
* WADO-RS - Retrieve Series
  * Does not support transfer syntaxes
* WADO-RS - Retrieve Instance
  * Does not support transfer syntaxes
* WADO-RS - Retrieve Frames
  * Not implemented
* WADO-RS - Retrieve Bulkdata
* WADO-RS - Retrieve Metadata
* STOW-RS
  * Does not support transfer syntaxes

dicomsystems
------------
* License: Commercial
* Version: ?
* Last Updated: April 10, 2015
* Status: ?

Agfa
----
* License: Commercial
* Version: ?
* Last Updated: April 10, 2015
* Status: Demo QIDO-RS at SIIM 2014 Hackathon

McKesson
--------
* License: Commercial
* Version: ?
* Last Updated: April 10, 2015
* Status: Demo QIDO-RS at SIIM 2014 Hackathon

Vital Images
------------
* License: Commercial
* Version: ?
* Last Updated: April 10, 2015
* Status: Demo STOW-RS at SIIM 2014 Hackathon


Client Implementations
=======================

cornerstoneQIDOWorklist
-----------------------
* License: Open Source (MIT)
* Version: N/A
* Last Updated: April 10, 2015
* Status: Alpha/Prototype
* URL: https://github.com/chafey/cornerstoneQIDORSWorklist

API's used:
* QIDO-RS - Studies