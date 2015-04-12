# DICOMWeb
Information about DICOMWeb - API's, implementations, etc.  Pull requests are welcome!!

Information
===========


DICOM
-----
* [WG 27 meeting minutes](http://medical.nema.org/DICOM/minutes/WG-27/)
* [DICOM Strategy](http://medical.nema.org/dicom/geninfo/Strategy.pdf)
* [DICOM Standard Documents](http://dicom.nema.org/medical/dicom/current/)

Web Sites
---------
* [HCIntegrations DICOMWeb site](http://dicomweb.hcintegrations.ca/#/home)

Presentations
-------------
* [Presentation by Brad Genereaux](http://www.slideshare.net/IntegratorBrad/dicomweb)
* [Presentation by Jim Philbin](http://medical.nema.org/dicom/CP/Conference-2013/Presentations/Post-Conf-Day-1/D1-0935F-Philbin-by-Tarbox-Image%20Access%20Everywhere.pptx)

Articles
--------
* [5 Questions With Tim Dawson, Chief Architect at Vital Images](http://www.hl7standards.com/blog/2013/11/07/dicom-rs/)

Blog Posts
----------
* [Implementing QIDO-RS](http://chafey.blogspot.com/2014/05/implementing-qido-rs-service.html)
* [DICOM WADO and WADO-URI](http://chafey.blogspot.com/2014/09/dicom-wado-and-wado-uri.html)
* [WADO-RS Overview](http://chafey.blogspot.com/2014/09/wado-rs-overview.html)

Twitter Tags
------------
* [#dicomweb](https://twitter.com/search?q=%23dicomweb&src=typd)



Service Implementations
=======================

The following is a list of implementations that support DICOMWeb with detailed lists of functionality.  If you would
like to add your product to this list, email me the details.  If you would like me to verify that specific features
work, please provide access to a system for me to test.

Value | Meaning
---------------
 +    | Believed to support (not verified)
 Y    | Supported (verified by Chris Hafey)
 N    | Does not support
 ?    | Unknown support

dcm4chee
--------
* License: Open Source (Mozilla)
* Version: ?
* Last Updated: April 11, 2015
* Status: Alpha
* URL: https://github.com/dcm4che/dcm4chee-arc-cdi
* Note: Last official release was May 7, 2014 - trunk may have more functionality

### QIDO-RS

Feature                          | Supported | Notes
---------------------------------|-----------|------------------------------
application/dicom+xml            |     +     |
application/json                 |     +     |
Studies                          |     +     | Returns names not group element
Series                           |     +     |
Instances                        |     +     |
relational query                 |     ?     |
fuzzy matching                   |     ?     |
ranges                           |     +     |
includefield                     |     ?     |
sequences                        |     ?     |
limit                            |     +     |
offset                           |     +     |
dicomKeyword group element       |     ?     |
dicomKeyword name                |     ?     |
TimezoneOffsetFromUTC            |     +     |

### WADO-RS

Feature                          | Supported | Notes
---------------------------------|-----------|------------------------------
application/dicom+xml            |     +     |
application/json                 |     +     |
transfer-syntax                  |     ?     |
Retrieve Study                   |     +     |
Retrieve Series                  |     +     |
Retrieve Instance                |     +     |
Retreive Frames                  |     ?     |
Retrieve Bulkdata                |     ?     |
Retrieve Metadata                |     +     | Does not support application/json response

### STOW-RS

Feature                          | Supported | Notes
---------------------------------|-----------|------------------------------
application/dicom+xml            |      ?    |
application/json                 |      ?    |

orthanc
-------
* Core License: Open Source (GPLv3)
* Plugin License: Open Source (AGPL)
* Version:
* Last Updated: April 10, 2015
* Status: Alpha
* Core URL: http://www.orthanc-server.com/
* Plugin URL: https://bitbucket.org/sjodogne/orthanc-dicomweb/src/db07057d77ad00c60f030c83b9a970cf2cc62783?at=default

### QIDO-RS

Feature                          | Supported | Notes
---------------------------------|-----------|------------------------------
application/dicom+xml            |     +     |
application/json                 |     +     |
Studies                          |     +     |
Series                           |     +     |
Instances                        |     +     |
relational query                 |     N     |
fuzzy matching                   |     N     |
ranges                           |     +     |
includefield                     |     +     |
sequences                        |     +     |
limit                            |     +     |
offset                           |     +     |
dicomKeyword group element       |     +     |
dicomKeyword name                |     ?     |
TimezoneOffsetFromUTC            |     ?     |

### WADO-RS

Feature                          | Supported | Notes
---------------------------------|-----------|------------------------------
application/dicom+xml            |     ?     |
application/json                 |     ?     |
transfer-syntax                  |     N     |
Retrieve Study                   |     +     |
Retrieve Series                  |     +     |
Retrieve Instance                |     +     |
Retreive Frames                  |     N     |
Retrieve Bulkdata                |     N     |
Retrieve Metadata                |     N     |

### STOW-RS

Feature                          | Supported | Notes
---------------------------------|-----------|------------------------------
application/dicom+xml            |      ?    |
application/json                 |      ?    |


SimpleQIDOService
-----------------
* License: Open Source (MIT)
* Version: N/A
* Last Updated: April 10, 2015
* Status: Alpha/Prototype
* URL :https://github.com/chafey/SimpleQIDOService

### QIDO-RS

Feature                          | Supported | Notes
---------------------------------|-----------|------------------------------
application/dicom+xml            |     N     |
application/json                 |     Y     |
Studies                          |     Y     |
Series                           |     Y     |
Instances                        |     Y     |
relational query                 |     N     |
fuzzy matching                   |     N     |
ranges                           |     Y     | * limited to specific fields
includefield                     |     N     |
sequences                        |     N     |
limit                            |     Y     |
offset                           |     Y     |
dicomKeyword group element       |     Y     |
dicomKeyword name                |     N     |
TimezoneOffsetFromUTC            |     N     |

Medical Connections
-------------------
* License: Commercial
* Version: ?
* Status: Alpha
* URL: http://www.medicalconnections.co.uk/DICOM_Web_Services

### QIDO-RS

Feature                          | Supported | Notes
---------------------------------|-----------|------------------------------
application/dicom+xml            |     +     |
application/json                 |     +     |
Studies                          |     +     |
Series                           |     +     |
Instances                        |     +     |
relational query                 |     ?     |
fuzzy matching                   |     N     |
ranges                           |     +     |
includefield                     |     +     |
sequences                        |     ?     |
limit                            |     +     |
offset                           |     +     |
dicomKeyword group element       |     +     |
dicomKeyword name                |     ?     |
TimezoneOffsetFromUTC            |     N     |

### WADO-RS

Feature                          | Supported | Notes
---------------------------------|-----------|------------------------------
application/dicom+xml            |     ?     |
application/json                 |     ?     |
transfer-syntax                  |     N     |
Retrieve Study                   |     +     |
Retrieve Series                  |     +     |
Retrieve Instance                |     +     |
Retreive Frames                  |     N     |
Retrieve Bulkdata                |     N     |
Retrieve Metadata                |     N     |

### STOW-RS

Feature                          | Supported | Notes
---------------------------------|-----------|------------------------------
application/dicom+xml            |      ?    |
application/json                 |      ?    |

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

