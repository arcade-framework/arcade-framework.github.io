## Open PCA Pump

- The Open Patient Controlled Analgesic (PCA) Pump project provides open source design artifacts
for a realistic a PCA Pump. 
- Link: [http://openpcapump.santoslab.org/](http://openpcapump.santoslab.org/)

Open PCA Pump is used to deliver analgesic in a clinical setting:

![](Imagem1.jpg)

Example of real PCA Pump:

![](Imagem2.jpg)

Open PCA Pump architecture overview:

![](Imagem3.jpg)

### Adapted dataset represented in ARCADE interchange format

```turtle
@prefix : <dare:arcade/sao#> .
@prefix sao: <dare:arcade/sao#> .
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xml: <http://www.w3.org/XML/1998/namespace> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .

<dare:arcade/sao> rdf:type owl:Ontology ;
                           owl:imports <dare:0.1> .
:OPENPCAB-81 rdf:type owl:NamedIndividual .
:OPENPCAB-81 rdf:type sao:Requirement .
:OPENPCAB-81 rdfs:label "PCA Pump Interfaces" .
:OPENPCAB-81 rdfs:comment "Sensors, actuators, alarms." .
:OPENPCAB-81 sao:status "To Do" .
:OPENPCAB-81 sao:creationdate "2023-05-09T09:14:26.424-0300" .
:OPENPCAB-81 sao:lastupdate "2023-05-09T09:14:28.081-0300" .
:OPENPCAB-81 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-81" .
:OPENPCAB-81 sao:isRefinedBy :OPENPCAB-64 .
:OPENPCAB-81 sao:isRefinedBy :OPENPCAB-66 .
:OPENPCAB-81 sao:isRefinedBy :OPENPCAB-68 .
:OPENPCAB-80 rdf:type owl:NamedIndividual .
:OPENPCAB-80 rdf:type sao:Requirement .
:OPENPCAB-80 rdfs:label "Max dose warning" .
:OPENPCAB-80 rdfs:comment "Clinician-commanded bolus shall be halted when continuing to infuse exceeds prescribed volume of drug infused over a period of time (ml/hr). Pump rate shall be reduced to KVO and a max dose warning be issued." .
:OPENPCAB-80 sao:status "To Do" .
:OPENPCAB-80 sao:creationdate "2023-05-09T09:14:24.792-0300" .
:OPENPCAB-80 sao:lastupdate "2023-05-09T09:14:26.591-0300" .
:OPENPCAB-80 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-80" .
:OPENPCAB-80 sao:refines :OPENPCAB-34 .
:OPENPCAB-79 rdf:type owl:NamedIndividual .
:OPENPCAB-79 rdf:type sao:Requirement .
:OPENPCAB-79 rdfs:label "Minimum clinician-chosen duration" .
:OPENPCAB-79 rdfs:comment "The minimum clinician-chosen duration for a clinician-requested bolus shall be the prescribed minimum number of minutes between consecutive patient-requested bolus deliveries, Δprb." .
:OPENPCAB-79 sao:status "To Do" .
:OPENPCAB-79 sao:creationdate "2023-05-09T09:14:22.546-0300" .
:OPENPCAB-79 sao:lastupdate "2023-05-09T09:14:24.578-0300" .
:OPENPCAB-79 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-79" .
:OPENPCAB-79 sao:refines :OPENPCAB-34 .
:OPENPCAB-78 rdf:type owl:NamedIndividual .
:OPENPCAB-78 rdf:type sao:Requirement .
:OPENPCAB-78 rdfs:label "Maximum clinician-chosen duration" .
:OPENPCAB-78 rdfs:comment "The maximum clinician-chosen duration for a clinician-requested bolus shall be Δccb max = 6 hours." .
:OPENPCAB-78 sao:status "To Do" .
:OPENPCAB-78 sao:creationdate "2023-05-09T09:14:20.713-0300" .
:OPENPCAB-78 sao:lastupdate "2023-05-09T09:14:22.359-0300" .
:OPENPCAB-78 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-78" .
:OPENPCAB-78 sao:refines :OPENPCAB-34 .
:OPENPCAB-77 rdf:type owl:NamedIndividual .
:OPENPCAB-77 rdf:type sao:Requirement .
:OPENPCAB-77 rdfs:label "Alarm halts clinician-requested bolus" .
:OPENPCAB-77 rdfs:comment "Any alarm halts clinician-requested bolus delivery either halting pump or switching to KVO rate." .
:OPENPCAB-77 sao:status "To Do" .
:OPENPCAB-77 sao:creationdate "2023-05-09T09:14:18.945-0300" .
:OPENPCAB-77 sao:lastupdate "2023-05-09T09:14:20.950-0300" .
:OPENPCAB-77 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-77" .
:OPENPCAB-77 sao:refines :OPENPCAB-34 .
:OPENPCAB-76 rdf:type owl:NamedIndividual .
:OPENPCAB-76 rdf:type sao:Requirement .
:OPENPCAB-76 rdfs:label "Patient-requested bolus takes precedence" .
:OPENPCAB-76 rdfs:comment "A patient-requested bolus takes precedence over a clinician-requested bolus. The clinician-requested bolus shall be suspended while the patient-requested bolus dose is administered, and resumed afterward." .
:OPENPCAB-76 sao:status "To Do" .
:OPENPCAB-76 sao:creationdate "2023-05-09T09:14:17.154-0300" .
:OPENPCAB-76 sao:lastupdate "2023-05-09T09:14:19.022-0300" .
:OPENPCAB-76 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-76" .
:OPENPCAB-76 sao:refines :OPENPCAB-34 .
:OPENPCAB-75 rdf:type owl:NamedIndividual .
:OPENPCAB-75 rdf:type sao:Requirement .
:OPENPCAB-75 rdfs:label "Delivery of clinician-requested bolus" .
:OPENPCAB-75 rdfs:comment "A clinician-requested bolus shall be delivered at the rate, Fccb, of VTBI divided by the duration chosen by the clinician, Δccb, in addition to the prescribed basal ﬂow rate, Fbasal, but no more than the maximum ﬂow rate for the pump, Fmax." .
:OPENPCAB-75 sao:status "To Do" .
:OPENPCAB-75 sao:creationdate "2023-05-09T09:14:15.169-0300" .
:OPENPCAB-75 sao:lastupdate "2023-05-09T09:14:17.106-0300" .
:OPENPCAB-75 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-75" .
:OPENPCAB-75 sao:refines :OPENPCAB-34 .
:OPENPCAB-74 rdf:type owl:NamedIndividual .
:OPENPCAB-74 rdf:type sao:Requirement .
:OPENPCAB-74 rdfs:label "Alarm stops patient-requested bolus" .
:OPENPCAB-74 rdfs:comment "Any alarm stops patient-requested bolus delivery either halting pump or switching to KVO rate." .
:OPENPCAB-74 sao:status "To Do" .
:OPENPCAB-74 sao:creationdate "2023-05-09T09:14:13.516-0300" .
:OPENPCAB-74 sao:lastupdate "2023-05-09T09:14:15.323-0300" .
:OPENPCAB-74 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-74" .
:OPENPCAB-74 sao:refines :OPENPCAB-36 .
:OPENPCAB-73 rdf:type owl:NamedIndividual .
:OPENPCAB-73 rdf:type sao:Requirement .
:OPENPCAB-73 rdfs:label "Max dose warning" .
:OPENPCAB-73 rdfs:comment "Patient-requested bolus shall not be delivered if infusing prescribed VTBI will exceed hard limits retrieved from the drug library for the volume of drug infused over a period of time. Pump rate shall be reduced to KVO and a max dose warning be issued." .
:OPENPCAB-73 sao:status "To Do" .
:OPENPCAB-73 sao:creationdate "2023-05-09T09:14:12.006-0300" .
:OPENPCAB-73 sao:lastupdate "2023-05-09T09:14:13.695-0300" .
:OPENPCAB-73 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-73" .
:OPENPCAB-73 sao:refines :OPENPCAB-36 .
:OPENPCAB-72 rdf:type owl:NamedIndividual .
:OPENPCAB-72 rdf:type sao:Requirement .
:OPENPCAB-72 rdfs:label "Basal ﬂow rate" .
:OPENPCAB-72 rdfs:comment "The basal ﬂow rate, Fbasal, is prescribed by a physician, and entered into the PCA pump by scanning the prescription from the drug container label as it is loaded into the reservoir." .
:OPENPCAB-72 sao:status "To Do" .
:OPENPCAB-72 sao:creationdate "2023-05-09T09:14:10.158-0300" .
:OPENPCAB-72 sao:lastupdate "2023-05-09T09:14:12.178-0300" .
:OPENPCAB-72 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-72" .
:OPENPCAB-72 sao:refines :OPENPCAB-18 .
:OPENPCAB-71 rdf:type owl:NamedIndividual .
:OPENPCAB-71 rdf:type sao:Requirement .
:OPENPCAB-71 rdfs:label "PCA pump performs intended function" .
:OPENPCAB-71 rdfs:comment "The high-level goals (G) of the PCA pump are:
G0 The pump will safely infuse drugs intravenously for pain relief.
G1 The patient should receive enough drug to reduce his pain.
G2 The patient should not receive so much drug that makes him unaware, or is harmful.
G3 Clinician(s) should be notiﬁed upon occurrence of hazardous conditions, unless alarms have been inactivated.
G4 The PCA pump should detect the smallest-possible air-in-line embolism (bubble) and halt the infusion drug.
G5 The PCA pump should infuse safely when failures occur or hazards are detected
G6 Patients should receive the drug as prescribed by their physician, administered by appropriate
clinicians.
G7 Patient’s health information should be available to those caring for the patient, and only those." .
:OPENPCAB-71 sao:status "To Do" .
:OPENPCAB-71 sao:creationdate "2023-05-09T09:14:08.027-0300" .
:OPENPCAB-71 sao:lastupdate "2023-05-09T09:14:10.475-0300" .
:OPENPCAB-71 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-71" .
:OPENPCAB-71 sao:isRefinedBy :OPENPCAB-18 .
:OPENPCAB-71 sao:isRefinedBy :OPENPCAB-34 .
:OPENPCAB-71 sao:isRefinedBy :OPENPCAB-36 .
:OPENPCAB-71_justification rdf:type owl:NamedIndividual .
:OPENPCAB-71_justification rdf:type sao:Justification .
:OPENPCAB-71_justification sao:explains :OPENPCAB-71 .
:OPENPCAB-71 sao:isExplainedBy :OPENPCAB-71_justification .
:OPENPCAB-71_justification rdfs:label "Divide into individual behaviors, and then argue their composition has intended function" .
:OPENPCAB-71_assumption rdf:type owl:NamedIndividual .
:OPENPCAB-71_assumption rdf:type sao:Assumption .
:OPENPCAB-71_assumption sao:explains :OPENPCAB-71 .
:OPENPCAB-71 sao:isExplainedBy :OPENPCAB-71_assumption .
:OPENPCAB-71_assumption rdfs:label "Individual behaviors, and intended function, as defined in Requirements" .
:OPENPCAB-70 rdf:type owl:NamedIndividual .
:OPENPCAB-70 rdf:type sao:Hazard .
:OPENPCAB-70 rdfs:label "Reverse ﬂow hazard" .
:OPENPCAB-70 rdfs:comment "Retrograde Flow of Infusate. Potential causes: The pump is positioned much lower than the infusion site, causing the pump to siphon; or The delivery path is damaged, creating a vent on the path that diverts an intentional drug flow from reaching the user." .
:OPENPCAB-70 sao:status "To Do" .
:OPENPCAB-70 sao:creationdate "2023-05-09T09:14:06.146-0300" .
:OPENPCAB-70 sao:lastupdate "2023-05-09T09:14:07.897-0300" .
:OPENPCAB-70 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-70" .
:OPENPCAB-70 sao:isMitigatedBy :OPENPCAB-68 .
:OPENPCAB-70 sao:isMitigatedBy :OPENPCAB-69 .
:OPENPCAB-70_justification rdf:type owl:NamedIndividual .
:OPENPCAB-70_justification rdf:type sao:Justification .
:OPENPCAB-70_justification sao:explains :OPENPCAB-70 .
:OPENPCAB-70 sao:isExplainedBy :OPENPCAB-70_justification .
:OPENPCAB-70_justification rdfs:label "Rely on mechanical design of pumping mechanism" .
:OPENPCAB-69 rdf:type owl:NamedIndividual .
:OPENPCAB-69 rdf:type sao:Requirement .
:OPENPCAB-69 rdfs:label "Continuous reverse delivery" .
:OPENPCAB-69 rdfs:comment "During normal use and/or single fault condition of the equipment, continuous reverse delivery
shall not be possible." .
:OPENPCAB-69 sao:status "To Do" .
:OPENPCAB-69 sao:creationdate "2023-05-09T09:14:03.533-0300" .
:OPENPCAB-69 sao:lastupdate "2023-05-09T09:14:07.151-0300" .
:OPENPCAB-69 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-69" .
:OPENPCAB-69 sao:mitigates :OPENPCAB-70 .
:OPENPCAB-68 rdf:type owl:NamedIndividual .
:OPENPCAB-68 rdf:type sao:Requirement .
:OPENPCAB-68 rdfs:label "Reverse ﬂow" .
:OPENPCAB-68 rdfs:comment "The mechanical pump shall not allow reverse ﬂow from the patient into the pump." .
:OPENPCAB-68 sao:status "To Do" .
:OPENPCAB-68 sao:creationdate "2023-05-09T09:14:01.855-0300" .
:OPENPCAB-68 sao:lastupdate "2023-05-09T09:14:27.166-0300" .
:OPENPCAB-68 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-68" .
:OPENPCAB-68 sao:mitigates :OPENPCAB-70 .
:OPENPCAB-68 sao:refines :OPENPCAB-81 .
:OPENPCAB-67 rdf:type owl:NamedIndividual .
:OPENPCAB-67 rdf:type sao:Requirement .
:OPENPCAB-67 rdfs:label "Air-in-line alarm" .
:OPENPCAB-67 rdfs:comment "An air-in-line alarm shall be triggered by the pump if detectable air bubbles are infused into the patient." .
:OPENPCAB-67 sao:status "To Do" .
:OPENPCAB-67 sao:creationdate "2023-05-09T09:13:59.855-0300" .
:OPENPCAB-67 sao:lastupdate "2023-05-09T09:14:01.639-0300" .
:OPENPCAB-67 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-67" .
:OPENPCAB-67 sao:mitigates :OPENPCAB-23 .
:OPENPCAB-67 sao:refines :OPENPCAB-25 .
:OPENPCAB-66 rdf:type owl:NamedIndividual .
:OPENPCAB-66 rdf:type sao:Requirement .
:OPENPCAB-66 rdfs:label "Detect air-in-line embolism" .
:OPENPCAB-66 rdfs:comment "The PCA pump shall detect air-in-line embolism (bubble)." .
:OPENPCAB-66 sao:status "To Do" .
:OPENPCAB-66 sao:creationdate "2023-05-09T09:13:57.483-0300" .
:OPENPCAB-66 sao:lastupdate "2023-05-09T09:14:27.269-0300" .
:OPENPCAB-66 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-66" .
:OPENPCAB-66 sao:mitigates :OPENPCAB-23 .
:OPENPCAB-66 sao:refines :OPENPCAB-81 .
:OPENPCAB-65 rdf:type owl:NamedIndividual .
:OPENPCAB-65 rdf:type sao:Strategy .
:OPENPCAB-65 rdfs:label "Mitigations of external and internal air in line hazards differ" .
:OPENPCAB-65 rdfs:comment "Argue for mitigation of internal and external causes  of air in line separately" .
:OPENPCAB-65 sao:status "To Do" .
:OPENPCAB-65 sao:creationdate "2023-05-09T09:13:55.633-0300" .
:OPENPCAB-65 sao:lastupdate "2023-05-09T09:13:57.317-0300" .
:OPENPCAB-65 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-65" .
:OPENPCAB-65 sao:explains :OPENPCAB-23 .
:OPENPCAB-64 rdf:type owl:NamedIndividual .
:OPENPCAB-64 rdf:type sao:Requirement .
:OPENPCAB-64 rdfs:label "Halt pumping" .
:OPENPCAB-64 rdfs:comment "The mechanical pump shall halt pumping when commanded, or caused in response to an alarm condition.(many EC)" .
:OPENPCAB-64 sao:status "To Do" .
:OPENPCAB-64 sao:creationdate "2023-05-09T09:13:53.440-0300" .
:OPENPCAB-64 sao:lastupdate "2023-05-09T09:14:27.234-0300" .
:OPENPCAB-64 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-64" .
:OPENPCAB-64 sao:mitigates :OPENPCAB-21 .
:OPENPCAB-64 sao:refines :OPENPCAB-81 .
:OPENPCAB-64 sao:isAllocatedIn :Component10036 .
:Component10036 sao:allocates :OPENPCAB-64 .
:OPENPCAB-63 rdf:type owl:NamedIndividual .
:OPENPCAB-63 rdf:type sao:Requirement .
:OPENPCAB-63 rdfs:label "Square bolus under-infusion warning" .
:OPENPCAB-63 rdfs:comment "If delivered clinician-requested bolus ﬂow rate is less than the calculated square bolus rate by more than its allowed tolerance over a period of more than 5 minutes, or immediately if the ﬂow stops, the pump shall issue a square bolus under-infusion warning." .
:OPENPCAB-63 sao:status "To Do" .
:OPENPCAB-63 sao:creationdate "2023-05-09T09:13:50.365-0300" .
:OPENPCAB-63 sao:lastupdate "2023-05-09T09:13:52.135-0300" .
:OPENPCAB-63 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-63" .
:OPENPCAB-63 sao:mitigates :OPENPCAB-43 .
:OPENPCAB-63 sao:isAllocatedIn :Component10035 .
:Component10035 sao:allocates :OPENPCAB-63 .
:OPENPCAB-62 rdf:type owl:NamedIndividual .
:OPENPCAB-62 rdf:type sao:Requirement .
:OPENPCAB-62 rdfs:label "Square bolus over-infusion alarm" .
:OPENPCAB-62 rdfs:comment "If delivered clinician-requested bolus ﬂow rate exceeds the calculated square bolus rate by more than its allowed tolerance over a period of more than 5 minutes, or immediately if the pump goes into free ﬂow, the pump shall issue a square bolus over-infusion alarm." .
:OPENPCAB-62 sao:status "To Do" .
:OPENPCAB-62 sao:creationdate "2023-05-09T09:13:47.727-0300" .
:OPENPCAB-62 sao:lastupdate "2023-05-09T09:13:49.507-0300" .
:OPENPCAB-62 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-62" .
:OPENPCAB-62 sao:mitigates :OPENPCAB-43 .
:OPENPCAB-62 sao:isAllocatedIn :Component10035 .
:Component10035 sao:allocates :OPENPCAB-62 .
:OPENPCAB-61 rdf:type owl:NamedIndividual .
:OPENPCAB-61 rdf:type sao:Requirement .
:OPENPCAB-61 rdfs:label "Bolus under-infusion warning" .
:OPENPCAB-61 rdfs:comment "If delivered patient-requested bolus ﬂow rate is less than the prescribed bolus rate setting by more than its allowed tolerance over a period of more than 1 minutes, or immediately if the ﬂow stops, the pump shall issue a bolus under-infusion warning." .
:OPENPCAB-61 sao:status "To Do" .
:OPENPCAB-61 sao:creationdate "2023-05-09T09:13:45.830-0300" .
:OPENPCAB-61 sao:lastupdate "2023-05-09T09:13:47.757-0300" .
:OPENPCAB-61 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-61" .
:OPENPCAB-61 sao:mitigates :OPENPCAB-43 .
:OPENPCAB-61 sao:isAllocatedIn :Component10035 .
:Component10035 sao:allocates :OPENPCAB-61 .
:OPENPCAB-60 rdf:type owl:NamedIndividual .
:OPENPCAB-60 rdf:type sao:Requirement .
:OPENPCAB-60 rdfs:label "Bolus over-infusion alarm" .
:OPENPCAB-60 rdfs:comment "If delivered patient-requested bolus ﬂow rate exceeds the prescribed patient-requested bolus rate setting by more than its allowed tolerance over a period of more than 1 minutes, or immediately if the pump goes into free ﬂow, the pump shall issue a bolus over-infusion alarm." .
:OPENPCAB-60 sao:status "To Do" .
:OPENPCAB-60 sao:creationdate "2023-05-09T09:13:43.829-0300" .
:OPENPCAB-60 sao:lastupdate "2023-05-09T09:13:45.902-0300" .
:OPENPCAB-60 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-60" .
:OPENPCAB-60 sao:mitigates :OPENPCAB-43 .
:OPENPCAB-60 sao:isAllocatedIn :Component10035 .
:Component10035 sao:allocates :OPENPCAB-60 .
:OPENPCAB-59 rdf:type owl:NamedIndividual .
:OPENPCAB-59 rdf:type sao:Requirement .
:OPENPCAB-59 rdfs:label "Basal under-infusion warning" .
:OPENPCAB-59 rdfs:comment "If delivered basal ﬂow rate is less than the prescribed basal rate setting by more than its allowed tolerance over a period of more than 5 minutes, or immediately if the ﬂow stops, the pump shall issue an basal under-infusion warning." .
:OPENPCAB-59 sao:status "To Do" .
:OPENPCAB-59 sao:creationdate "2023-05-09T09:13:42.143-0300" .
:OPENPCAB-59 sao:lastupdate "2023-05-09T09:13:43.840-0300" .
:OPENPCAB-59 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-59" .
:OPENPCAB-59 sao:mitigates :OPENPCAB-43 .
:OPENPCAB-59 sao:isAllocatedIn :Component10035 .
:Component10035 sao:allocates :OPENPCAB-59 .
:OPENPCAB-58 rdf:type owl:NamedIndividual .
:OPENPCAB-58 rdf:type sao:Requirement .
:OPENPCAB-58 rdfs:label "Basal over-infusion alarm" .
:OPENPCAB-58 rdfs:comment "If delivered basal ﬂow rate exceeds the prescribed basal rate setting by more than its allowed tolerance over a period of more than 5 minutes, or immediately if the pump goes into free ﬂow, the pump shall issue an basal over-infusion alarm" .
:OPENPCAB-58 sao:status "To Do" .
:OPENPCAB-58 sao:creationdate "2023-05-09T09:13:39.977-0300" .
:OPENPCAB-58 sao:lastupdate "2023-05-09T09:13:41.707-0300" .
:OPENPCAB-58 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-58" .
:OPENPCAB-58 sao:mitigates :OPENPCAB-43 .
:OPENPCAB-58 sao:isAllocatedIn :Component10035 .
:Component10035 sao:allocates :OPENPCAB-58 .
:OPENPCAB-57 rdf:type owl:NamedIndividual .
:OPENPCAB-57 rdf:type sao:DesignDefinition .
:OPENPCAB-57 rdfs:label "Safety architecture specification" .
:OPENPCAB-57 rdfs:comment "Generic Patient Controlled Analgesic Infusion Architectural Model Description" .
:OPENPCAB-57 sao:status "To Do" .
:OPENPCAB-57 sao:creationdate "2023-05-09T09:13:37.314-0300" .
:OPENPCAB-57 sao:lastupdate "2023-05-09T09:13:40.484-0300" .
:OPENPCAB-57 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-57" .
:OPENPCAB-57 sao:realizes :OPENPCAB-52 .
:Source10021 rdf:type owl:NamedIndividual .
:Source10021 rdf:type sao:Source .
:OPENPCAB-57 sao:isDocumentedBy :Source10021 .
:Source10021 rdfs:comment "Attachment" .
:Source10021 rdfs:label "Generic Patient Controlled Analgesic Infusion Architectural Model Description.pdf" .
:Source10021 sao:externaluri "https://arcade-dare.atlassian.net/rest/api/3/attachment/content/10021" .
:Source10021 sao:creationdate "2023-05-09T09:13:39.259-0300" .
:OPENPCAB-56 rdf:type owl:NamedIndividual .
:OPENPCAB-56 rdf:type sao:Context .
:OPENPCAB-56 rdfs:label "Generic Patient Controlled Analgesia Pump Hazard Analysis " .
:OPENPCAB-56 sao:status "To Do" .
:OPENPCAB-56 sao:creationdate "2023-05-09T09:13:35.528-0300" .
:OPENPCAB-56 sao:lastupdate "2023-05-09T09:13:38.643-0300" .
:OPENPCAB-56 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-56" .
:OPENPCAB-56 sao:contextualizes :OPENPCAB-21 .
:OPENPCAB-56 sao:contextualizes :OPENPCAB-22 .
:OPENPCAB-56 sao:contextualizes :OPENPCAB-23 .
:OPENPCAB-56 sao:contextualizes :OPENPCAB-43 .
:OPENPCAB-56 sao:contextualizes :OPENPCAB-44 .
:OPENPCAB-56 sao:contextualizes :OPENPCAB-53 .
:Source10020 rdf:type owl:NamedIndividual .
:Source10020 rdf:type sao:Source .
:OPENPCAB-56 sao:isDocumentedBy :Source10020 .
:Source10020 rdfs:comment "Attachment" .
:Source10020 rdfs:label "Hazard_Analysis_GPCA.pdf" .
:Source10020 sao:externaluri "https://arcade-dare.atlassian.net/rest/api/3/attachment/content/10020" .
:Source10020 sao:creationdate "2023-05-09T09:13:37.636-0300" .
:OPENPCAB-55 rdf:type owl:NamedIndividual .
:OPENPCAB-55 rdf:type sao:Context .
:OPENPCAB-55 rdfs:label "Open PCA Pump Architecture Overview" .
:OPENPCAB-55 sao:status "To Do" .
:OPENPCAB-55 sao:creationdate "2023-05-09T09:13:33.631-0300" .
:OPENPCAB-55 sao:lastupdate "2023-05-09T09:13:37.527-0300" .
:OPENPCAB-55 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-55" .
:Source10019 rdf:type owl:NamedIndividual .
:Source10019 rdf:type sao:Source .
:OPENPCAB-55 sao:isDocumentedBy :Source10019 .
:Source10019 rdfs:comment "Attachment" .
:Source10019 rdfs:label "PCA-Pump--Architecture-Overview.pdf" .
:Source10019 sao:externaluri "https://arcade-dare.atlassian.net/rest/api/3/attachment/content/10019" .
:Source10019 sao:creationdate "2023-05-09T09:13:36.137-0300" .
:OPENPCAB-54 rdf:type owl:NamedIndividual .
:OPENPCAB-54 rdf:type sao:Context .
:OPENPCAB-54 rdfs:label "Open PCA Pump Requirements Specification" .
:OPENPCAB-54 sao:status "To Do" .
:OPENPCAB-54 sao:creationdate "2023-05-09T09:13:31.928-0300" .
:OPENPCAB-54 sao:lastupdate "2023-05-09T09:13:35.399-0300" .
:OPENPCAB-54 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-54" .
:OPENPCAB-54 sao:contextualizes :OPENPCAB-18 .
:Source10018 rdf:type owl:NamedIndividual .
:Source10018 rdf:type sao:Source .
:OPENPCAB-54 sao:isDocumentedBy :Source10018 .
:Source10018 rdfs:comment "Attachment" .
:Source10018 rdfs:label "Open-PCA-Pump-Requirements.pdf" .
:Source10018 sao:externaluri "https://arcade-dare.atlassian.net/rest/api/3/attachment/content/10018" .
:Source10018 sao:creationdate "2023-05-09T09:13:33.877-0300" .
:OPENPCAB-53 rdf:type owl:NamedIndividual .
:OPENPCAB-53 rdf:type sao:Hazard .
:OPENPCAB-53 rdfs:label "System failure" .
:OPENPCAB-53 sao:status "To Do" .
:OPENPCAB-53 sao:creationdate "2023-05-09T09:13:30.175-0300" .
:OPENPCAB-53 sao:lastupdate "2023-05-09T09:13:36.306-0300" .
:OPENPCAB-53 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-53" .
:OPENPCAB-53 sao:isContextualizedBy :OPENPCAB-56 .
:OPENPCAB-53 sao:isMitigatedBy :OPENPCAB-52 .
:OPENPCAB-53_assumption rdf:type owl:NamedIndividual .
:OPENPCAB-53_assumption rdf:type sao:Assumption .
:OPENPCAB-53_assumption sao:explains :OPENPCAB-53 .
:OPENPCAB-53 sao:isExplainedBy :OPENPCAB-53_assumption .
:OPENPCAB-53_assumption rdfs:label "Separate safety architecture detects and mitigates faults in operation" .
:OPENPCAB-52 rdf:type owl:NamedIndividual .
:OPENPCAB-52 rdf:type sao:Requirement .
:OPENPCAB-52 rdfs:label "Safety architecture separates normal operation from fault detection and response" .
:OPENPCAB-52 rdfs:comment "The PCA pump shall implement a safety architecture that separates normal operation from fault
detection and response." .
:OPENPCAB-52 sao:status "To Do" .
:OPENPCAB-52 sao:creationdate "2023-05-09T09:13:28.225-0300" .
:OPENPCAB-52 sao:lastupdate "2023-05-09T09:13:38.249-0300" .
:OPENPCAB-52 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-52" .
:OPENPCAB-52 sao:mitigates :OPENPCAB-53 .
:OPENPCAB-52 sao:isRealizedBy :OPENPCAB-57 .
:OPENPCAB-51 rdf:type owl:NamedIndividual .
:OPENPCAB-51 rdf:type sao:Context .
:OPENPCAB-51 rdfs:label "IEC 60601-2-24" .
:OPENPCAB-51 rdfs:comment "IEC 60601-2-24 Particular Requirements for safety of infusion pumps and controllers" .
:OPENPCAB-51 sao:status "To Do" .
:OPENPCAB-51 sao:creationdate "2023-05-09T09:13:26.264-0300" .
:OPENPCAB-51 sao:lastupdate "2023-05-09T09:13:27.961-0300" .
:OPENPCAB-51 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-51" .
:OPENPCAB-50 rdf:type owl:NamedIndividual .
:OPENPCAB-50 rdf:type sao:Context .
:OPENPCAB-50 rdfs:label "SAE International AS5506B" .
:OPENPCAB-50 rdfs:comment "SAE International AS5506B Architecture Analysis & Design Language (AADL)" .
:OPENPCAB-50 sao:status "To Do" .
:OPENPCAB-50 sao:creationdate "2023-05-09T09:13:24.436-0300" .
:OPENPCAB-50 sao:lastupdate "2023-05-09T09:13:26.172-0300" .
:OPENPCAB-50 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-50" .
:OPENPCAB-49 rdf:type owl:NamedIndividual .
:OPENPCAB-49 rdf:type sao:Context .
:OPENPCAB-49 rdfs:label "IEC 60601-1-2 (2001)" .
:OPENPCAB-49 rdfs:comment "IEC 60601-1-2 (2001) Medical Electrical Equipment, Part 1: General Requirements for Safety, 2. Collateral Standard: Electromagnetic Compatibility - Requirements and Tests" .
:OPENPCAB-49 sao:status "To Do" .
:OPENPCAB-49 sao:creationdate "2023-05-09T09:13:22.415-0300" .
:OPENPCAB-49 sao:lastupdate "2023-05-09T09:13:24.317-0300" .
:OPENPCAB-49 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-49" .
:OPENPCAB-48 rdf:type owl:NamedIndividual .
:OPENPCAB-48 rdf:type sao:Context .
:OPENPCAB-48 rdfs:label "IEC 60601-1" .
:OPENPCAB-48 rdfs:comment "IEC 60601-1 Collateral Standard: Safety requirements for medical electrical systems" .
:OPENPCAB-48 sao:status "To Do" .
:OPENPCAB-48 sao:creationdate "2023-05-09T09:13:20.451-0300" .
:OPENPCAB-48 sao:lastupdate "2023-05-09T09:13:22.266-0300" .
:OPENPCAB-48 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-48" .
:OPENPCAB-47 rdf:type owl:NamedIndividual .
:OPENPCAB-47 rdf:type sao:Context .
:OPENPCAB-47 rdfs:label "IEC 60601-1 (1988)" .
:OPENPCAB-47 rdfs:comment "IEC 60601-1 (1988) Medical electrical equipment Part 1: General requirements for safety, including Amendment 1 (1991) and Amendment 2 (1995) for Type B equipment" .
:OPENPCAB-47 sao:status "To Do" .
:OPENPCAB-47 sao:creationdate "2023-05-09T09:13:18.514-0300" .
:OPENPCAB-47 sao:lastupdate "2023-05-09T09:13:20.286-0300" .
:OPENPCAB-47 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-47" .
:OPENPCAB-46 rdf:type owl:NamedIndividual .
:OPENPCAB-46 rdf:type sao:Context .
:OPENPCAB-46 rdfs:label "IEC 60601-1-8" .
:OPENPCAB-46 rdfs:comment "IEC 60601-1-8 Medical electrical equipment Part 1-8: General requirements for basic safety and essential performance Collateral Standard: General requirements, tests and guidance for alarm systems in medical electrical equipment and medical electrical systems" .
:OPENPCAB-46 sao:status "To Do" .
:OPENPCAB-46 sao:creationdate "2023-05-09T09:13:16.943-0300" .
:OPENPCAB-46 sao:lastupdate "2023-05-09T09:13:18.631-0300" .
:OPENPCAB-46 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-46" .
:OPENPCAB-45 rdf:type owl:NamedIndividual .
:OPENPCAB-45 rdf:type sao:Context .
:OPENPCAB-45 rdfs:label "ASTM International F2761-09" .
:OPENPCAB-45 rdfs:comment "ASTM International F2761-09 Medical Devices and Medical Systems–Essential safety requirements for equipment comprising the patient-centric integrated clinical environment (ICE)–Part 1 General requirements and conceptual model" .
:OPENPCAB-45 sao:status "To Do" .
:OPENPCAB-45 sao:creationdate "2023-05-09T09:13:15.199-0300" .
:OPENPCAB-45 sao:lastupdate "2023-05-09T09:13:17.052-0300" .
:OPENPCAB-45 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-45" .
:OPENPCAB-44 rdf:type owl:NamedIndividual .
:OPENPCAB-44 rdf:type sao:Hazard .
:OPENPCAB-44 rdfs:label "Too Many User Boluses Hazard" .
:OPENPCAB-44 rdfs:comment "Excessive bolus administration due to too many bolus requests from the user. The bolus history records are corrupted,  making the user unable to track previously received boluses." .
:OPENPCAB-44 sao:status "To Do" .
:OPENPCAB-44 sao:creationdate "2023-05-09T09:13:12.941-0300" .
:OPENPCAB-44 sao:lastupdate "2023-05-09T09:13:36.476-0300" .
:OPENPCAB-44 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-44" .
:OPENPCAB-44 sao:isContextualizedBy :OPENPCAB-56 .
:OPENPCAB-44 sao:isCausedBy :OPENPCAB-32 .
:OPENPCAB-44 sao:isCausedBy :OPENPCAB-34 .
:OPENPCAB-44 sao:isCausedBy :OPENPCAB-36 .
:OPENPCAB-44 sao:isCausedBy :OPENPCAB-39 .
:OPENPCAB-44 sao:isMitigatedBy :OPENPCAB-38 .
:OPENPCAB-43 rdf:type owl:NamedIndividual .
:OPENPCAB-43 rdf:type sao:Hazard .
:OPENPCAB-43 rdfs:label "Uneven delivery hazard" .
:OPENPCAB-43 rdfs:comment "The programmed bolus dose is delivered unevenly over its specified duration. Potential causes: Algorithmic errors, The pump motor does not operate as intended." .
:OPENPCAB-43 sao:status "To Do" .
:OPENPCAB-43 sao:creationdate "2023-05-09T09:13:11.110-0300" .
:OPENPCAB-43 sao:lastupdate "2023-05-09T09:13:51.167-0300" .
:OPENPCAB-43 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-43" .
:OPENPCAB-43 sao:isContextualizedBy :OPENPCAB-56 .
:OPENPCAB-43 sao:isCausedBy :OPENPCAB-32 .
:OPENPCAB-43 sao:isExplainedBy :OPENPCAB-41 .
:OPENPCAB-43 sao:isMitigatedBy :OPENPCAB-58 .
:OPENPCAB-43 sao:isMitigatedBy :OPENPCAB-59 .
:OPENPCAB-43 sao:isMitigatedBy :OPENPCAB-60 .
:OPENPCAB-43 sao:isMitigatedBy :OPENPCAB-61 .
:OPENPCAB-43 sao:isMitigatedBy :OPENPCAB-62 .
:OPENPCAB-43 sao:isMitigatedBy :OPENPCAB-63 .
:OPENPCAB-43_assumption rdf:type owl:NamedIndividual .
:OPENPCAB-43_assumption rdf:type sao:Assumption .
:OPENPCAB-43_assumption sao:explains :OPENPCAB-43 .
:OPENPCAB-43 sao:isExplainedBy :OPENPCAB-43_assumption .
:OPENPCAB-43_assumption rdfs:label "Alarming upon uneven delivery stops flow and hails clinician." .
:OPENPCAB-42 rdf:type owl:NamedIndividual .
:OPENPCAB-42 rdf:type sao:SafetyRequirement .
:OPENPCAB-42 rdfs:label "Basal infusion flow range" .
:OPENPCAB-42 rdfs:comment "The pump shall be able to deliver basal infusion at ﬂows throughout the basal infusion ﬂow range of min = 1ml/hour to max =10 ml/hour." .
:OPENPCAB-42 sao:status "To Do" .
:OPENPCAB-42 sao:creationdate "2023-05-09T09:13:09.438-0300" .
:OPENPCAB-42 sao:lastupdate "2023-05-09T09:13:11.113-0300" .
:OPENPCAB-42 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-42" .
:OPENPCAB-42 sao:refines :OPENPCAB-18 .
:OPENPCAB-42 sao:isAllocatedIn :Component10032 .
:Component10032 sao:allocates :OPENPCAB-42 .
:OPENPCAB-42_justification rdf:type owl:NamedIndividual .
:OPENPCAB-42_justification rdf:type sao:Justification .
:OPENPCAB-42_justification sao:explains :OPENPCAB-42 .
:OPENPCAB-42 sao:isExplainedBy :OPENPCAB-42_justification .
:OPENPCAB-42_justification rdfs:label "Users cannot bypass software limits on dose parameters." .
:OPENPCAB-41 rdf:type owl:NamedIndividual .
:OPENPCAB-41 rdf:type sao:Strategy .
:OPENPCAB-41 rdfs:label "Measure drug flow and alarm" .
:OPENPCAB-41 rdfs:comment "Measure drug flow and alarm if measurement differs from intended flow rate by more than allowed tolerance." .
:OPENPCAB-41 sao:status "To Do" .
:OPENPCAB-41 sao:creationdate "2023-05-09T09:13:07.537-0300" .
:OPENPCAB-41 sao:lastupdate "2023-05-09T09:13:12.219-0300" .
:OPENPCAB-41 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-41" .
:OPENPCAB-41 sao:explains :OPENPCAB-43 .
:OPENPCAB-40 rdf:type owl:NamedIndividual .
:OPENPCAB-40 rdf:type sao:SafetyRequirement .
:OPENPCAB-40 rdfs:label "Basal infusion flow tolerance" .
:OPENPCAB-40 rdfs:comment "The pump shall deliver basal infusion at the prescribed basal rate within a basal infusion ﬂow tolerance of tolerance = 0.5 ml/hour of the prescribed basal rate." .
:OPENPCAB-40 sao:status "To Do" .
:OPENPCAB-40 sao:creationdate "2023-05-09T09:13:05.793-0300" .
:OPENPCAB-40 sao:lastupdate "2023-05-09T09:13:07.461-0300" .
:OPENPCAB-40 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-40" .
:OPENPCAB-40 sao:refines :OPENPCAB-18 .
:OPENPCAB-40 sao:isAllocatedIn :Component10032 .
:Component10032 sao:allocates :OPENPCAB-40 .
:OPENPCAB-40_justification rdf:type owl:NamedIndividual .
:OPENPCAB-40_justification rdf:type sao:Justification .
:OPENPCAB-40_justification sao:explains :OPENPCAB-40 .
:OPENPCAB-40 sao:isExplainedBy :OPENPCAB-40_justification .
:OPENPCAB-40_justification rdfs:label "the tolerance of rate is adequated to avoid under and over-delivery of drug." .
:OPENPCAB-39 rdf:type owl:NamedIndividual .
:OPENPCAB-39 rdf:type sao:Requirement .
:OPENPCAB-39 rdfs:label "Delivery of patient-requested bolus" .
:OPENPCAB-39 rdfs:comment "A patient-requested bolus shall be delivered at its prescribed rate, Fbolus, in addition to the prescribed basal ﬂow rate, Fbasal, but no more than the maximum ﬂow rate for the pump, Fmax." .
:OPENPCAB-39 sao:status "To Do" .
:OPENPCAB-39 sao:creationdate "2023-05-09T09:13:02.460-0300" .
:OPENPCAB-39 sao:lastupdate "2023-05-09T09:13:13.838-0300" .
:OPENPCAB-39 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-39" .
:OPENPCAB-39 sao:causes :OPENPCAB-44 .
:OPENPCAB-39 sao:refines :OPENPCAB-36 .
:OPENPCAB-39 sao:isAllocatedIn :Component10026 .
:Component10026 sao:allocates :OPENPCAB-39 .
:OPENPCAB-38 rdf:type owl:NamedIndividual .
:OPENPCAB-38 rdf:type sao:SafetyRequirement .
:OPENPCAB-38 rdfs:label "Minimum time between patient-request bolus" .
:OPENPCAB-38 rdfs:comment "Patient-requested bolus shall not be delivered more often than a prescribed minimum time between patient-requested bolus." .
:OPENPCAB-38 sao:status "To Do" .
:OPENPCAB-38 sao:creationdate "2023-05-09T09:13:00.162-0300" .
:OPENPCAB-38 sao:lastupdate "2023-05-09T09:13:13.780-0300" .
:OPENPCAB-38 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-38" .
:OPENPCAB-38 sao:mitigates :OPENPCAB-44 .
:OPENPCAB-38 sao:refines :OPENPCAB-36 .
:OPENPCAB-38 sao:isAllocatedIn :Component10034 .
:Component10034 sao:allocates :OPENPCAB-38 .
:OPENPCAB-38_justification rdf:type owl:NamedIndividual .
:OPENPCAB-38_justification rdf:type sao:Justification .
:OPENPCAB-38_justification sao:explains :OPENPCAB-38 .
:OPENPCAB-38 sao:isExplainedBy :OPENPCAB-38_justification .
:OPENPCAB-38_justification rdfs:label "Enforcing minimum time between boluses prevents too many user boluses, avoiding overinfusion." .
:OPENPCAB-37 rdf:type owl:NamedIndividual .
:OPENPCAB-37 rdf:type sao:SafetyRequirement .
:OPENPCAB-37 rdfs:label "Maximum VTBI" .
:OPENPCAB-37 rdfs:comment "Prescribed VTBI and rate shall not exceed the maximum VTBI limit set by the drug library from the hospital pharmacy for the drug loaded in the PCA pump." .
:OPENPCAB-37 sao:status "To Do" .
:OPENPCAB-37 sao:creationdate "2023-05-09T09:12:56.613-0300" .
:OPENPCAB-37 sao:lastupdate "2023-05-09T09:12:58.576-0300" .
:OPENPCAB-37 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-37" .
:OPENPCAB-37 sao:refines :OPENPCAB-36 .
:OPENPCAB-37 sao:isAllocatedIn :Component10032 .
:Component10032 sao:allocates :OPENPCAB-37 .
:OPENPCAB-37_justification rdf:type owl:NamedIndividual .
:OPENPCAB-37_justification rdf:type sao:Justification .
:OPENPCAB-37_justification sao:explains :OPENPCAB-37 .
:OPENPCAB-37 sao:isExplainedBy :OPENPCAB-37_justification .
:OPENPCAB-37_justification rdfs:label "Upon a patient-requested dose, the maximum flow rate is checked." .
:OPENPCAB-36 rdf:type owl:NamedIndividual .
:OPENPCAB-36 rdf:type sao:Requirement .
:OPENPCAB-36 rdfs:label "Patient-Requested Bolus" .
:OPENPCAB-36 rdfs:comment "Upon patient’s press of the PCA pump’s patient-button, a prescribed bolus volume-to-be-infused, VTBI, of the drug loaded in the pump is delivered to the patient." .
:OPENPCAB-36 sao:status "To Do" .
:OPENPCAB-36 sao:creationdate "2023-05-09T09:12:54.472-0300" .
:OPENPCAB-36 sao:lastupdate "2023-05-09T09:14:14.342-0300" .
:OPENPCAB-36 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-36" .
:OPENPCAB-36 sao:causes :OPENPCAB-44 .
:OPENPCAB-36 sao:refines :OPENPCAB-71 .
:OPENPCAB-36 sao:isRefinedBy :OPENPCAB-37 .
:OPENPCAB-36 sao:isRefinedBy :OPENPCAB-38 .
:OPENPCAB-36 sao:isRefinedBy :OPENPCAB-39 .
:OPENPCAB-36 sao:isRefinedBy :OPENPCAB-73 .
:OPENPCAB-36 sao:isRefinedBy :OPENPCAB-74 .
:OPENPCAB-35 rdf:type owl:NamedIndividual .
:OPENPCAB-35 rdf:type sao:Requirement .
:OPENPCAB-35 rdfs:label "Patient authentication" .
:OPENPCAB-35 rdfs:comment "Patient’s identity and admittance to the hospital must be authenticated." .
:OPENPCAB-35 sao:status "To Do" .
:OPENPCAB-35 sao:creationdate "2023-05-09T09:12:51.894-0300" .
:OPENPCAB-35 sao:lastupdate "2023-05-09T09:12:53.897-0300" .
:OPENPCAB-35 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-35" .
:OPENPCAB-35 sao:isAllocatedIn :Component10029 .
:Component10029 sao:allocates :OPENPCAB-35 .
:OPENPCAB-34 rdf:type owl:NamedIndividual .
:OPENPCAB-34 rdf:type sao:Requirement .
:OPENPCAB-34 rdfs:label "Clinician-requested bolus" .
:OPENPCAB-34 rdfs:comment "A clinician observing the discomfort of the patient may command the PCA pump to deliver a dose of the same volume-to-be-infused as patient-requested dose over a period of time chosen by the clinician." .
:OPENPCAB-34 sao:status "To Do" .
:OPENPCAB-34 sao:creationdate "2023-05-09T09:12:49.204-0300" .
:OPENPCAB-34 sao:lastupdate "2023-05-09T09:14:25.562-0300" .
:OPENPCAB-34 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-34" .
:OPENPCAB-34 sao:causes :OPENPCAB-44 .
:OPENPCAB-34 sao:refines :OPENPCAB-71 .
:OPENPCAB-34 sao:isRefinedBy :OPENPCAB-75 .
:OPENPCAB-34 sao:isRefinedBy :OPENPCAB-76 .
:OPENPCAB-34 sao:isRefinedBy :OPENPCAB-77 .
:OPENPCAB-34 sao:isRefinedBy :OPENPCAB-78 .
:OPENPCAB-34 sao:isRefinedBy :OPENPCAB-79 .
:OPENPCAB-34 sao:isRefinedBy :OPENPCAB-80 .
:OPENPCAB-34 sao:isAllocatedIn :Component10026 .
:Component10026 sao:allocates :OPENPCAB-34 .
:OPENPCAB-33 rdf:type owl:NamedIndividual .
:OPENPCAB-33 rdf:type sao:Strategy .
:OPENPCAB-33 rdfs:label "Detect occlusion and stop pump" .
:OPENPCAB-33 rdfs:comment "Stopping pump upon occlusion is safe." .
:OPENPCAB-33 sao:status "To Do" .
:OPENPCAB-33 sao:creationdate "2023-05-09T09:12:47.722-0300" .
:OPENPCAB-33 sao:lastupdate "2023-05-09T09:12:49.300-0300" .
:OPENPCAB-33 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-33" .
:OPENPCAB-33 sao:explains :OPENPCAB-21 .
:OPENPCAB-32 rdf:type owl:NamedIndividual .
:OPENPCAB-32 rdf:type sao:Requirement .
:OPENPCAB-32 rdfs:label "Clinician starts/stops pump" .
:OPENPCAB-32 rdfs:comment "The basal ﬂow rate prescribed by a physician, and entered into the PCA pump by scanning the prescription from the drug container label as it is loaded into the reservoir. Clinician start pumps after configuring basal flow rate." .
:OPENPCAB-32 sao:status "To Do" .
:OPENPCAB-32 sao:creationdate "2023-05-09T09:12:46.112-0300" .
:OPENPCAB-32 sao:lastupdate "2023-05-09T09:13:13.887-0300" .
:OPENPCAB-32 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-32" .
:OPENPCAB-32 sao:causes :OPENPCAB-43 .
:OPENPCAB-32 sao:causes :OPENPCAB-44 .
:OPENPCAB-32 sao:isAllocatedIn :Component10026 .
:Component10026 sao:allocates :OPENPCAB-32 .
:OPENPCAB-31 rdf:type owl:NamedIndividual .
:OPENPCAB-31 rdf:type sao:SafetyRequirement .
:OPENPCAB-31 rdfs:label "Soft limit conﬁrmation" .
:OPENPCAB-31 rdfs:comment "Prescriptions that violate the soft limits of the drug in the drug library shall issue a visible and audible warning requiring a soft limit conﬁrmation by the clinician." .
:OPENPCAB-31 sao:status "To Do" .
:OPENPCAB-31 sao:creationdate "2023-05-09T09:12:44.388-0300" .
:OPENPCAB-31 sao:lastupdate "2023-05-09T09:12:45.993-0300" .
:OPENPCAB-31 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-31" .
:OPENPCAB-31 sao:isAllocatedIn :Component10026 .
:Component10026 sao:allocates :OPENPCAB-31 .
:OPENPCAB-31_assumption rdf:type owl:NamedIndividual .
:OPENPCAB-31_assumption rdf:type sao:Assumption .
:OPENPCAB-31_assumption sao:explains :OPENPCAB-31 .
:OPENPCAB-31 sao:isExplainedBy :OPENPCAB-31_assumption .
:OPENPCAB-31_assumption rdfs:label "User confirmation reduces error in parameters entry." .
:OPENPCAB-30 rdf:type owl:NamedIndividual .
:OPENPCAB-30 rdf:type sao:SafetyRequirement .
:OPENPCAB-30 rdfs:label "Hard limit rejection" .
:OPENPCAB-30 rdfs:comment "Prescriptions that violate a hard limit of the drug in the drug library shall be rejected with visible and audible indication when conﬁrmation is attempted by the clinician." .
:OPENPCAB-30 sao:status "To Do" .
:OPENPCAB-30 sao:creationdate "2023-05-09T09:12:42.632-0300" .
:OPENPCAB-30 sao:lastupdate "2023-05-09T09:12:44.414-0300" .
:OPENPCAB-30 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-30" .
:OPENPCAB-30 sao:isAllocatedIn :Component10026 .
:Component10026 sao:allocates :OPENPCAB-30 .
:OPENPCAB-30_justification rdf:type owl:NamedIndividual .
:OPENPCAB-30_justification rdf:type sao:Justification .
:OPENPCAB-30_justification sao:explains :OPENPCAB-30 .
:OPENPCAB-30 sao:isExplainedBy :OPENPCAB-30_justification .
:OPENPCAB-30_justification rdfs:label "Users cannot bypass limits on dose parameters." .
:OPENPCAB-29 rdf:type owl:NamedIndividual .
:OPENPCAB-29 rdf:type sao:SafetyRequirement .
:OPENPCAB-29 rdfs:label "Upstream occlusion alarm" .
:OPENPCAB-29 rdfs:comment "An upstream occlusion alarm shall be triggered when the pump senses an upstream (drug reservoir side) occlusion exceeding 1 psi." .
:OPENPCAB-29 sao:status "To Do" .
:OPENPCAB-29 sao:creationdate "2023-05-09T09:12:40.808-0300" .
:OPENPCAB-29 sao:lastupdate "2023-05-09T09:12:42.588-0300" .
:OPENPCAB-29 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-29" .
:OPENPCAB-29 sao:mitigates :OPENPCAB-21 .
:OPENPCAB-29 sao:refines :OPENPCAB-25 .
:OPENPCAB-29 sao:isAllocatedIn :Component10033 .
:Component10033 sao:allocates :OPENPCAB-29 .
:OPENPCAB-29_assumption rdf:type owl:NamedIndividual .
:OPENPCAB-29_assumption rdf:type sao:Assumption .
:OPENPCAB-29_assumption sao:explains :OPENPCAB-29 .
:OPENPCAB-29 sao:isExplainedBy :OPENPCAB-29_assumption .
:OPENPCAB-29_assumption rdfs:label "Alarming upon occlusion stops flow and hails clinician." .
:OPENPCAB-28 rdf:type owl:NamedIndividual .
:OPENPCAB-28 rdf:type sao:SafetyRequirement .
:OPENPCAB-28 rdfs:label "Downstream occlusion alarm" .
:OPENPCAB-28 rdfs:comment "A downstream occlusion alarm shall be triggered if the pump senses a downstream (patient side) occlusion exceeding 10 psi." .
:OPENPCAB-28 sao:status "To Do" .
:OPENPCAB-28 sao:creationdate "2023-05-09T09:12:39.074-0300" .
:OPENPCAB-28 sao:lastupdate "2023-05-09T09:12:40.848-0300" .
:OPENPCAB-28 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-28" .
:OPENPCAB-28 sao:mitigates :OPENPCAB-21 .
:OPENPCAB-28 sao:refines :OPENPCAB-25 .
:OPENPCAB-28 sao:isAllocatedIn :Component10033 .
:Component10033 sao:allocates :OPENPCAB-28 .
:OPENPCAB-28_assumption rdf:type owl:NamedIndividual .
:OPENPCAB-28_assumption rdf:type sao:Assumption .
:OPENPCAB-28_assumption sao:explains :OPENPCAB-28 .
:OPENPCAB-28 sao:isExplainedBy :OPENPCAB-28_assumption .
:OPENPCAB-28_assumption rdfs:label "Alarming upon occlusion stops flow and hails clinician." .
:OPENPCAB-27 rdf:type owl:NamedIndividual .
:OPENPCAB-27 rdf:type sao:SafetyRequirement .
:OPENPCAB-27 rdfs:label "Detect upstream occlusion" .
:OPENPCAB-27 rdfs:comment "The PCA pump shall detect upstream occlusion." .
:OPENPCAB-27 sao:status "To Do" .
:OPENPCAB-27 sao:creationdate "2023-05-09T09:12:37.341-0300" .
:OPENPCAB-27 sao:lastupdate "2023-05-09T09:12:39.018-0300" .
:OPENPCAB-27 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-27" .
:OPENPCAB-27 sao:mitigates :OPENPCAB-21 .
:OPENPCAB-27_justification rdf:type owl:NamedIndividual .
:OPENPCAB-27_justification rdf:type sao:Justification .
:OPENPCAB-27_justification sao:explains :OPENPCAB-27 .
:OPENPCAB-27 sao:isExplainedBy :OPENPCAB-27_justification .
:OPENPCAB-27_justification rdfs:label "An independent sensor checks the upstream flow." .
:OPENPCAB-26 rdf:type owl:NamedIndividual .
:OPENPCAB-26 rdf:type sao:SafetyRequirement .
:OPENPCAB-26 rdfs:label "Detect downstream occlusion" .
:OPENPCAB-26 rdfs:comment "The PCA pump shall detect downstream occlusion." .
:OPENPCAB-26 sao:status "To Do" .
:OPENPCAB-26 sao:creationdate "2023-05-09T09:12:35.746-0300" .
:OPENPCAB-26 sao:lastupdate "2023-05-09T09:12:37.739-0300" .
:OPENPCAB-26 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-26" .
:OPENPCAB-26 sao:mitigates :OPENPCAB-21 .
:OPENPCAB-26_justification rdf:type owl:NamedIndividual .
:OPENPCAB-26_justification rdf:type sao:Justification .
:OPENPCAB-26_justification sao:explains :OPENPCAB-26 .
:OPENPCAB-26 sao:isExplainedBy :OPENPCAB-26_justification .
:OPENPCAB-26_justification rdfs:label "An independent sensor checks the downstream flow." .
:OPENPCAB-25 rdf:type owl:NamedIndividual .
:OPENPCAB-25 rdf:type sao:Requirement .
:OPENPCAB-25 rdfs:label "Anomaly Detection and Response" .
:OPENPCAB-25 rdfs:comment "The system uses a safety architecture that separates normal operation from error and anomaly detection and response." .
:OPENPCAB-25 sao:status "To Do" .
:OPENPCAB-25 sao:creationdate "2023-05-09T09:12:33.754-0300" .
:OPENPCAB-25 sao:lastupdate "2023-05-09T09:14:00.623-0300" .
:OPENPCAB-25 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-25" .
:OPENPCAB-25 sao:isRefinedBy :OPENPCAB-28 .
:OPENPCAB-25 sao:isRefinedBy :OPENPCAB-29 .
:OPENPCAB-25 sao:isRefinedBy :OPENPCAB-67 .
:OPENPCAB-25 sao:isAllocatedIn :Component10033 .
:Component10033 sao:allocates :OPENPCAB-25 .
:OPENPCAB-24 rdf:type owl:NamedIndividual .
:OPENPCAB-24 rdf:type sao:Requirement .
:OPENPCAB-24 rdfs:label "Resume Infusion After Stop" .
:OPENPCAB-24 rdfs:comment "1. Clinician presses Start Button
2. Previous normal operation resumes" .
:OPENPCAB-24 sao:status "To Do" .
:OPENPCAB-24 sao:creationdate "2023-05-09T09:12:31.538-0300" .
:OPENPCAB-24 sao:lastupdate "2023-05-09T09:12:33.362-0300" .
:OPENPCAB-24 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-24" .
:OPENPCAB-24 sao:isAllocatedIn :Component10026 .
:Component10026 sao:allocates :OPENPCAB-24 .
:OPENPCAB-23 rdf:type owl:NamedIndividual .
:OPENPCAB-23 rdf:type sao:Hazard .
:OPENPCAB-23 rdfs:label "Air in line hazard" .
:OPENPCAB-23 rdfs:comment "Air in Infusion Line. Potential causes: Incorrect/incomplete priming processes; Broken, loose, or unsealed delivery path; The pump is unable to release gas or air; or The pump is set up with an incompatible infusion set." .
:OPENPCAB-23 sao:status "To Do" .
:OPENPCAB-23 sao:creationdate "2023-05-09T09:12:29.563-0300" .
:OPENPCAB-23 sao:lastupdate "2023-05-09T09:14:00.649-0300" .
:OPENPCAB-23 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-23" .
:OPENPCAB-23 sao:isContextualizedBy :OPENPCAB-56 .
:OPENPCAB-23 sao:isExplainedBy :OPENPCAB-65 .
:OPENPCAB-23 sao:isMitigatedBy :OPENPCAB-66 .
:OPENPCAB-23 sao:isMitigatedBy :OPENPCAB-67 .
:OPENPCAB-22 rdf:type owl:NamedIndividual .
:OPENPCAB-22 rdf:type sao:Hazard .
:OPENPCAB-22 rdfs:label "Free flow hazard" .
:OPENPCAB-22 rdfs:comment "Uncontrolled Flow of Infusate. Potential causes: Valves in the delivery path are broken, The pump is positioned much higher than the infusion site, causing unintentional drug flow, or The delivery path is damaged, creating a vent on the path that allows unintentional gravity flow." .
:OPENPCAB-22 sao:status "To Do" .
:OPENPCAB-22 sao:creationdate "2023-05-09T09:12:27.975-0300" .
:OPENPCAB-22 sao:lastupdate "2023-05-09T09:13:36.390-0300" .
:OPENPCAB-22 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-22" .
:OPENPCAB-22 sao:isContextualizedBy :OPENPCAB-56 .
:OPENPCAB-22_assumption rdf:type owl:NamedIndividual .
:OPENPCAB-22_assumption rdf:type sao:Assumption .
:OPENPCAB-22_assumption sao:explains :OPENPCAB-22 .
:OPENPCAB-22 sao:isExplainedBy :OPENPCAB-22_assumption .
:OPENPCAB-22_assumption rdfs:label "Rely on mechanical design of pumping mechanism" .
:OPENPCAB-21 rdf:type owl:NamedIndividual .
:OPENPCAB-21 rdf:type sao:Hazard .
:OPENPCAB-21 rdfs:label "Occlusion hazard" .
:OPENPCAB-21 rdfs:comment "When there is a blockage between pump and patient (downstream), or between reservoir and pump (upstream). It may be caused by delivery path obstructed, e.g., kinked tubes, or chemical precipitation inside the delivery path , or bolus occurring after an occlusion." .
:OPENPCAB-21 sao:status "To Do" .
:OPENPCAB-21 sao:creationdate "2023-05-09T09:12:26.232-0300" .
:OPENPCAB-21 sao:lastupdate "2023-05-09T09:13:54.358-0300" .
:OPENPCAB-21 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-21" .
:OPENPCAB-21 sao:isContextualizedBy :OPENPCAB-56 .
:OPENPCAB-21 sao:isExplainedBy :OPENPCAB-33 .
:OPENPCAB-21 sao:isMitigatedBy :OPENPCAB-26 .
:OPENPCAB-21 sao:isMitigatedBy :OPENPCAB-27 .
:OPENPCAB-21 sao:isMitigatedBy :OPENPCAB-28 .
:OPENPCAB-21 sao:isMitigatedBy :OPENPCAB-29 .
:OPENPCAB-21 sao:isMitigatedBy :OPENPCAB-64 .
:OPENPCAB-20 rdf:type owl:NamedIndividual .
:OPENPCAB-20 rdf:type sao:SafetyRequirement .
:OPENPCAB-20 rdfs:label "Minimum KVO ﬂow rate" .
:OPENPCAB-20 rdfs:comment "The pump shall maintain a minimum KVO ﬂow rate of FKV O = 1 ml/hr at all times during infusion, even during alarms, unless the alarm also stops ﬂow, or the stop button is pressed." .
:OPENPCAB-20 sao:status "To Do" .
:OPENPCAB-20 sao:creationdate "2023-05-09T09:12:24.552-0300" .
:OPENPCAB-20 sao:lastupdate "2023-05-09T09:12:26.612-0300" .
:OPENPCAB-20 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-20" .
:OPENPCAB-20 sao:refines :OPENPCAB-18 .
:OPENPCAB-20 sao:isAllocatedIn :Component10032 .
:Component10032 sao:allocates :OPENPCAB-20 .
:OPENPCAB-20_justification rdf:type owl:NamedIndividual .
:OPENPCAB-20_justification rdf:type sao:Justification .
:OPENPCAB-20_justification sao:explains :OPENPCAB-20 .
:OPENPCAB-20 sao:isExplainedBy :OPENPCAB-20_justification .
:OPENPCAB-20_justification rdfs:label "If minor hazard is detected, keeping the vein open (KVO) eases the resume of flow after clinician verification." .
:OPENPCAB-19 rdf:type owl:NamedIndividual .
:OPENPCAB-19 rdf:type sao:SafetyRequirement .
:OPENPCAB-19 rdfs:label "Alarm stops basal rate" .
:OPENPCAB-19 rdfs:comment "Any alarm stops basal rate delivery either halting pump or switching to KVO rate." .
:OPENPCAB-19 sao:status "To Do" .
:OPENPCAB-19 sao:creationdate "2023-05-09T09:12:22.933-0300" .
:OPENPCAB-19 sao:lastupdate "2023-05-09T09:12:24.664-0300" .
:OPENPCAB-19 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-19" .
:OPENPCAB-19 sao:refines :OPENPCAB-18 .
:OPENPCAB-19 sao:isAllocatedIn :Component10032 .
:Component10032 sao:allocates :OPENPCAB-19 .
:OPENPCAB-19_justification rdf:type owl:NamedIndividual .
:OPENPCAB-19_justification rdf:type sao:Justification .
:OPENPCAB-19_justification sao:explains :OPENPCAB-19 .
:OPENPCAB-19 sao:isExplainedBy :OPENPCAB-19_justification .
:OPENPCAB-19_justification rdfs:label "If critical hazard is detected, pump shall stop completely." .
:OPENPCAB-18 rdf:type owl:NamedIndividual .
:OPENPCAB-18 rdf:type sao:Requirement .
:OPENPCAB-18 rdfs:label "PCA Pump infuses at basal rate " .
:OPENPCAB-18 rdfs:comment "PCA Pump infuses at basal rate. This use case describes normal operation of the Patient-Controlled Analgesia (PCA) pump.
1. Clinician turns on PCA pump;
2. Clinician presses button when hearing audible alarm sound;
3. Clinician scans own badge;
4. Clinician is authenticated to operate PCA pump;
5. Clinician scans patient information (wristband);
6. Patient is authenticated to receive medical care;
7. Clinician scans drug information and patient’s prescription from drug container (vial);
8. Prescription is authenticated for the patient;
9. PCA pump compares prescription with its drug library;
10. Clinician puts drug vial into the reservoir and closes and locks the door;
11. Clinician attaches infusion tube and needle to pump;
12. Clinician primes pump;
13. Clinician inserts infusion needle into patient’s vein;
14. Clinician presses Start button to begin basal-rate infusion;
15. Clinician presses Stop button to halt infusion;
16. Clinician removes infusion needle from patient’s vein, and infusion tube from pump;
17. Clinician removes drug vial, returning remaining drug to pharmacy;
18. Clinician turns off PCA pump power." .
:OPENPCAB-18 sao:status "To Do" .
:OPENPCAB-18 sao:creationdate "2023-05-09T09:12:20.180-0300" .
:OPENPCAB-18 sao:lastupdate "2023-05-09T09:14:11.052-0300" .
:OPENPCAB-18 sao:externaluri "https://arcade-dare.atlassian.net/browse/OPENPCAB-18" .
:OPENPCAB-18 sao:isContextualizedBy :OPENPCAB-54 .
:OPENPCAB-18 sao:refines :OPENPCAB-71 .
:OPENPCAB-18 sao:isRefinedBy :OPENPCAB-19 .
:OPENPCAB-18 sao:isRefinedBy :OPENPCAB-20 .
:OPENPCAB-18 sao:isRefinedBy :OPENPCAB-40 .
:OPENPCAB-18 sao:isRefinedBy :OPENPCAB-42 .
:OPENPCAB-18 sao:isRefinedBy :OPENPCAB-72 .
:Source10008 rdf:type owl:NamedIndividual .
:Source10008 rdf:type sao:Source .
:OPENPCAB-52 sao:isDocumentedBy :Source10008 .
:Source10008 rdfs:comment "Web link" .
:Source10008 rdfs:label "Requirements specification" .
:Source10008 sao:externaluri "https://arcade-dare.atlassian.net/wiki/spaces/~5f6b8e8e1d34a50077d1bb5a/pages/1112539137/" .
:Source10008 sao:creationdate "" .
:Component10033 rdf:type owl:NamedIndividual .
:Component10033 rdf:type sao:Component .
:Component10033 rdfs:label "Alarm Thread" .
:Component10033 rdfs:comment "The alarm thread evaluates fault signals to determine whether the infusion rate should be changed, issues alarm and warning signals to be sounded and displayed by the control panel, and creates fault entries to be stored in the fault log." .
:Component10026 rdf:type owl:NamedIndividual .
:Component10026 rdf:type sao:Component .
:Component10026 rdfs:label "Control Panel" .
:Component10026 rdfs:comment "" .
:Component10035 rdf:type owl:NamedIndividual .
:Component10035 rdf:type sao:Component .
:Component10035 rdfs:label "Flow Rate Checker" .
:Component10035 rdfs:comment "The pump fault manager determines if the measured upstream and downstream ﬂow rates are within tolerance of the speciﬁed rate, and aggregates other pump fault indications into a combined pump fault indication." .
:Component10034 rdf:type owl:NamedIndividual .
:Component10034 rdf:type sao:Component .
:Component10034 rdfs:label "Patient Bolus Checker" .
:Component10034 rdfs:comment "The patient bolus checker thread prevents patient-requests bolus delivery sooner than the minimum time between patient-requested bolus." .
:Component10032 rdf:type owl:NamedIndividual .
:Component10032 rdf:type sao:Component .
:Component10032 rdfs:label "Pump" .
:Component10032 rdfs:comment "The pump moves ﬂuid at speciﬁed rate, primes itself, announces if priming fails, indicates when it’s too hot, and halts pumping when commanded." .
:Component10036 rdf:type owl:NamedIndividual .
:Component10036 rdf:type sao:Component .
:Component10036 rdfs:label "Rate Controller Thread" .
:Component10036 rdfs:comment "The rate controller thread determines the pump rate" .
:Component10029 rdf:type owl:NamedIndividual .
:Component10029 rdf:type sao:Component .
:Component10029 rdfs:label "Security" .
:Component10029 rdfs:comment "" .
```
