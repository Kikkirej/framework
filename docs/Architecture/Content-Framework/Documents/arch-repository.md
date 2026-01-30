# Architecture Repository

This is a special "document" as it is more a storage for architecture information than a classic document. The base information is based on the [TOGAF® standard](https://publications.opengroup.org/standards/togaf/c220).

Different Flavours to handle this.

1. Simple file/files to store it in in text/markdown format.
2. Wiki based approach to store the information in a wiki system.
3. Database based approach to store the information in a database system.
4. Specialized Architecture Repository tools.
    * Archi, Sparx, etc.
5. QMS based approach to store the information in a Quality Management System.

The preffered approach for small to medium organisations is often a file based or wiki based approach.

For larger organisations or if a lot of architecture information is created a database based approach or specialized tools are often better suited.

My personal preffered approach is the tool approach, but I only have experience with Sparx Enterprise Architect here by now. 

## Structure

There are different areas which should be covered by the repository.

### Architecture Landscape

This includes per TOGAF® standard:

* Strategic Architectures
* Segment Architectures
* Capability Architectures

These I would normally put into different folders or areas of the repository, like shown on the [Overview](../index.md) page.

### Reference Library

This includes all reference information which is needed to create architectures. This can be:

| Content | Description | Storage |
|---------|-------------|----------|
| Standards Bodies | Information about standards bodies like ISO, IEEE, etc. | One versioned document |
| Product and Service Vendors | All vendor related information with a process in place to update this regularly | One database or Excel table |
| Templates | All standard templates which are used in the organisation | One folder with versioned documents |
| Enterprise Best Practice | Best practices which are used in the organisation. Process to onboard them needs to be in place | One document with descriptions |
| Reference Architectures | Reference architectures which can be used as a starting point for architecture work | One folder with versioned documents |
| Viewpoint Library | All standard viewpoints which are used in the organisation | One folder with versioned documents |

In case of a tool based approach this can be stored in the tool itself. The storage classes are rather for file systems.

### Standards Library

This includes all standards which are defined in the organisation or used by the organisation. This can be a versioned document with references.

### Governance Library

This is from my point of view one of the more interesting aspects of the repository.

| Content | Description | Storage |
|---------|-------------|----------|
| Decision Log | All architecture decisions which are made in the organisation. Need to have a process in place for making decisions | One database or Excel table |
| Compliance Assessments | All compliance assessments which are made for products or projects | One folder with the reports. This can also be connected to the product or portfolio folder |
| Capability Assessments | All capability assessments which are made | One folder with the reports. This can also be connected to the product or portfolio folder |
| Project/Product Portfolios | All products or projects which are in the organisation. This can also be connected to the capability assessments | One database or Excel table |
| Performance Measurements | All performance measurements which are made for architectures or architecture work | One database or Excel table |

## Template

A template can be found in the [TOGAF® Standard, 10th Edition Template Deliverables](https://publications.opengroup.org/i094) as "Architecture Repository" in the Preliminary Phase.