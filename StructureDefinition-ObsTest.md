# ObsTest - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ObsTest**

## Resource Profile: ObsTest 

| | |
| :--- | :--- |
| *Official URL*:http://example.org/StructureDefinition/ObsTest | *Version*:0.1.0 |
| Draft as of 2026-03-01 | *Computable Name*:ObsTest |

**Usages:**

* This Profile is not used by any profiles in this Implementation Guide

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/fhir.example|current/StructureDefinition/ObsTest)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ObsTest.csv), [Excel](StructureDefinition-ObsTest.xlsx), [Schematron](StructureDefinition-ObsTest.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ObsTest",
  "url" : "http://example.org/StructureDefinition/ObsTest",
  "version" : "0.1.0",
  "name" : "ObsTest",
  "status" : "draft",
  "date" : "2026-03-01T20:35:21+00:00",
  "publisher" : "Example Publisher",
  "contact" : [{
    "name" : "Example Publisher",
    "telecom" : [{
      "system" : "url",
      "value" : "http://example.org/example-publisher"
    }]
  }],
  "fhirVersion" : "4.0.1",
  "mapping" : [{
    "identity" : "workflow",
    "uri" : "http://hl7.org/fhir/workflow",
    "name" : "Workflow Pattern"
  },
  {
    "identity" : "sct-concept",
    "uri" : "http://snomed.info/conceptdomain",
    "name" : "SNOMED CT Concept Domain Binding"
  },
  {
    "identity" : "v2",
    "uri" : "http://hl7.org/v2",
    "name" : "HL7 v2 Mapping"
  },
  {
    "identity" : "rim",
    "uri" : "http://hl7.org/v3",
    "name" : "RIM Mapping"
  },
  {
    "identity" : "w5",
    "uri" : "http://hl7.org/fhir/fivews",
    "name" : "FiveWs Pattern Mapping"
  },
  {
    "identity" : "sct-attr",
    "uri" : "http://snomed.org/attributebinding",
    "name" : "SNOMED CT Attribute Binding"
  }],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Observation",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Observation",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Observation",
      "path" : "Observation"
    },
    {
      "id" : "Observation.code",
      "path" : "Observation.code",
      "binding" : {
        "strength" : "required",
        "valueSet" : "http://hl7.org/fhir/uv/ips/ValueSet/current-smoking-status-uv-ips|1.1.0"
      }
    }]
  }
}

```
