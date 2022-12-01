# Geocode-Service
The Geocode Service provides geocoding and reverse-geocoding. This web service provides two functions:

*	Geocode: which takes a PIDF LO, as described in RFC 4119, and updated by RFC 5139 and RFC 5491, which contains a civic address, and returns a PIDF LO containing a geodetic representation for the same location.
* ReverseGeocode: which takes a PIDF LO as described in RFC 4119 and updated by RFC 5139 and RFC 5491, which contains a geodetic representation, and returns a PIDF LO that contains a civic address for the same location.

The Geocode Service is provisioned using the same mechanism as is used to provision the ECRF and LVF: layer replication from the master SI. The layers include all of the layers to create a PIDF LO. 

Any conversion, and specifically geocoding and reverse geocoding, can introduce errors. Unless the underlying SI provides very accurate polygons to represent all civic locations precisely, the conversion is complicated by the inherent uncertainty of the measurements and the “nearest” point algorithm employed. Users of these transformation services should be aware of the limitations of the geocoding and reverse geocoding mechanisms. Reverse geocoding is typically less accurate than geocoding, although some error and unquantified uncertainty is inherent in both.

## Owner

The owner of this repository approves all changes to the repository. 

This repository is owned by the NENA Core Services Committee, i3 Architecture working group.

#### Rules:

Specification Required. 

#### Contact:

[https://www.nena.org/page/911CoreSvcs](https://www.nena.org/page/911CoreSvcs) 

## Version History

### Geocode Conversion Service v 1.0

Version 1 OpenAPI schema for this service was originally defined in NENA-STA-010.3.2021. See https://www.nena.org/page/i3_Stage
