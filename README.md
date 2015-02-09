## Specialty Integer Workspace Objects ##

The **Specialty Integer Workspace Objects** add-on allows users to display numeric integer data using non-decimal radices such as binary, octal, and hexadecimal.

These numeric representations are typically used when such formats are easier to interpret or manipulate than standard decimal numerics. Common use cases include displaying virtual memory address information, error codes, digital port values, instrument commands, bitpacked Boolean data, and various other applications. This is not possible without using the free label custom object framework due to the fact that the default configuration options for numeric objects will supersede any in-VI property modifications, precluding the use of specialty integer formats not compatible with the double precision floating decimal data type.

This library includes the following objects:

- Numeric Control Integer
- Numeric Indicator Integer

These objects are configurable to display values in:

- Decimal
- Hexadecimal
- Binary
- Octal
- Scientific Notation
- Engineering Notation

### LabVIEW Version ###

LabVIEW 2012

### Built Availability ###

No builds are provided.

### Quality, Limitations ###

This add-on is loosely based on the [Numeric Indicator MinMax Latching](https://github.com/NIVeriStandAdd-Ons/Numeric-Indicator-MinMax-Latching) add-on, therefore it inherits its quality and limitations however - it has been updated some since it was written in 2012. 

There are no known users of the IP. Proceed with caution.

### Dependencies ###

Moore Good Ideas (MGI) Library is used to scan for and convert NaN values to zeroes before converting to integers, this LabVIEW add-on is available here. If you do not wish to install the library, the missing subVI can be removed or re-implemented, if removed this will cause the objects to display the maximum possible value rather than zero if a channel returns NaN (such as when no system definition is deployed.)

### License ###

*This repository and any materials provided by NI therein are provided AS IS. NI DISCLAIMS ANY AND ALL LIABILITIES FOR AND MAKES NO WARRANTIES, EITHER EXPRESS OR IMPLIED, INCLUDING WITHOUT LIMITATION ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR  PARTICULAR PURPOSE, OR NON-INFRINGEMENT OF INTELLECTUAL PROPERTY. NI shall have no liability for any direct, indirect, incidental, punitive, special, or consequential damages for your use of the repository or any materials contained therein.*