# acpi_tables

## Design

This crate provides the ability to generate static tables (e.g. FADT/FACP,
MCFG, etc) as well as generate AML for filling a DSDT table.

## Usage

There are thirteen modules:

* `aml` provides the ability to generate AML code, see the chapter titled "ACPI
  Machine Language (AML) Specification" in the ACPI Specification.
* `cedt` contains routines for creating a `CEDT` table (see the CXL specification
  for more details)
* `facs` contains routines for creating a `FACS` table
* `fadt` contains routines for creating a `FADT` table (also known as FACP)
* `madt` contains routines for creating an `MADT` table (also known as APIC)
* `mcfg` contains routines for creating an `MCFG` table
* `pptt` contains routines for creating a `PPTT` table
* `rhct` contains routines for creating a `RHCT` table
* `rsdp` contains a helper for creating a `RSDP` table
* `sdt` provides the ability to build user defined tables including header and
  checksum validation
* `slit` contains routines for creating a `SLIT` table
* `srat` contains routines for creating a `SRAT` table
* `xsdt` contains routines for creating an `XSDT` table

## Examples

The crate is currently used by the Cloud Hypervisor project so detailed
examples of populating different ACPI table types can be found there.


## Licence

This crate is licensed under the Apache 2.0 licence. The full text can be found
in the LICENSE-APACHE file.
