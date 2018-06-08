---
title: Additional Demographics Event Message Bundle
keywords:  messaging, bundles
tags: [fhir,messaging]
sidebar: foundations_sidebar
permalink: explore_additional_demographics.html
summary: "The FHIR profiles used for the Additional Demographics Message Bundle"
---

{% include important.html content="The links below will refer to the StructureDefinition url applied to the FHIR profile, which are not yet active. For queries please refer to the Help and Support section." %} 

The following FHIR profiles are used to form the Additional Demographics Event Message Bundle:

- [DM-Bundle-1](https://fhir.nhs.uk/STU3/StructureDefinition/DM-Bundle-1)
- [DM-MessageHeader-1](https://fhir.nhs.uk/STU3/StructureDefinition/DM-MessageHeader-1) - where the coding and display elements for the 'event' type are fixed to '001 - Additional Demographics'
- [CareConnect-DM-Organization-1](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-DM-Organization-1)
- [DM-HealthcareService-1](https://fhir.nhs.uk/STU3/StructureDefinition/DM-HealthcareService-1)
- [CareConnect-DM-Patient-1](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-DM-Patient-1)
- [CareConnect-DM-Encounter-1](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-DM-Encounter-1)
- [CareConnect-DM-Location-1](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-DM-Location-1)
                                                                                                   
### Additional Demographics Event data item mapping to FHIR profiles ###

The Child Health Event data items are fulfilled by elements within the FHIR resources listed below:

| DM Data Item            | FHIR resource element                                 | Mandatory/Required/Optional |
|--------------------------|-------------------------------------------------------|-----------------------------|
| Local Patient Identifier | CareConnect-DM-Patient-1.identifier (localIdentifier) | Mandatory                   |
| Town of Birth            | CareConnect-DM-Patient-1.birthPlace                  | Required                    |
| Country of Birth         | CareConnect-DM-Patient-1.birthPlace                  | Required                    |
| Communication Preference | CareConnect-DM-Patient-1.telecom.system              | Required                    |
| Patient email address    | CareConnect-DM-Patient-1.telecom.value               | Required                    |
| Ethnicity                | CareConnect-DM-Patient-1.ethnicCategory              | Required                    |
| Religion                 | CareConnect-DM-Patient-1.religiousAffiliation        | Required                    |
| Marital Status		   | CareConnect-DM-Patient-1.maritalStatus				   | Required					 |

