# PSD2 specifications

openAPI 3.0 for PSD2 based on the [Berlin Group specifications](https://www.berlin-group.org/nextgenpsd2-downloads "Berling Group downloads")

Please note that the `psd2_swagger2.yaml` file is the result of an automatic conversion using APIMATIC. Unfortunatly this process is not working perfectly, and some features of the 3.0 spec may not be reliably transfered to the 2.0 one.

## Changes

- 2018-06-01: `0.0.1`
  - inital version implementing the basic endpoint structure

- 2018-06-21: `0.0.2`
  - corrected security schema
  - removed http protocol
  - added global tag definition

- 2018-06-23: `0.0.3`
  - defined the different variations for handling the SCA process
  - merged the endpoint for PIS of the different payment-services into one
  - added a definition for all HTTP status codes in the specification
  - defined the HTTP status codes specifically for the various endpoints
  - added the header definitions for the PSU related informations
  - defined schemas for request and response bodies relevant for the SCA process
  - added a few more regex validations
  - fixed several minor errors

## TODO
- add more regex validations
- add request body examples for the PIS calls
- check the application/XML variants of the calls
- add more descriptions for the various schema and parameter definitions

## Validation
We are using [speccy](https://www.npmjs.com/package/speccy "speccy") for linting and validation.

`speccy lint psd2.yaml`



