# Commercial Fishing RFC

This repository is intended to propose and discuss standards for interoperability of commercial fishery data for the purposes of data transfer and software component portability between fisheries.

# Formats

The following parent formats are recommended unless precluded by specific needs.

## CSV

CSV (Comma Separated Values) is a generic tabular data format, specified in [RFC 4180](https://tools.ietf.org/html/rfc4180). CSV is likely the most common format currently in use for fisheries data interoperability. For interoperability, CSV should be preferred to proprietary tabular formats such as Microsoft Excel (XLS) because the latter is not available on many systems. It's typically trivial to convert from a proprietary tabular format to CSV, but the reverse many not be true for all stakeholders.

## JSON

[JSON](http://json.org/) is an open, generic heirarchically structured format. It's typically used in modern web application APIs. It presents advantages including:

* Built in parsers for many technologies and programming languages.
* Quickly becoming industry standard for modern HTTP APIs.
* Includes a [schema notation](http://json-schema.org/), allowing precise specification of structure for interoperability.
* Designed for extensibility - new attributes can be ignored by legacy systems unlike CSV.
