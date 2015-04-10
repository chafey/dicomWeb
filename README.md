# DICOMWeb
Information about DICOMWeb - API's, implementations, etc.  Pull requests are welcome!!

DICOM
=====

* [WG 27 meeting minutes](http://medical.nema.org/DICOM/minutes/WG-27/)
* [DICOM Strategy](http://medical.nema.org/dicom/geninfo/Strategy.pdf)
* [DICOM Standard Documents](http://dicom.nema.org/medical/dicom/current/)

Service Implementations
=======================

dcm4chee
--------
* License: Open Source (Mozilla)
* Status: Alpha
* URL: https://github.com/dcm4che/dcm4chee-arc-cdi

APIs supported:


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
* QIDO-RS - Series
* QIDO-RS - Instances

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