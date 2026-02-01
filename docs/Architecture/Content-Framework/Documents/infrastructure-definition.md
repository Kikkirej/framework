# Infrastructure Definition and Sizing

This is not a formal document in the TOGAF® standard, but it is important to define the infrastructure needed to support the architecture in a product organization. 

## Role/Purpose

Giving information to client or internal planners about the infrastructure needed to support the architecture.

## Content

This makes sense to have in a tabular format. Which directly enables to do sizing exercises.

### Input Data

This table should capture the input data needed for the sizing exercise. 

This can be user count, datasets, network traffic, etc. This highly depends on the used software, which product is used.

### Data Catalog

This should be referenced in a own versioned document. 

It should contain all possible options for components. These can be in different groupings. Like different vendors, different performance classes, etc.

Groups can be for example:

* Product XY - Single Server
* Product XY - Seperate Database Server
* Product XY - Clustered

The required groups should be defined in the input data section. A data catalog version should also be defined in the Input Data section.

### Output Data

This table should capture the output data of the sizing exercise. Combining Input with the Data Catalog.

The concrete sizing for the different possible values can be selected by size steps. For example: 

| User Count | Size Tier |
|------------|-----------|
| 100 Users  | Size 1    |
| 500 Users  | Size 2    |
| 1000 Users | Size 3    |
| 5000 Users | Size 4    |

Alternatively the size can be defined by a formula which uses the variables.

For Example: 

```
4 CPUs + (User Count / 100) * 2 CPUs
``` 

The formula result should be rounded. For example there should be not an uneven number of CPUs (unless it is 1) and ideally RAM is a Potence of 2 (4, 8, 16, 32, 64, ...) or set together from Potences of 2 (for example 12 GB = 8 GB + 4 GB).


## Software

I think for this a sizing software would be nice. I am not aware of any open source or free tools for this. If you know any, please let me know.