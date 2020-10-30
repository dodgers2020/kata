# ADR #1

## Architecture Characteristics

### Primary
* Feasibility - it’s a startup, funds are limited
* Reliability - customer must be able to get food at any time, and inventory must be available
* Usability - need low barrier of use to customers
* Testability - data needs to be right, otherwise poor user experience
* Maintainability - needs to be easy to maintain; probably not going to maintain full time development staff

### Secondary
* Consistency - need inventory list to be accurate
* Auditability - $ trail
* Performance - an aspect of usability; customers should not have to wait a long time to get the necessary information
* Security - handling some customer data (more important when handling health information)
* Evolvability - as the company grows the needs will expand
* Interoperability - POS software and smart fridge choice could change over time
* Extensibility - startup has lots of plans for the future; want to be able to support making meals specific to individual’s health needs

## Decision
We believe that a monolithic/layered architecture will best fulfill the criteria above.

As an early stage startup still validating product market fit, large technical investments (time and money) may reduce agility. Farmacy Foods does not have intense scaling needs and minimizing complexity will help them focus on reaching viability.
