## Dronology

- Dronology provides an open source framework for controlling and coordinating the flight of individual UAS, formations, and swarms in order to to support applications such as search-and-rescue, surveillance, and scientific data collection. The project establishes a research environment for studying various aspects of software and systems engineering for cyber-physical systems -- e.g., runtime monitoring, safety analysis, and product line development.
- Link: [https://dronology.info/](https://dronology.info/)

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
:DRONE-155 rdf:type owl:NamedIndividual .
:DRONE-155 rdf:type sao:Hazard .
:DRONE-155 rdfs:label "UAV receives waypoint commands but does not obey them" .
:DRONE-155 rdfs:comment "UAV receives waypoint commands but does not obey them" .
:DRONE-155 sao:status "To Do" .
:DRONE-155 sao:creationdate "2023-05-13T17:13:05.881-0300" .
:DRONE-155 sao:lastupdate "2023-05-13T17:13:28.702-0300" .
:DRONE-155 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-155" .
:DRONE-155 sao:isExplainedBy :DRONE-127 .
:DRONE-155 sao:isMitigatedBy :DRONE-152 .
:DRONE-154 rdf:type owl:NamedIndividual .
:DRONE-154 rdf:type sao:Requirement .
:DRONE-154 rdfs:label "Compute the total distance flown by all UAVs" .
:DRONE-154 rdfs:comment "Given a route allocation compute the total distance flown by all drones including start and home locations and distance between assigned routes." .
:DRONE-154 sao:status "To Do" .
:DRONE-154 sao:creationdate "2023-05-13T17:13:05.295-0300" .
:DRONE-154 sao:lastupdate "2023-05-15T14:42:29.601-0300" .
:DRONE-154 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-154" .
:DRONE-154 sao:isRealizedBy :DRONE-40 .
:DRONE-154 sao:isRefinedBy :DRONE-107 .
:DRONE-154 sao:isAllocatedIn :Component10051 .
:Component10051 sao:allocates :DRONE-154 .
:DRONE-154 sao:isAllocatedIn :Component10052 .
:Component10052 sao:allocates :DRONE-154 .
:DRONE-153 rdf:type owl:NamedIndividual .
:DRONE-153 rdf:type sao:SafetyRequirement .
:DRONE-153 rdfs:label "Battery voltage must be displayed on UI" .
:DRONE-153 rdfs:comment "The UI shall display the available battery percentage for each UAV in flight." .
:DRONE-153 sao:status "To Do" .
:DRONE-153 sao:creationdate "2023-05-13T17:13:04.726-0300" .
:DRONE-153 sao:lastupdate "2023-05-13T17:13:28.825-0300" .
:DRONE-153 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-153" .
:DRONE-153 sao:mitigates :DRONE-136 .
:DRONE-153 sao:isRealizedBy :DRONE-65 .
:DRONE-153 sao:isRealizedBy :DRONE-77 .
:DRONE-152 rdf:type owl:NamedIndividual .
:DRONE-152 rdf:type sao:Requirement .
:DRONE-152 rdfs:label "RPIC will takeover control with the hand-held GCS when deemed necessary" .
:DRONE-152 rdfs:comment "When the RPIC determines that Dronology has lost control of the UAV for more than 
acceptable loss of communication
 minutes, then the RPIC shall take control." .
:DRONE-152 sao:status "To Do" .
:DRONE-152 sao:creationdate "2023-05-13T17:13:04.158-0300" .
:DRONE-152 sao:lastupdate "2023-05-13T17:13:28.638-0300" .
:DRONE-152 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-152" .
:DRONE-152 sao:mitigates :DRONE-25 .
:DRONE-152 sao:mitigates :DRONE-26 .
:DRONE-152 sao:mitigates :DRONE-121 .
:DRONE-152 sao:mitigates :DRONE-155 .
:DRONE-151 rdf:type owl:NamedIndividual .
:DRONE-151 rdf:type sao:Requirement .
:DRONE-151 rdfs:label "RPIC will takeover control with the hand-held GCS when deemed necessary" .
:DRONE-151 rdfs:comment "When the RPIC determines that Dronology has lost control of the UAV for more than 
acceptable loss of communication
 minutes, then the RPIC shall take control." .
:DRONE-151 sao:status "To Do" .
:DRONE-151 sao:creationdate "2023-05-13T17:13:03.583-0300" .
:DRONE-151 sao:lastupdate "2023-05-13T17:13:04.055-0300" .
:DRONE-151 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-151" .
:DRONE-150 rdf:type owl:NamedIndividual .
:DRONE-150 rdf:type sao:Requirement .
:DRONE-150 rdfs:label "RPIC will takeover control with the hand-held GCS when deemed necessary" .
:DRONE-150 rdfs:comment "When the RPIC determines that Dronology has lost control of the UAV for more than 
acceptable loss of communication
 minutes, then the RPIC shall take control." .
:DRONE-150 sao:status "To Do" .
:DRONE-150 sao:creationdate "2023-05-13T17:13:03.024-0300" .
:DRONE-150 sao:lastupdate "2023-05-13T17:13:03.478-0300" .
:DRONE-150 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-150" .
:DRONE-149 rdf:type owl:NamedIndividual .
:DRONE-149 rdf:type sao:Requirement .
:DRONE-149 rdfs:label "RPIC will takeover control with the hand-held GCS when deemed necessary" .
:DRONE-149 rdfs:comment "When the RPIC determines that Dronology has lost control of the UAV for more than 
acceptable loss of communication
 minutes, then the RPIC shall take control." .
:DRONE-149 sao:status "To Do" .
:DRONE-149 sao:creationdate "2023-05-13T17:13:02.456-0300" .
:DRONE-149 sao:lastupdate "2023-05-13T17:13:02.922-0300" .
:DRONE-149 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-149" .
:DRONE-148 rdf:type owl:NamedIndividual .
:DRONE-148 rdf:type sao:DesignDefinition .
:DRONE-148 rdfs:label "All UAVs use PixHawk 1.x or 2.x controllers with inbuilt RTL capabilities including programmable RTL triggers and RTL altitudes." .
:DRONE-148 rdfs:comment "RTL capabilities are built into the PixHawk 1.x and 2.x controller used by all UAVs integrated into Dronology." .
:DRONE-148 sao:status "To Do" .
:DRONE-148 sao:creationdate "2023-05-13T17:13:01.853-0300" .
:DRONE-148 sao:lastupdate "2023-05-13T17:13:27.856-0300" .
:DRONE-148 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-148" .
:DRONE-148 sao:isExplainedBy :DRONE-130 .
:DRONE-148 sao:isExplainedBy :DRONE-131 .
:DRONE-148 sao:realizes :DRONE-147 .
:DRONE-147 rdf:type owl:NamedIndividual .
:DRONE-147 rdf:type sao:SafetyRequirement .
:DRONE-147 rdfs:label "All UAVs shall have onboard failsafe mechanisms" .
:DRONE-147 rdfs:comment "All UAVs shall have failsafe mechanisms that enable them to independently make basic land-in-place, stop in place,  and RTL decisions in case of emergency." .
:DRONE-147 sao:status "To Do" .
:DRONE-147 sao:creationdate "2023-05-13T17:13:01.280-0300" .
:DRONE-147 sao:lastupdate "2023-05-13T17:13:27.961-0300" .
:DRONE-147 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-147" .
:DRONE-147 sao:isExplainedBy :DRONE-88 .
:DRONE-147 sao:mitigates :DRONE-121 .
:DRONE-147 sao:isRealizedBy :DRONE-148 .
:DRONE-146 rdf:type owl:NamedIndividual .
:DRONE-146 rdf:type sao:Requirement .
:DRONE-146 rdfs:label "Routes assigned manually" .
:DRONE-146 rdfs:comment "For area mapping applications, routes are assigned manually." .
:DRONE-146 sao:status "To Do" .
:DRONE-146 sao:creationdate "2023-05-13T17:13:00.708-0300" .
:DRONE-146 sao:lastupdate "2023-05-13T17:13:27.497-0300" .
:DRONE-146 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-146" .
:DRONE-146 sao:mitigates :DRONE-135 .
:DRONE-145 rdf:type owl:NamedIndividual .
:DRONE-145 rdf:type sao:Requirement .
:DRONE-145 rdfs:label "User issues RTL command using GCS." .
:DRONE-145 rdfs:comment "After the user cedes control of the UAV from Dronology, the user can issue a RTL command using the hand-held GCS." .
:DRONE-145 sao:status "To Do" .
:DRONE-145 sao:creationdate "2023-05-13T17:12:59.955-0300" .
:DRONE-145 sao:lastupdate "2023-05-13T17:13:27.292-0300" .
:DRONE-145 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-145" .
:DRONE-145 sao:isExplainedBy :DRONE-90 .
:DRONE-145 sao:mitigates :DRONE-133 .
:DRONE-144 rdf:type owl:NamedIndividual .
:DRONE-144 rdf:type sao:Assumption .
:DRONE-144 rdfs:label "All UAVs support user defined RTL altitudes" .
:DRONE-144 rdfs:comment "All UAVs provide functionality that allows them to be preprogrammed with a RTL altitude." .
:DRONE-144 sao:status "To Do" .
:DRONE-144 sao:creationdate "2023-05-13T17:12:59.402-0300" .
:DRONE-144 sao:lastupdate "2023-05-13T17:13:27.129-0300" .
:DRONE-144 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-144" .
:DRONE-144 sao:explains :DRONE-90 .
:DRONE-143 rdf:type owl:NamedIndividual .
:DRONE-143 rdf:type sao:Requirement .
:DRONE-143 rdfs:label "Carefully plan routes to avoid known obstacles" .
:DRONE-143 rdfs:comment "Avoid all fixed obstacles such as trees on the bank, bridges etc when planning routes.  Check all routes on the simulator prior to flight." .
:DRONE-143 sao:status "To Do" .
:DRONE-143 sao:creationdate "2023-05-13T17:12:58.876-0300" .
:DRONE-143 sao:lastupdate "2023-05-13T17:13:26.930-0300" .
:DRONE-143 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-143" .
:DRONE-143 sao:mitigates :DRONE-20 .
:DRONE-142 rdf:type owl:NamedIndividual .
:DRONE-142 rdf:type sao:Context .
:DRONE-142 rdfs:label "Dronology applications include flights over water" .
:DRONE-142 rdfs:comment "Landing in place when flying over water is not acceptable" .
:DRONE-142 sao:status "To Do" .
:DRONE-142 sao:creationdate "2023-05-13T17:12:58.330-0300" .
:DRONE-142 sao:lastupdate "2023-05-15T09:45:21.033-0300" .
:DRONE-142 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-142" .
:DRONE-142 sao:contextualizes :DRONE-136 .
:DRONE-141 rdf:type owl:NamedIndividual .
:DRONE-141 rdf:type sao:Assumption .
:DRONE-141 rdfs:label "Default behavior for depleted voltage is land-in-place" .
:DRONE-141 rdfs:comment "Most UAVs are preprogrammed by their manufacturers to land-in-place when voltage falls below a certain threshold." .
:DRONE-141 sao:status "To Do" .
:DRONE-141 sao:creationdate "2023-05-13T17:12:57.739-0300" .
:DRONE-141 sao:lastupdate "2023-05-13T17:13:26.576-0300" .
:DRONE-141 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-141" .
:DRONE-141 sao:explains :DRONE-136 .
:DRONE-140 rdf:type owl:NamedIndividual .
:DRONE-140 rdf:type sao:Assumption .
:DRONE-140 rdfs:label "Check hand-held controller battery prior to takeoff" .
:DRONE-140 rdfs:comment "RPIC is responsible for assuring that the hand-held controller's voltage is greater than the minimum takeoff threshold prior to takeoff." .
:DRONE-140 sao:status "To Do" .
:DRONE-140 sao:creationdate "2023-05-13T17:12:57.158-0300" .
:DRONE-140 sao:lastupdate "2023-05-13T17:13:26.379-0300" .
:DRONE-140 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-140" .
:DRONE-140 sao:explains :DRONE-138 .
:DRONE-139 rdf:type owl:NamedIndividual .
:DRONE-139 rdf:type sao:Assumption .
:DRONE-139 rdfs:label "Check UAV battery prior to takeoff" .
:DRONE-139 rdfs:comment "RPIC is responsible for checking that the UAV battery's voltage is greater than, or equal to, the minimum takeoff threshold for that UAV type." .
:DRONE-139 sao:status "To Do" .
:DRONE-139 sao:creationdate "2023-05-13T17:12:56.613-0300" .
:DRONE-139 sao:lastupdate "2023-05-13T17:13:26.189-0300" .
:DRONE-139 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-139" .
:DRONE-139 sao:explains :DRONE-138 .
:DRONE-138 rdf:type owl:NamedIndividual .
:DRONE-138 rdf:type sao:Assumption .
:DRONE-138 rdfs:label "Battery voltage checked manually prior to takeoff" .
:DRONE-138 sao:status "To Do" .
:DRONE-138 sao:creationdate "2023-05-13T17:12:56.022-0300" .
:DRONE-138 sao:lastupdate "2023-05-13T17:13:26.430-0300" .
:DRONE-138 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-138" .
:DRONE-138 sao:explains :DRONE-137 .
:DRONE-138 sao:isExplainedBy :DRONE-139 .
:DRONE-138 sao:isExplainedBy :DRONE-140 .
:DRONE-137 rdf:type owl:NamedIndividual .
:DRONE-137 rdf:type sao:SafetyRequirement .
:DRONE-137 rdfs:label "Sufficient battery voltage needed for all issued waypoints" .
:DRONE-137 rdfs:comment "Waypoint commands shall only be issued to a UAV if it has sufficient voltage to reach its destination and return to a safe landing place." .
:DRONE-137 sao:status "To Do" .
:DRONE-137 sao:creationdate "2023-05-13T17:12:55.447-0300" .
:DRONE-137 sao:lastupdate "2023-05-13T17:13:26.060-0300" .
:DRONE-137 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-137" .
:DRONE-137 sao:isExplainedBy :DRONE-138 .
:DRONE-137 sao:mitigates :DRONE-136 .
:DRONE-136 rdf:type owl:NamedIndividual .
:DRONE-136 rdf:type sao:Hazard .
:DRONE-136 rdfs:label "Battery fails during flight" .
:DRONE-136 sao:status "To Do" .
:DRONE-136 sao:creationdate "2023-05-13T17:12:54.925-0300" .
:DRONE-136 sao:lastupdate "2023-05-15T09:45:20.965-0300" .
:DRONE-136 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-136" .
:DRONE-136 sao:isContextualizedBy :DRONE-142 .
:DRONE-136 sao:isExplainedBy :DRONE-141 .
:DRONE-136 sao:isMitigatedBy :DRONE-101 .
:DRONE-136 sao:isMitigatedBy :DRONE-137 .
:DRONE-136 sao:isMitigatedBy :DRONE-153 .
:DRONE-135 rdf:type owl:NamedIndividual .
:DRONE-135 rdf:type sao:Hazard .
:DRONE-135 rdfs:label "Area mapping provides insufficient coverage during search and rescue" .
:DRONE-135 rdfs:comment "Area mapping is used to support aerial search and rescue.  Insufficient coverage can impact the feasibility of a successful search and rescue." .
:DRONE-135 sao:status "To Do" .
:DRONE-135 sao:creationdate "2023-05-13T17:12:54.391-0300" .
:DRONE-135 sao:lastupdate "2023-05-13T17:13:27.548-0300" .
:DRONE-135 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-135" .
:DRONE-135 sao:isMitigatedBy :DRONE-34 .
:DRONE-135 sao:isMitigatedBy :DRONE-146 .
:DRONE-134 rdf:type owl:NamedIndividual .
:DRONE-134 rdf:type sao:Assumption .
:DRONE-134 rdfs:label "The user shall assign a set of UAVs to search a mapped region of the river and request routes to be generated for them." .
:DRONE-134 rdfs:comment "When the user wants to generate a route from a mapping, prompt them to select the drones they'd like to use. Then send that information to generateAreaMapping()." .
:DRONE-134 sao:status "To Do" .
:DRONE-134 sao:creationdate "2023-05-13T17:12:53.859-0300" .
:DRONE-134 sao:lastupdate "2023-05-13T17:13:25.639-0300" .
:DRONE-134 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-134" .
:DRONE-134 sao:explains :DRONE-34 .
:DRONE-133 rdf:type owl:NamedIndividual .
:DRONE-133 rdf:type sao:Hazard .
:DRONE-133 rdfs:label "UAV collides with another UAV when Dronology issues RTL commands to multiple UAVs." .
:DRONE-133 rdfs:comment "When Dronology issues a  RTL command to multiple UAVs their flight paths could overlap causing a potential midair collision." .
:DRONE-133 sao:status "To Do" .
:DRONE-133 sao:creationdate "2023-05-13T17:12:53.326-0300" .
:DRONE-133 sao:lastupdate "2023-05-13T17:13:27.357-0300" .
:DRONE-133 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-133" .
:DRONE-133 sao:isMitigatedBy :DRONE-78 .
:DRONE-133 sao:isMitigatedBy :DRONE-145 .
:DRONE-132 rdf:type owl:NamedIndividual .
:DRONE-132 rdf:type sao:Assumption .
:DRONE-132 rdfs:label "One RPIC per UAV in flight" .
:DRONE-132 rdfs:comment "There will be one human RPIC assigned to each UAV during its flight" .
:DRONE-132 sao:status "To Do" .
:DRONE-132 sao:creationdate "2023-05-13T17:12:52.694-0300" .
:DRONE-132 sao:lastupdate "2023-05-13T17:13:25.405-0300" .
:DRONE-132 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-132" .
:DRONE-132 sao:explains :DRONE-89 .
:DRONE-131 rdf:type owl:NamedIndividual .
:DRONE-131 rdf:type sao:Assumption .
:DRONE-131 rdfs:label "3rd party customized RTL altitudes" .
:DRONE-131 rdfs:comment "The UAVs RTL feature allows the return altitude for each UAV to be customized and each UAV has been assigned an individual RTL altitude." .
:DRONE-131 sao:status "To Do" .
:DRONE-131 sao:creationdate "2023-05-13T17:12:52.092-0300" .
:DRONE-131 sao:lastupdate "2023-05-13T17:13:25.239-0300" .
:DRONE-131 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-131" .
:DRONE-131 sao:explains :DRONE-148 .
:DRONE-130 rdf:type owl:NamedIndividual .
:DRONE-130 rdf:type sao:Assumption .
:DRONE-130 rdfs:label "3rd party RTL at Geofence breach" .
:DRONE-130 rdfs:comment "The UAV has capabilities to activate RTL upon Geofence breach, and these capabilities have been activated in each UAV." .
:DRONE-130 sao:status "To Do" .
:DRONE-130 sao:creationdate "2023-05-13T17:12:51.495-0300" .
:DRONE-130 sao:lastupdate "2023-05-13T17:13:25.064-0300" .
:DRONE-130 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-130" .
:DRONE-130 sao:explains :DRONE-148 .
:DRONE-129 rdf:type owl:NamedIndividual .
:DRONE-129 rdf:type sao:Assumption .
:DRONE-129 rdfs:label "No unauthorized commands are received" .
:DRONE-129 rdfs:comment "UAVs under the control of Dronology only receive commands from the Dronology GCS and the official handheld controllers" .
:DRONE-129 sao:status "To Do" .
:DRONE-129 sao:creationdate "2023-05-13T17:12:50.891-0300" .
:DRONE-129 sao:lastupdate "2023-05-13T17:13:24.870-0300" .
:DRONE-129 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-129" .
:DRONE-129 sao:explains :DRONE-89 .
:DRONE-128 rdf:type owl:NamedIndividual .
:DRONE-128 rdf:type sao:Requirement .
:DRONE-128 rdfs:label "The user shall mark critical regions of the demarcated riverbank as high priority" .
:DRONE-128 rdfs:comment "When the user right clicks on an existing riverbank polyline, it should turn red and be saved as a priority side." .
:DRONE-128 sao:status "To Do" .
:DRONE-128 sao:creationdate "2023-05-13T17:12:50.285-0300" .
:DRONE-128 sao:lastupdate "2023-05-15T14:19:27.972-0300" .
:DRONE-128 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-128" .
:DRONE-128 sao:isRealizedBy :DRONE-115 .
:DRONE-128 sao:isAllocatedIn :Component10049 .
:Component10049 sao:allocates :DRONE-128 .
:DRONE-127 rdf:type owl:NamedIndividual .
:DRONE-127 rdf:type sao:Assumption .
:DRONE-127 rdfs:label "UAV is operated under FAA Line of Sight regulations" .
:DRONE-127 rdfs:comment "The UAV may not fly beyond line of sight (BLOS) of the operator enabling an operator to constantly observe the UAVs behavior and to respond accordingly." .
:DRONE-127 sao:status "To Do" .
:DRONE-127 sao:creationdate "2023-05-13T17:12:49.687-0300" .
:DRONE-127 sao:lastupdate "2023-05-13T17:13:24.509-0300" .
:DRONE-127 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-127" .
:DRONE-127 sao:explains :DRONE-19 .
:DRONE-127 sao:explains :DRONE-20 .
:DRONE-127 sao:explains :DRONE-25 .
:DRONE-127 sao:explains :DRONE-89 .
:DRONE-127 sao:explains :DRONE-155 .
:DRONE-126 rdf:type owl:NamedIndividual .
:DRONE-126 rdf:type sao:Assumption .
:DRONE-126 rdfs:label "UAV is operated under FAA Line of Sight regulations" .
:DRONE-126 rdfs:comment "The UAV may not fly beyond line of sight (BLOS) of the operator enabling an operator to constantly observe the UAVs behavior and to respond accordingly." .
:DRONE-126 sao:status "To Do" .
:DRONE-126 sao:creationdate "2023-05-13T17:12:49.124-0300" .
:DRONE-126 sao:lastupdate "2023-05-13T17:12:49.583-0300" .
:DRONE-126 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-126" .
:DRONE-125 rdf:type owl:NamedIndividual .
:DRONE-125 rdf:type sao:Assumption .
:DRONE-125 rdfs:label "UAV is operated under FAA Line of Sight regulations" .
:DRONE-125 rdfs:comment "The UAV may not fly beyond line of sight (BLOS) of the operator enabling an operator to constantly observe the UAVs behavior and to respond accordingly." .
:DRONE-125 sao:status "To Do" .
:DRONE-125 sao:creationdate "2023-05-13T17:12:48.569-0300" .
:DRONE-125 sao:lastupdate "2023-05-13T17:12:49.020-0300" .
:DRONE-125 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-125" .
:DRONE-124 rdf:type owl:NamedIndividual .
:DRONE-124 rdf:type sao:Assumption .
:DRONE-124 rdfs:label "UAV is operated under FAA Line of Sight regulations" .
:DRONE-124 rdfs:comment "The UAV may not fly beyond line of sight (BLOS) of the operator enabling an operator to constantly observe the UAVs behavior and to respond accordingly." .
:DRONE-124 sao:status "To Do" .
:DRONE-124 sao:creationdate "2023-05-13T17:12:47.990-0300" .
:DRONE-124 sao:lastupdate "2023-05-13T17:12:48.458-0300" .
:DRONE-124 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-124" .
:DRONE-123 rdf:type owl:NamedIndividual .
:DRONE-123 rdf:type sao:Assumption .
:DRONE-123 rdfs:label "UAV is operated under FAA Line of Sight regulations" .
:DRONE-123 rdfs:comment "The UAV may not fly beyond line of sight (BLOS) of the operator enabling an operator to constantly observe the UAVs behavior and to respond accordingly." .
:DRONE-123 sao:status "To Do" .
:DRONE-123 sao:creationdate "2023-05-13T17:12:47.405-0300" .
:DRONE-123 sao:lastupdate "2023-05-13T17:12:47.861-0300" .
:DRONE-123 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-123" .
:DRONE-122 rdf:type owl:NamedIndividual .
:DRONE-122 rdf:type sao:Context .
:DRONE-122 rdfs:label "All communication between GCS and UAVs uses telemetry" .
:DRONE-122 rdfs:comment "The ground control station sends all commands to the UAV via telemetry and receives all status reports via telemetry." .
:DRONE-122 sao:status "To Do" .
:DRONE-122 sao:creationdate "2023-05-13T17:12:46.845-0300" .
:DRONE-122 sao:lastupdate "2023-05-15T09:46:10.336-0300" .
:DRONE-122 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-122" .
:DRONE-122 sao:contextualizes :DRONE-121 .
:DRONE-121 rdf:type owl:NamedIndividual .
:DRONE-121 rdf:type sao:Hazard .
:DRONE-121 rdfs:label "UAV is no longer controllable from Dronology due to communication loss." .
:DRONE-121 rdfs:comment "Commands sent to the UAV from the GCS are not received" .
:DRONE-121 sao:status "To Do" .
:DRONE-121 sao:creationdate "2023-05-13T17:12:46.286-0300" .
:DRONE-121 sao:lastupdate "2023-05-15T09:46:10.280-0300" .
:DRONE-121 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-121" .
:DRONE-121 sao:isContextualizedBy :DRONE-122 .
:DRONE-121 sao:isMitigatedBy :DRONE-89 .
:DRONE-121 sao:isMitigatedBy :DRONE-147 .
:DRONE-121 sao:isMitigatedBy :DRONE-152 .
:DRONE-120 rdf:type owl:NamedIndividual .
:DRONE-120 rdf:type sao:Requirement .
:DRONE-120 rdfs:label "High priority areas shall be moved and reshaped" .
:DRONE-120 rdfs:comment "Make it so that the user can right click a polygon priority area to change it's attributes. Also, the user should be able to drag the existing vertices to change the shape." .
:DRONE-120 sao:status "To Do" .
:DRONE-120 sao:creationdate "2023-05-13T17:12:45.675-0300" .
:DRONE-120 sao:lastupdate "2023-05-15T14:20:05.761-0300" .
:DRONE-120 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-120" .
:DRONE-120 sao:isRealizedBy :DRONE-115 .
:DRONE-120 sao:isAllocatedIn :Component10053 .
:Component10053 sao:allocates :DRONE-120 .
:DRONE-120 sao:isAllocatedIn :Component10054 .
:Component10054 sao:allocates :DRONE-120 .
:DRONE-120 sao:isAllocatedIn :Component10049 .
:Component10049 sao:allocates :DRONE-120 .
:DRONE-119 rdf:type owl:NamedIndividual .
:DRONE-119 rdf:type sao:Requirement .
:DRONE-119 rdfs:label "When the user mouseovers a high priority area, a description and other data about the area shall be displayed." .
:DRONE-119 rdfs:comment "When the user mouses over a priority area, a popup should appear that displays the type, importance, and description. It should also allow the user to edit." .
:DRONE-119 sao:status "To Do" .
:DRONE-119 sao:creationdate "2023-05-13T17:12:45.047-0300" .
:DRONE-119 sao:lastupdate "2023-05-15T14:23:03.048-0300" .
:DRONE-119 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-119" .
:DRONE-119 sao:isRealizedBy :DRONE-115 .
:DRONE-119 sao:isAllocatedIn :Component10053 .
:Component10053 sao:allocates :DRONE-119 .
:DRONE-119 sao:isAllocatedIn :Component10049 .
:Component10049 sao:allocates :DRONE-119 .
:DRONE-118 rdf:type owl:NamedIndividual .
:DRONE-118 rdf:type sao:Context .
:DRONE-118 rdfs:label "Operators place UAVs in random positions prior to takeoff which could cause them to cross routes as they fly to their first waypoint." .
:DRONE-118 sao:status "To Do" .
:DRONE-118 sao:creationdate "2023-05-13T17:12:44.541-0300" .
:DRONE-118 sao:lastupdate "2023-05-15T09:46:38.789-0300" .
:DRONE-118 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-118" .
:DRONE-118 sao:contextualizes :DRONE-116 .
:DRONE-117 rdf:type owl:NamedIndividual .
:DRONE-117 rdf:type sao:SafetyRequirement .
:DRONE-117 rdfs:label "Avoid collisions when flying to first waypoint" .
:DRONE-117 rdfs:comment "When in Mission Planning mode, the takeoff and positioning of all UAVs at the start of their first assigned routes shall be choreographed to avoid collisions.\t\t\t\t\t" .
:DRONE-117 sao:status "To Do" .
:DRONE-117 sao:creationdate "2023-05-13T17:12:43.971-0300" .
:DRONE-117 sao:lastupdate "2023-05-13T17:13:22.867-0300" .
:DRONE-117 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-117" .
:DRONE-117 sao:mitigates :DRONE-116 .
:DRONE-117 sao:isRealizedBy :DRONE-80 .
:DRONE-117 sao:isRealizedBy :DRONE-81 .
:DRONE-117 sao:isRealizedBy :DRONE-83 .
:DRONE-117 sao:isRealizedBy :DRONE-84 .
:DRONE-117 sao:isRealizedBy :DRONE-86 .
:DRONE-117 sao:isRealizedBy :DRONE-87 .
:DRONE-116 rdf:type owl:NamedIndividual .
:DRONE-116 rdf:type sao:Hazard .
:DRONE-116 rdfs:label "Collision occurs between UAVs at takeoff" .
:DRONE-116 rdfs:comment "UAVs are placed at random positions prior to takeoff, and may collide when flying to the first waypoint of their assigned routes" .
:DRONE-116 sao:status "To Do" .
:DRONE-116 sao:creationdate "2023-05-13T17:12:43.414-0300" .
:DRONE-116 sao:lastupdate "2023-05-15T09:46:38.739-0300" .
:DRONE-116 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-116" .
:DRONE-116 sao:isContextualizedBy :DRONE-118 .
:DRONE-116 sao:isMitigatedBy :DRONE-117 .
:DRONE-115 rdf:type owl:NamedIndividual .
:DRONE-115 rdf:type sao:DesignDefinition .
:DRONE-115 rdfs:label "The user shall mark high priority search areas on the map." .
:DRONE-115 rdfs:comment "The user shall specify high priority search areas on the river as polygons weighted according to priority level." .
:DRONE-115 sao:status "To Do" .
:DRONE-115 sao:creationdate "2023-05-13T17:12:42.884-0300" .
:DRONE-115 sao:lastupdate "2023-05-15T14:22:57.061-0300" .
:DRONE-115 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-115" .
:DRONE-115 sao:realizes :DRONE-34 .
:DRONE-115 sao:realizes :DRONE-119 .
:DRONE-115 sao:realizes :DRONE-120 .
:DRONE-115 sao:realizes :DRONE-128 .
:DRONE-114 rdf:type owl:NamedIndividual .
:DRONE-114 rdf:type sao:Requirement .
:DRONE-114 rdfs:label "Icons used to map riverbanks shall be different from those used to map flight routes." .
:DRONE-114 rdfs:comment "Instead of using the same waypoint icons from flight routes, create small dots that represent coordinates for each side of the mapping." .
:DRONE-114 sao:status "To Do" .
:DRONE-114 sao:creationdate "2023-05-13T17:12:42.288-0300" .
:DRONE-114 sao:lastupdate "2023-05-15T14:30:06.068-0300" .
:DRONE-114 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-114" .
:DRONE-114 sao:refines :DRONE-33 .
:DRONE-114 sao:isAllocatedIn :Component10049 .
:Component10049 sao:allocates :DRONE-114 .
:DRONE-113 rdf:type owl:NamedIndividual .
:DRONE-113 rdf:type sao:DesignDefinition .
:DRONE-113 rdfs:label "Provide a flight routes tab that is intuitive for the user." .
:DRONE-113 rdfs:comment "Provide a flight routes tab that is intuitive for the user." .
:DRONE-113 sao:status "To Do" .
:DRONE-113 sao:creationdate "2023-05-13T17:12:41.760-0300" .
:DRONE-113 sao:lastupdate "2023-05-13T17:13:22.279-0300" .
:DRONE-113 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-113" .
:DRONE-113 sao:realizes :DRONE-34 .
:DRONE-112 rdf:type owl:NamedIndividual .
:DRONE-112 rdf:type sao:Requirement .
:DRONE-112 rdfs:label "Compute prioritized coverage" .
:DRONE-112 rdfs:comment "This metric calculates the priority coverage score for a given route allocation. A normal route is given a weight of zero, while a PriorityAreaRoute gets a weight based on the assigned weight of the PriorityPolygon. The score for the route allocation is the sum of the score of the assignments for each drone. The score for each drone is the sum of the following calculation: (weighting of the route) * (1 / route position)." .
:DRONE-112 sao:status "To Do" .
:DRONE-112 sao:creationdate "2023-05-13T17:12:41.117-0300" .
:DRONE-112 sao:lastupdate "2023-05-15T14:41:09.802-0300" .
:DRONE-112 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-112" .
:DRONE-112 sao:isRealizedBy :DRONE-40 .
:DRONE-112 sao:isAllocatedIn :Component10051 .
:Component10051 sao:allocates :DRONE-112 .
:DRONE-112 sao:isAllocatedIn :Component10052 .
:Component10052 sao:allocates :DRONE-112 .
:DRONE-111 rdf:type owl:NamedIndividual .
:DRONE-111 rdf:type sao:Requirement .
:DRONE-111 rdfs:label "Compute overall fitness function for the mission" .
:DRONE-111 rdfs:comment "Given an allocation of routes to N drones – we need to compute a mission cost.  (This could be either positive or negative).  All metrics used to compute the mission cost must be normalized.
In phase one of the experiment, we plan to compute a task allocation score based on fixed weightings for each of the factors.  However, we need to be able to try different weights.
This calculation is currently:
Mission Cost = 0.25 x ((Coverage) + (Downstream Ratio) + (Equality of Tasks) - (collisions) / 5)  
This weights all of them equally, and a perfect route assignment would receive a score of 1." .
:DRONE-111 sao:status "To Do" .
:DRONE-111 sao:creationdate "2023-05-13T17:12:40.555-0300" .
:DRONE-111 sao:lastupdate "2023-05-15T14:32:24.357-0300" .
:DRONE-111 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-111" .
:DRONE-111 sao:isRealizedBy :DRONE-40 .
:DRONE-111 sao:isAllocatedIn :Component10051 .
:Component10051 sao:allocates :DRONE-111 .
:DRONE-110 rdf:type owl:NamedIndividual .
:DRONE-110 rdf:type sao:Requirement .
:DRONE-110 rdfs:label "Check that all UAVs have sufficient battery voltage to complete their allocated routes." .
:DRONE-110 rdfs:comment "Given a set of flight routes assigned to each drone, determine whether each drone has sufficient power to complete its allocated flight routes." .
:DRONE-110 sao:status "To Do" .
:DRONE-110 sao:creationdate "2023-05-13T17:12:39.975-0300" .
:DRONE-110 sao:lastupdate "2023-05-15T14:48:23.452-0300" .
:DRONE-110 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-110" .
:DRONE-110 sao:isExplainedBy :DRONE-42 .
:DRONE-110 sao:isRealizedBy :DRONE-41 .
:DRONE-110 sao:isAllocatedIn :Component10050 .
:Component10050 sao:allocates :DRONE-110 .
:DRONE-109 rdf:type owl:NamedIndividual .
:DRONE-109 rdf:type sao:Requirement .
:DRONE-109 rdfs:label "Estimate the equality of tasks assigned to UAVs." .
:DRONE-109 rdfs:comment "Compute an equality metric based on the delta between the longest total distance and the shortest total distance, divided by the longest total distance." .
:DRONE-109 sao:status "To Do" .
:DRONE-109 sao:creationdate "2023-05-13T17:12:39.388-0300" .
:DRONE-109 sao:lastupdate "2023-05-15T14:43:35.386-0300" .
:DRONE-109 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-109" .
:DRONE-109 sao:isRealizedBy :DRONE-40 .
:DRONE-109 sao:isAllocatedIn :Component10050 .
:Component10050 sao:allocates :DRONE-109 .
:DRONE-108 rdf:type owl:NamedIndividual .
:DRONE-108 rdf:type sao:Requirement .
:DRONE-108 rdfs:label "Estimate prevalence of downstream versus upstream search direction" .
:DRONE-108 rdfs:comment "Compute the ratio of downstream routes over the total number of routes." .
:DRONE-108 sao:status "To Do" .
:DRONE-108 sao:creationdate "2023-05-13T17:12:38.837-0300" .
:DRONE-108 sao:lastupdate "2023-05-15T14:43:09.202-0300" .
:DRONE-108 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-108" .
:DRONE-108 sao:isExplainedBy :DRONE-43 .
:DRONE-108 sao:isRealizedBy :DRONE-40 .
:DRONE-108 sao:isAllocatedIn :Component10050 .
:Component10050 sao:allocates :DRONE-108 .
:DRONE-107 rdf:type owl:NamedIndividual .
:DRONE-107 rdf:type sao:Requirement .
:DRONE-107 rdfs:label "Compute distance traveled per UAV" .
:DRONE-107 rdfs:comment "Compute the sum of the distances traveled per Drone from their current starting location (not necessarily home) and including all of their routes + distances between routes + final distance needed to return home." .
:DRONE-107 sao:status "To Do" .
:DRONE-107 sao:creationdate "2023-05-13T17:12:38.303-0300" .
:DRONE-107 sao:lastupdate "2023-05-15T14:42:32.701-0300" .
:DRONE-107 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-107" .
:DRONE-107 sao:refines :DRONE-154 .
:DRONE-107 sao:isAllocatedIn :Component10050 .
:Component10050 sao:allocates :DRONE-107 .
:DRONE-106 rdf:type owl:NamedIndividual .
:DRONE-106 rdf:type sao:Requirement .
:DRONE-106 rdfs:label "Compute area coverage of a set of routes" .
:DRONE-106 rdfs:comment "Given a vectorized form of the map divided into rectangular cells, compute route coverage of multiple UAVs assigned multiple routes by computing the number of cells visited by at least one UAV." .
:DRONE-106 sao:status "To Do" .
:DRONE-106 sao:creationdate "2023-05-13T17:12:37.736-0300" .
:DRONE-106 sao:lastupdate "2023-05-15T14:41:53.024-0300" .
:DRONE-106 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-106" .
:DRONE-106 sao:isRealizedBy :DRONE-40 .
:DRONE-106 sao:isAllocatedIn :Component10050 .
:Component10050 sao:allocates :DRONE-106 .
:DRONE-105 rdf:type owl:NamedIndividual .
:DRONE-105 rdf:type sao:Assumption .
:DRONE-105 rdfs:label "Next waypoint sent after previous waypoint reached" .
:DRONE-105 rdfs:comment "When a flight plan is executed, the 
VehicleCore
 shall send the next waypoint to the UAV after the previous waypoint has been reached." .
:DRONE-105 sao:status "To Do" .
:DRONE-105 sao:creationdate "2023-05-13T17:12:37.170-0300" .
:DRONE-105 sao:lastupdate "2023-05-13T17:13:20.783-0300" .
:DRONE-105 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-105" .
:DRONE-105 sao:explains :DRONE-89 .
:DRONE-104 rdf:type owl:NamedIndividual .
:DRONE-104 rdf:type sao:DesignDefinition .
:DRONE-104 rdfs:label "The UI provides features for mapping the right and left hand side of the river banks." .
:DRONE-104 rdfs:comment "The user shall map the sides of each river bank as a set of connected  points." .
:DRONE-104 sao:status "To Do" .
:DRONE-104 sao:creationdate "2023-05-13T17:12:36.626-0300" .
:DRONE-104 sao:lastupdate "2023-05-13T17:13:20.609-0300" .
:DRONE-104 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-104" .
:DRONE-104 sao:realizes :DRONE-34 .
:DRONE-103 rdf:type owl:NamedIndividual .
:DRONE-103 rdf:type sao:DesignDefinition .
:DRONE-103 rdfs:label "The area mapping system will provide search features for locating and retrieving existing mappings" .
:DRONE-103 rdfs:comment "The area mapping system will provide a search bar located at the top of the screen  for locating and retrieving existing mappings." .
:DRONE-103 sao:status "To Do" .
:DRONE-103 sao:creationdate "2023-05-13T17:12:36.025-0300" .
:DRONE-103 sao:lastupdate "2023-05-15T10:58:55.143-0300" .
:DRONE-103 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-103" .
:DRONE-103 sao:realizes :DRONE-34 .
:DRONE-103 sao:isImplementedBy :Component10049 .
:Component10049 sao:implements :DRONE-103 .
:DRONE-102 rdf:type owl:NamedIndividual .
:DRONE-102 rdf:type sao:DesignDefinition .
:DRONE-102 rdfs:label "Emergency Battery Notification when threshold is reached" .
:DRONE-102 rdfs:comment "When the UAV's battery level drops below a predefined threshold, then the UAV health indicator is activated." .
:DRONE-102 sao:status "To Do" .
:DRONE-102 sao:creationdate "2023-05-13T17:12:35.448-0300" .
:DRONE-102 sao:lastupdate "2023-05-15T10:58:54.952-0300" .
:DRONE-102 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-102" .
:DRONE-102 sao:realizes :DRONE-101 .
:DRONE-102 sao:isImplementedBy :Component10042 .
:Component10042 sao:implements :DRONE-102 .
:DRONE-101 rdf:type owl:NamedIndividual .
:DRONE-101 rdf:type sao:SafetyRequirement .
:DRONE-101 rdfs:label "Emergency Notification" .
:DRONE-101 rdfs:comment "The 
RealTimeFlightUI
 shall notify users when an emergency occurs." .
:DRONE-101 sao:status "To Do" .
:DRONE-101 sao:creationdate "2023-05-13T17:12:34.883-0300" .
:DRONE-101 sao:lastupdate "2023-05-13T17:13:20.316-0300" .
:DRONE-101 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-101" .
:DRONE-101 sao:mitigates :DRONE-136 .
:DRONE-101 sao:isRealizedBy :DRONE-102 .
:DRONE-100 rdf:type owl:NamedIndividual .
:DRONE-100 rdf:type sao:DesignDefinition .
:DRONE-100 rdfs:label "Periodically update UAV location" .
:DRONE-100 rdfs:comment "The UI shall periodically request current locations of all registered UAVs from the 
UIMiddleware
 and update their locations on the map." .
:DRONE-100 sao:status "To Do" .
:DRONE-100 sao:creationdate "2023-05-13T17:12:34.275-0300" .
:DRONE-100 sao:lastupdate "2023-05-15T10:58:54.769-0300" .
:DRONE-100 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-100" .
:DRONE-100 sao:realizes :DRONE-28 .
:DRONE-100 sao:isImplementedBy :Component10043 .
:Component10043 sao:implements :DRONE-100 .
:DRONE-100 sao:isImplementedBy :Component10044 .
:Component10044 sao:implements :DRONE-100 .
:DRONE-99 rdf:type owl:NamedIndividual .
:DRONE-99 rdf:type sao:DesignDefinition .
:DRONE-99 rdfs:label "Display UAV information and operations" .
:DRONE-99 rdfs:comment "For each activated UAV, the UI shall display information about that UAV (i.e. longitude, latitude, altitude, groud speed, battery level, etc.)" .
:DRONE-99 sao:status "To Do" .
:DRONE-99 sao:creationdate "2023-05-13T17:12:33.688-0300" .
:DRONE-99 sao:lastupdate "2023-05-15T10:58:54.568-0300" .
:DRONE-99 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-99" .
:DRONE-99 sao:realizes :DRONE-28 .
:DRONE-99 sao:isImplementedBy :Component10043 .
:Component10043 sao:implements :DRONE-99 .
:DRONE-98 rdf:type owl:NamedIndividual .
:DRONE-98 rdf:type sao:DesignDefinition .
:DRONE-98 rdfs:label "Differentiate UAV types" .
:DRONE-98 rdfs:comment "Different types of UAVs shall have different icons." .
:DRONE-98 sao:status "To Do" .
:DRONE-98 sao:creationdate "2023-05-13T17:12:33.087-0300" .
:DRONE-98 sao:lastupdate "2023-05-15T10:58:54.349-0300" .
:DRONE-98 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-98" .
:DRONE-98 sao:realizes :DRONE-28 .
:DRONE-98 sao:isImplementedBy :Component10043 .
:Component10043 sao:implements :DRONE-98 .
:DRONE-97 rdf:type owl:NamedIndividual .
:DRONE-97 rdf:type sao:DesignDefinition .
:DRONE-97 rdfs:label "Display UAVs on map" .
:DRONE-97 rdfs:comment "When the map is loaded and the all active UAVs list is obtained the 
UIRealTimeFlightView
 shall display an icon on the map for each registered UAV based on its current location." .
:DRONE-97 sao:status "To Do" .
:DRONE-97 sao:creationdate "2023-05-13T17:12:32.499-0300" .
:DRONE-97 sao:lastupdate "2023-05-15T10:58:54.142-0300" .
:DRONE-97 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-97" .
:DRONE-97 sao:realizes :DRONE-28 .
:DRONE-97 sao:isImplementedBy :Component10043 .
:Component10043 sao:implements :DRONE-97 .
:DRONE-96 rdf:type owl:NamedIndividual .
:DRONE-96 rdf:type sao:Assumption .
:DRONE-96 rdfs:label "Mission plan synchronization points" .
:DRONE-96 rdfs:comment "The flight plans of two or more UAVs shall be synchronized by inserting shared synchronization points between the ordered list of flight routes assigned to each participating UAV." .
:DRONE-96 sao:status "To Do" .
:DRONE-96 sao:creationdate "2023-05-13T17:12:31.954-0300" .
:DRONE-96 sao:lastupdate "2023-05-15T14:31:07.444-0300" .
:DRONE-96 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-96" .
:DRONE-96 sao:explains :DRONE-81 .
:DRONE-95 rdf:type owl:NamedIndividual .
:DRONE-95 rdf:type sao:DesignDefinition .
:DRONE-95 rdfs:label "Visiting waypoints during flight plan" .
:DRONE-95 rdfs:comment "When the UAV reaches a target waypoint, if additional waypoints are specified in the flight plan, then the 
VehicleCore
  shall send the next waypoint to the UAV's 
GCS
." .
:DRONE-95 sao:status "To Do" .
:DRONE-95 sao:creationdate "2023-05-13T17:12:31.390-0300" .
:DRONE-95 sao:lastupdate "2023-05-15T10:58:53.767-0300" .
:DRONE-95 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-95" .
:DRONE-95 sao:realizes :DRONE-89 .
:DRONE-95 sao:isImplementedBy :Component10039 .
:Component10039 sao:implements :DRONE-95 .
:DRONE-94 rdf:type owl:NamedIndividual .
:DRONE-94 rdf:type sao:DesignDefinition .
:DRONE-94 rdfs:label "Determine if waypoint is reached" .
:DRONE-94 rdfs:comment "If the computed distance from the UAV to the target waypoint is less than 
THRESHOLD_WAYPOINT_DISTANCE
 than the waypoint shall be considered reached." .
:DRONE-94 sao:status "To Do" .
:DRONE-94 sao:creationdate "2023-05-13T17:12:30.705-0300" .
:DRONE-94 sao:lastupdate "2023-05-15T10:58:53.571-0300" .
:DRONE-94 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-94" .
:DRONE-94 sao:realizes :DRONE-89 .
:DRONE-94 sao:isImplementedBy :Component10039 .
:Component10039 sao:implements :DRONE-94 .
:DRONE-93 rdf:type owl:NamedIndividual .
:DRONE-93 rdf:type sao:DesignDefinition .
:DRONE-93 rdfs:label "Compute distance to next waypoint" .
:DRONE-93 rdfs:comment "When the 
VehicleCore
 receives the UAV's current coordinates and if the UAV has an assigned target waypoint, then the 
VehicleCore
 shall compute the current distance to the target waypoint." .
:DRONE-93 sao:status "To Do" .
:DRONE-93 sao:creationdate "2023-05-13T17:12:30.112-0300" .
:DRONE-93 sao:lastupdate "2023-05-15T10:58:53.177-0300" .
:DRONE-93 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-93" .
:DRONE-93 sao:realizes :DRONE-89 .
:DRONE-93 sao:isImplementedBy :Component10039 .
:Component10039 sao:implements :DRONE-93 .
:DRONE-92 rdf:type owl:NamedIndividual .
:DRONE-92 rdf:type sao:DesignDefinition .
:DRONE-92 rdfs:label "Send first waypoint at start of flight plan" .
:DRONE-92 rdfs:comment "At the start of a flight plan the system shall send the first target waypoint to the UAV's 
GCS
." .
:DRONE-92 sao:status "To Do" .
:DRONE-92 sao:creationdate "2023-05-13T17:12:29.477-0300" .
:DRONE-92 sao:lastupdate "2023-05-15T10:58:52.978-0300" .
:DRONE-92 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-92" .
:DRONE-92 sao:realizes :DRONE-89 .
:DRONE-92 sao:isImplementedBy :Component10048 .
:Component10048 sao:implements :DRONE-92 .
:DRONE-92 sao:isImplementedBy :Component10039 .
:Component10039 sao:implements :DRONE-92 .
:DRONE-91 rdf:type owl:NamedIndividual .
:DRONE-91 rdf:type sao:DesignDefinition .
:DRONE-91 rdfs:label "In normal operating environment, without no-fly restrictions, RTL is issued as single waypoint" .
:DRONE-91 rdfs:comment "When the UAV is commanded to return to home, the current flight plan shall be removed and a new flight plan shall be created containing only a single waypoint representing its original launch coordinates." .
:DRONE-91 sao:status "To Do" .
:DRONE-91 sao:creationdate "2023-05-13T17:12:28.912-0300" .
:DRONE-91 sao:lastupdate "2023-05-15T10:58:52.793-0300" .
:DRONE-91 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-91" .
:DRONE-91 sao:realizes :DRONE-78 .
:DRONE-91 sao:isImplementedBy :Component10047 .
:Component10047 sao:implements :DRONE-91 .
:DRONE-90 rdf:type owl:NamedIndividual .
:DRONE-90 rdf:type sao:Assumption .
:DRONE-90 rdfs:label "UAV default RTL uses predefined altitude" .
:DRONE-90 rdfs:comment "A UAV that executes its inbuilt RTL function shall fly at a uniquely defined altitude preestablished in its firmware." .
:DRONE-90 sao:status "To Do" .
:DRONE-90 sao:creationdate "2023-05-13T17:12:28.344-0300" .
:DRONE-90 sao:lastupdate "2023-05-13T17:13:27.179-0300" .
:DRONE-90 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-90" .
:DRONE-90 sao:explains :DRONE-145 .
:DRONE-90 sao:isExplainedBy :DRONE-144 .
:DRONE-89 rdf:type owl:NamedIndividual .
:DRONE-89 rdf:type sao:SafetyRequirement .
:DRONE-89 rdfs:label "Hover in place if no pending commands and connectivity to GCS is lost" .
:DRONE-89 rdfs:comment "If a UAV has lost connectivity with the GCS and has no currently assigned waypoint, then it shall hover in place until it receives a further command." .
:DRONE-89 sao:status "To Do" .
:DRONE-89 sao:creationdate "2023-05-13T17:12:27.760-0300" .
:DRONE-89 sao:lastupdate "2023-05-13T17:13:25.518-0300" .
:DRONE-89 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-89" .
:DRONE-89 sao:isExplainedBy :DRONE-105 .
:DRONE-89 sao:isExplainedBy :DRONE-127 .
:DRONE-89 sao:isExplainedBy :DRONE-129 .
:DRONE-89 sao:isExplainedBy :DRONE-132 .
:DRONE-89 sao:mitigates :DRONE-121 .
:DRONE-89 sao:isRealizedBy :DRONE-92 .
:DRONE-89 sao:isRealizedBy :DRONE-93 .
:DRONE-89 sao:isRealizedBy :DRONE-94 .
:DRONE-89 sao:isRealizedBy :DRONE-95 .
:DRONE-88 rdf:type owl:NamedIndividual .
:DRONE-88 rdf:type sao:Assumption .
:DRONE-88 rdfs:label "RTL if UAV reaches onboard GeoFence boundary" .
:DRONE-88 rdfs:comment "If a UAV reaches the boundary of the onboard GeoFence it shall RTL." .
:DRONE-88 sao:status "To Do" .
:DRONE-88 sao:creationdate "2023-05-13T17:12:27.153-0300" .
:DRONE-88 sao:lastupdate "2023-05-13T17:13:17.648-0300" .
:DRONE-88 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-88" .
:DRONE-88 sao:explains :DRONE-147 .
:DRONE-87 rdf:type owl:NamedIndividual .
:DRONE-87 rdf:type sao:DesignDefinition .
:DRONE-87 rdfs:label "Transition to regular flight mode after coordinated takeoff" .
:DRONE-87 rdfs:comment "When in COORDINATED_TAKEOFF Mode and all UAVs reach the first waypoint of their assigned flight routes, the mode shall change to COORDINATED_FLIGHT and each UAV shall commence flying its prescribed route." .
:DRONE-87 sao:status "To Do" .
:DRONE-87 sao:creationdate "2023-05-13T17:12:26.613-0300" .
:DRONE-87 sao:lastupdate "2023-05-15T10:58:52.608-0300" .
:DRONE-87 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-87" .
:DRONE-87 sao:realizes :DRONE-117 .
:DRONE-87 sao:isImplementedBy :Component10045 .
:Component10045 sao:implements :DRONE-87 .
:DRONE-86 rdf:type owl:NamedIndividual .
:DRONE-86 rdf:type sao:DesignDefinition .
:DRONE-86 rdfs:label "When reaching the first waypoint, the UAV descends or ascends to the specified altitude duing coordinated takeoff" .
:DRONE-86 rdfs:comment "When in COORDINATED_TAKEOFF mode and all UAVs have reached the targeted longitude and latitude of their first waypoint, they shall all descend to the altitude specified in the flight route for the first waypoint." .
:DRONE-86 sao:status "To Do" .
:DRONE-86 sao:creationdate "2023-05-13T17:12:26.029-0300" .
:DRONE-86 sao:lastupdate "2023-05-13T17:13:17.292-0300" .
:DRONE-86 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-86" .
:DRONE-86 sao:realizes :DRONE-49 .
:DRONE-86 sao:realizes :DRONE-117 .
:DRONE-85 rdf:type owl:NamedIndividual .
:DRONE-85 rdf:type sao:DesignDefinition .
:DRONE-85 rdfs:label "When reaching the first waypoint, the UAV descends or ascends to the specified altitude duing coordinated takeoff" .
:DRONE-85 rdfs:comment "When in COORDINATED_TAKEOFF mode and all UAVs have reached the targeted longitude and latitude of their first waypoint, they shall all descend to the altitude specified in the flight route for the first waypoint." .
:DRONE-85 sao:status "To Do" .
:DRONE-85 sao:creationdate "2023-05-13T17:12:25.477-0300" .
:DRONE-85 sao:lastupdate "2023-05-15T10:58:52.420-0300" .
:DRONE-85 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-85" .
:DRONE-85 sao:isImplementedBy :Component10046 .
:Component10046 sao:implements :DRONE-85 .
:DRONE-84 rdf:type owl:NamedIndividual .
:DRONE-84 rdf:type sao:DesignDefinition .
:DRONE-84 rdfs:label "UAV hovers in place at start of first route during coordinated takeoff awaiting instructions to proceed" .
:DRONE-84 rdfs:comment "When in COORDINATED_TAKEOFF mode and a UAV has reached the longitude and latitude coordinates of its first waypoint then it shall hover in place until it receives a command to descend to the target altitude of its first waypoint." .
:DRONE-84 sao:status "To Do" .
:DRONE-84 sao:creationdate "2023-05-13T17:12:24.870-0300" .
:DRONE-84 sao:lastupdate "2023-05-15T10:58:52.205-0300" .
:DRONE-84 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-84" .
:DRONE-84 sao:realizes :DRONE-117 .
:DRONE-84 sao:isImplementedBy :Component10046 .
:Component10046 sao:implements :DRONE-84 .
:DRONE-83 rdf:type owl:NamedIndividual .
:DRONE-83 rdf:type sao:DesignDefinition .
:DRONE-83 rdfs:label "Fly to first waypoint at assigned altitude during coordinated takeoff" .
:DRONE-83 rdfs:comment "When in COORDINATED_TAKEOFF mode and all UAVs have reached their target altitudes, each UAV shall fly in a direct path to the longitude and latitude of its first waypoint while maintaining its current altitude." .
:DRONE-83 sao:status "To Do" .
:DRONE-83 sao:creationdate "2023-05-13T17:12:24.208-0300" .
:DRONE-83 sao:lastupdate "2023-05-13T17:13:16.710-0300" .
:DRONE-83 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-83" .
:DRONE-83 sao:realizes :DRONE-49 .
:DRONE-83 sao:realizes :DRONE-117 .
:DRONE-82 rdf:type owl:NamedIndividual .
:DRONE-82 rdf:type sao:DesignDefinition .
:DRONE-82 rdfs:label "Fly to first waypoint at assigned altitude during coordinated takeoff" .
:DRONE-82 rdfs:comment "When in COORDINATED_TAKEOFF mode and all UAVs have reached their target altitudes, each UAV shall fly in a direct path to the longitude and latitude of its first waypoint while maintaining its current altitude." .
:DRONE-82 sao:status "To Do" .
:DRONE-82 sao:creationdate "2023-05-13T17:12:23.670-0300" .
:DRONE-82 sao:lastupdate "2023-05-15T10:58:52.001-0300" .
:DRONE-82 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-82" .
:DRONE-82 sao:isImplementedBy :Component10045 .
:Component10045 sao:implements :DRONE-82 .
:DRONE-81 rdf:type owl:NamedIndividual .
:DRONE-81 rdf:type sao:DesignDefinition .
:DRONE-81 rdfs:label "Hover after ascent during coordinated takeoff" .
:DRONE-81 rdfs:comment "When in COORDINATED_TAKEOFF mode and a UAV reaches its target altitude it shall hover in place until it receives a command to proceed to the first waypoint of its prescribed flight route." .
:DRONE-81 sao:status "To Do" .
:DRONE-81 sao:creationdate "2023-05-13T17:12:23.075-0300" .
:DRONE-81 sao:lastupdate "2023-05-15T10:58:51.804-0300" .
:DRONE-81 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-81" .
:DRONE-81 sao:isExplainedBy :DRONE-96 .
:DRONE-81 sao:realizes :DRONE-117 .
:DRONE-81 sao:isImplementedBy :Component10045 .
:Component10045 sao:implements :DRONE-81 .
:DRONE-80 rdf:type owl:NamedIndividual .
:DRONE-80 rdf:type sao:DesignDefinition .
:DRONE-80 rdfs:label "Each UAV ascends to a unique altitude during coordinated take off ascent" .
:DRONE-80 rdfs:comment "When in COORDINATED_TAKEOFF mode and commanded to takeoff, each UAV in the group will ascend to a unique takeoff altitude such that there is a minimum distance of 4 meters between each pair of specified altitudes." .
:DRONE-80 sao:status "To Do" .
:DRONE-80 sao:creationdate "2023-05-13T17:12:22.412-0300" .
:DRONE-80 sao:lastupdate "2023-05-13T17:13:16.147-0300" .
:DRONE-80 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-80" .
:DRONE-80 sao:isExplainedBy :DRONE-72 .
:DRONE-80 sao:realizes :DRONE-49 .
:DRONE-80 sao:realizes :DRONE-117 .
:DRONE-79 rdf:type owl:NamedIndividual .
:DRONE-79 rdf:type sao:DesignDefinition .
:DRONE-79 rdfs:label "Each UAV ascends to a unique altitude during coordinated take off ascent" .
:DRONE-79 rdfs:comment "When in COORDINATED_TAKEOFF mode and commanded to takeoff, each UAV in the group will ascend to a unique takeoff altitude such that there is a minimum distance of 4 meters between each pair of specified altitudes." .
:DRONE-79 sao:status "To Do" .
:DRONE-79 sao:creationdate "2023-05-13T17:12:21.868-0300" .
:DRONE-79 sao:lastupdate "2023-05-15T10:58:51.580-0300" .
:DRONE-79 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-79" .
:DRONE-79 sao:isImplementedBy :Component10045 .
:Component10045 sao:implements :DRONE-79 .
:DRONE-78 rdf:type owl:NamedIndividual .
:DRONE-78 rdf:type sao:SafetyRequirement .
:DRONE-78 rdfs:label "Return home along a unique path when issued RTL command" .
:DRONE-78 rdfs:comment "When the 'return to home' command is issued the 
FlightManager
 shall immediately command the the UAV to return to its original launch location using a unique flight route." .
:DRONE-78 sao:status "To Do" .
:DRONE-78 sao:creationdate "2023-05-13T17:12:21.311-0300" .
:DRONE-78 sao:lastupdate "2023-05-13T17:13:18.306-0300" .
:DRONE-78 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-78" .
:DRONE-78 sao:isExplainedBy :DRONE-74 .
:DRONE-78 sao:mitigates :DRONE-133 .
:DRONE-78 sao:isRealizedBy :DRONE-73 .
:DRONE-78 sao:isRealizedBy :DRONE-91 .
:DRONE-77 rdf:type owl:NamedIndividual .
:DRONE-77 rdf:type sao:DesignDefinition .
:DRONE-77 rdfs:label "Display battery life unit as a percentage" .
:DRONE-77 rdfs:comment "The battery availability shall be displayed as a percentage computed according to the manufacturer's claims of maximum battery capacity." .
:DRONE-77 sao:status "To Do" .
:DRONE-77 sao:creationdate "2023-05-13T17:12:20.713-0300" .
:DRONE-77 sao:lastupdate "2023-05-15T10:58:51.371-0300" .
:DRONE-77 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-77" .
:DRONE-77 sao:realizes :DRONE-153 .
:DRONE-77 sao:isImplementedBy :Component10043 .
:Component10043 sao:implements :DRONE-77 .
:DRONE-76 rdf:type owl:NamedIndividual .
:DRONE-76 rdf:type sao:DesignDefinition .
:DRONE-76 rdfs:label "Update UAV location frequency" .
:DRONE-76 rdfs:comment "The UAV location shall be updated on the map at the currently defined 
UI_UAV_REFRESH_RATE" .
:DRONE-76 sao:status "To Do" .
:DRONE-76 sao:creationdate "2023-05-13T17:12:20.088-0300" .
:DRONE-76 sao:lastupdate "2023-05-15T10:58:51.149-0300" .
:DRONE-76 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-76" .
:DRONE-76 sao:realizes :DRONE-28 .
:DRONE-76 sao:isImplementedBy :Component10043 .
:Component10043 sao:implements :DRONE-76 .
:DRONE-76 sao:isImplementedBy :Component10044 .
:Component10044 sao:implements :DRONE-76 .
:DRONE-75 rdf:type owl:NamedIndividual .
:DRONE-75 rdf:type sao:Assumption .
:DRONE-75 rdfs:label "Real-Time Flight UI display status of all active UAVs" .
:DRONE-75 rdfs:comment "The 
RealTimeFlightUI
 shall display the location and status of active UAVs." .
:DRONE-75 sao:status "To Do" .
:DRONE-75 sao:creationdate "2023-05-13T17:12:19.571-0300" .
:DRONE-75 sao:lastupdate "2023-05-13T17:13:15.183-0300" .
:DRONE-75 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-75" .
:DRONE-75 sao:explains :DRONE-28 .
:DRONE-74 rdf:type owl:NamedIndividual .
:DRONE-74 rdf:type sao:Assumption .
:DRONE-74 rdfs:label "User issues RTL command using Dronology UI" .
:DRONE-74 sao:status "To Do" .
:DRONE-74 sao:creationdate "2023-05-13T17:12:19.022-0300" .
:DRONE-74 sao:lastupdate "2023-05-13T17:13:15.009-0300" .
:DRONE-74 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-74" .
:DRONE-74 sao:explains :DRONE-78 .
:DRONE-73 rdf:type owl:NamedIndividual .
:DRONE-73 rdf:type sao:DesignDefinition .
:DRONE-73 rdfs:label "Dronology sends UAV to home coordinates using its uniques RTL altitude." .
:DRONE-73 rdfs:comment "User issues RTL command using Dronology UI" .
:DRONE-73 sao:status "To Do" .
:DRONE-73 sao:creationdate "2023-05-13T17:12:18.416-0300" .
:DRONE-73 sao:lastupdate "2023-05-15T10:58:50.895-0300" .
:DRONE-73 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-73" .
:DRONE-73 sao:realizes :DRONE-78 .
:DRONE-73 sao:isImplementedBy :Component10042 .
:Component10042 sao:implements :DRONE-73 .
:DRONE-73 sao:isImplementedBy :Component10043 .
:Component10043 sao:implements :DRONE-73 .
:DRONE-72 rdf:type owl:NamedIndividual .
:DRONE-72 rdf:type sao:Assumption .
:DRONE-72 rdfs:label "Sufficient vertical airspace exists to allocate each UAV its own altitude with vertical spacing of at least 5 meters from all other UAVs." .
:DRONE-72 sao:status "To Do" .
:DRONE-72 sao:creationdate "2023-05-13T17:12:17.871-0300" .
:DRONE-72 sao:lastupdate "2023-05-13T17:13:14.636-0300" .
:DRONE-72 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-72" .
:DRONE-72 sao:explains :DRONE-80 .
:DRONE-71 rdf:type owl:NamedIndividual .
:DRONE-71 rdf:type sao:Assumption .
:DRONE-71 rdfs:label "Sufficient vertical airspace exists to allocate each UAV its own altitude with vertical spacing of at least 5 meters from all other UAVs." .
:DRONE-71 sao:status "To Do" .
:DRONE-71 sao:creationdate "2023-05-13T17:12:17.345-0300" .
:DRONE-71 sao:lastupdate "2023-05-13T17:12:17.773-0300" .
:DRONE-71 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-71" .
:DRONE-70 rdf:type owl:NamedIndividual .
:DRONE-70 rdf:type sao:Requirement .
:DRONE-70 rdfs:label "When a GPS calibration error is reported, the dronology operator will issue a RTL command." .
:DRONE-70 rdfs:comment "When the RPIC determines that Dronology has lost control of the UAV for more than 
acceptable loss of communication
 minutes, then the RPIC shall take control." .
:DRONE-70 sao:status "To Do" .
:DRONE-70 sao:creationdate "2023-05-13T17:12:16.815-0300" .
:DRONE-70 sao:lastupdate "2023-05-13T17:13:14.464-0300" .
:DRONE-70 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-70" .
:DRONE-70 sao:mitigates :DRONE-26 .
:DRONE-69 rdf:type owl:NamedIndividual .
:DRONE-69 rdf:type sao:SafetyRequirement .
:DRONE-69 rdfs:label "The GCS shall monitor each UAV under its control for GPS calibration errors and shall report them to Dronology." .
:DRONE-69 rdfs:comment "The GCS shall monitor each UAV under its control for GPS calibration errors and shall report them to Dronology." .
:DRONE-69 sao:status "To Do" .
:DRONE-69 sao:creationdate "2023-05-13T17:12:16.259-0300" .
:DRONE-69 sao:lastupdate "2023-05-13T17:13:14.296-0300" .
:DRONE-69 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-69" .
:DRONE-69 sao:mitigates :DRONE-26 .
:DRONE-68 rdf:type owl:NamedIndividual .
:DRONE-68 rdf:type sao:Assumption .
:DRONE-68 rdfs:label "RPIC checks the geofence to ensure that the maximum altitude is 400 feet above ground level as allowed by FAA regulations." .
:DRONE-68 sao:status "To Do" .
:DRONE-68 sao:creationdate "2023-05-13T17:12:15.742-0300" .
:DRONE-68 sao:lastupdate "2023-05-13T17:13:14.123-0300" .
:DRONE-68 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-68" .
:DRONE-68 sao:explains :DRONE-61 .
:DRONE-67 rdf:type owl:NamedIndividual .
:DRONE-67 rdf:type sao:Requirement .
:DRONE-67 rdfs:label "When a route is run in the simulator and MINIMUM_SEPARATION_DISTANCE is violated an error shall be reported in the simulator log." .
:DRONE-67 rdfs:comment "When a route is run in the simulator and 
MINIMUM_SEPARATION_DISTANCE
 is violated an error shall be reported in the simulator log." .
:DRONE-67 sao:status "To Do" .
:DRONE-67 sao:creationdate "2023-05-13T17:12:15.182-0300" .
:DRONE-67 sao:lastupdate "2023-05-13T17:13:13.936-0300" .
:DRONE-67 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-67" .
:DRONE-67 sao:mitigates :DRONE-22 .
:DRONE-66 rdf:type owl:NamedIndividual .
:DRONE-66 rdf:type sao:Requirement .
:DRONE-66 rdfs:label "All routes are planned to ensure minimum separation of UAVs in flight at all times." .
:DRONE-66 rdfs:comment "All routes are carefully planned and tested in the simulator by the Dronology operator prior to physical flights to ensure minimum separation of UAVs by at least 8 meters vertical or horizontal distance at all times." .
:DRONE-66 sao:status "To Do" .
:DRONE-66 sao:creationdate "2023-05-13T17:12:14.628-0300" .
:DRONE-66 sao:lastupdate "2023-05-13T17:13:13.753-0300" .
:DRONE-66 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-66" .
:DRONE-66 sao:isExplainedBy :DRONE-30 .
:DRONE-66 sao:mitigates :DRONE-22 .
:DRONE-65 rdf:type owl:NamedIndividual .
:DRONE-65 rdf:type sao:DesignDefinition .
:DRONE-65 rdfs:label "The current battery capacity display shall be refreshed at least every 2 seconds." .
:DRONE-65 sao:status "To Do" .
:DRONE-65 sao:creationdate "2023-05-13T17:12:14.060-0300" .
:DRONE-65 sao:lastupdate "2023-05-13T17:13:13.582-0300" .
:DRONE-65 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-65" .
:DRONE-65 sao:realizes :DRONE-153 .
:DRONE-64 rdf:type owl:NamedIndividual .
:DRONE-64 rdf:type sao:Assumption .
:DRONE-64 rdfs:label "Python Based Ground Control Station V1.0 with control logic distributed between ground-based GCS and Processor onboard the UAV." .
:DRONE-64 sao:status "To Do" .
:DRONE-64 sao:creationdate "2023-05-13T17:12:13.554-0300" .
:DRONE-64 sao:lastupdate "2023-05-13T17:13:13.412-0300" .
:DRONE-64 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-64" .
:DRONE-64 sao:explains :DRONE-31 .
:DRONE-63 rdf:type owl:NamedIndividual .
:DRONE-63 rdf:type sao:Assumption .
:DRONE-63 rdfs:label "Python Based Ground Control Station V1.0 with all control logic on the ground." .
:DRONE-63 sao:status "To Do" .
:DRONE-63 sao:creationdate "2023-05-13T17:12:13.036-0300" .
:DRONE-63 sao:lastupdate "2023-05-13T17:13:13.245-0300" .
:DRONE-63 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-63" .
:DRONE-63 sao:explains :DRONE-31 .
:DRONE-62 rdf:type owl:NamedIndividual .
:DRONE-62 rdf:type sao:Context .
:DRONE-62 rdfs:label "UAVs may fly in controlled airspaces where maximum altitude is determined by Air Traffic Controllers prior to each flight." .
:DRONE-62 sao:status "To Do" .
:DRONE-62 sao:creationdate "2023-05-13T17:12:12.474-0300" .
:DRONE-62 sao:lastupdate "2023-05-15T09:47:00.188-0300" .
:DRONE-62 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-62" .
:DRONE-62 sao:contextualizes :DRONE-61 .
:DRONE-61 rdf:type owl:NamedIndividual .
:DRONE-61 rdf:type sao:SafetyRequirement .
:DRONE-61 rdfs:label "Prior to flying in a controlled airspace, the maximum altitude of each UAV is set through its internal geofence." .
:DRONE-61 sao:status "To Do" .
:DRONE-61 sao:creationdate "2023-05-13T17:12:11.945-0300" .
:DRONE-61 sao:lastupdate "2023-05-15T09:47:00.124-0300" .
:DRONE-61 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-61" .
:DRONE-61 sao:isContextualizedBy :DRONE-62 .
:DRONE-61 sao:isExplainedBy :DRONE-68 .
:DRONE-61 sao:mitigates :DRONE-60 .
:DRONE-60 rdf:type owl:NamedIndividual .
:DRONE-60 rdf:type sao:Hazard .
:DRONE-60 rdfs:label "UAV flies above the altitude permitted by FAA regulations." .
:DRONE-60 sao:status "To Do" .
:DRONE-60 sao:creationdate "2023-05-13T17:12:11.411-0300" .
:DRONE-60 sao:lastupdate "2023-05-13T17:13:12.920-0300" .
:DRONE-60 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-60" .
:DRONE-60 sao:isMitigatedBy :DRONE-61 .
:DRONE-59 rdf:type owl:NamedIndividual .
:DRONE-59 rdf:type sao:Assumption .
:DRONE-59 rdfs:label "Ground Station Middleware handles all communication between Dronology and external GCSs." .
:DRONE-59 sao:status "To Do" .
:DRONE-59 sao:creationdate "2023-05-13T17:12:10.879-0300" .
:DRONE-59 sao:lastupdate "2023-05-13T17:13:12.688-0300" .
:DRONE-59 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-59" .
:DRONE-59 sao:explains :DRONE-31 .
:DRONE-58 rdf:type owl:NamedIndividual .
:DRONE-58 rdf:type sao:Context .
:DRONE-58 rdfs:label "Use of global altitude requires additional instrumentation in order to achieve required degrees of accuracy." .
:DRONE-58 sao:status "To Do" .
:DRONE-58 sao:creationdate "2023-05-13T17:12:10.370-0300" .
:DRONE-58 sao:lastupdate "2023-05-15T09:47:24.016-0300" .
:DRONE-58 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-58" .
:DRONE-58 sao:contextualizes :DRONE-47 .
:DRONE-57 rdf:type owl:NamedIndividual .
:DRONE-57 rdf:type sao:DesignDefinition .
:DRONE-57 rdfs:label "When a _MINIMUM_SEPARATION_DISTANCE_ violation occurs, Dronology will issue a zero NED directive causing UAVs to hover in place.." .
:DRONE-57 rdfs:comment "When a 
MINIMUM_SEPARATION_DISTANCE
 violation occurs, Dronology will issue a zero NED directive to both impacted UAVs causing them both to stop and hover in place." .
:DRONE-57 sao:status "To Do" .
:DRONE-57 sao:creationdate "2023-05-13T17:12:09.800-0300" .
:DRONE-57 sao:lastupdate "2023-05-15T10:58:50.686-0300" .
:DRONE-57 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-57" .
:DRONE-57 sao:realizes :DRONE-54 .
:DRONE-57 sao:isImplementedBy :Component10041 .
:Component10041 sao:implements :DRONE-57 .
:DRONE-56 rdf:type owl:NamedIndividual .
:DRONE-56 rdf:type sao:DesignDefinition .
:DRONE-56 rdfs:label "Dronology monitors the distance between all active pairs of UAVs and checks for proximity violations" .
:DRONE-56 rdfs:comment "Dronology shall monitor the distance between all active pairs of UAVs and check for violations of the 
MINIMUM_SEPARATION_DISTANCE
." .
:DRONE-56 sao:status "To Do" .
:DRONE-56 sao:creationdate "2023-05-13T17:12:09.225-0300" .
:DRONE-56 sao:lastupdate "2023-05-15T10:58:50.473-0300" .
:DRONE-56 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-56" .
:DRONE-56 sao:realizes :DRONE-54 .
:DRONE-56 sao:isImplementedBy :Component10041 .
:Component10041 sao:implements :DRONE-56 .
:DRONE-55 rdf:type owl:NamedIndividual .
:DRONE-55 rdf:type sao:Context .
:DRONE-55 rdfs:label "External 3DR simulator does not accurately model NED commands and is not reliable for testing collision avoidance." .
:DRONE-55 sao:status "To Do" .
:DRONE-55 sao:creationdate "2023-05-13T17:12:08.712-0300" .
:DRONE-55 sao:lastupdate "2023-05-15T09:58:43.922-0300" .
:DRONE-55 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-55" .
:DRONE-55 sao:contextualizes :DRONE-54 .
:DRONE-54 rdf:type owl:NamedIndividual .
:DRONE-54 rdf:type sao:SafetyRequirement .
:DRONE-54 rdfs:label "When two UAVs violate the _MINIMUM_SEPARATION_DISTANCE_ they will both stop and hover in place." .
:DRONE-54 rdfs:comment "When two UAVs violate the 
MINIMUM_SEPARATION_DISTANCE
 they will both stop and hover in place." .
:DRONE-54 sao:status "To Do" .
:DRONE-54 sao:creationdate "2023-05-13T17:12:08.165-0300" .
:DRONE-54 sao:lastupdate "2023-05-15T09:58:43.852-0300" .
:DRONE-54 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-54" .
:DRONE-54 sao:isContextualizedBy :DRONE-55 .
:DRONE-54 sao:mitigates :DRONE-22 .
:DRONE-54 sao:isRealizedBy :DRONE-56 .
:DRONE-54 sao:isRealizedBy :DRONE-57 .
:DRONE-53 rdf:type owl:NamedIndividual .
:DRONE-53 rdf:type sao:Assumption .
:DRONE-53 rdfs:label "All dynamically generated waypoints are validated to be above ground level" .
:DRONE-53 rdfs:comment "Waypoints that are dynamically generated by dronology are assigned altitudes above ground level." .
:DRONE-53 sao:status "To Do" .
:DRONE-53 sao:creationdate "2023-05-13T17:12:07.629-0300" .
:DRONE-53 sao:lastupdate "2023-05-13T17:13:11.561-0300" .
:DRONE-53 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-53" .
:DRONE-53 sao:explains :DRONE-49 .
:DRONE-52 rdf:type owl:NamedIndividual .
:DRONE-52 rdf:type sao:Assumption .
:DRONE-52 rdfs:label "All flight routes imported using the mission planner interface are constructed using the Dronology UI." .
:DRONE-52 rdfs:comment "Flight routes imported using the mission planner interface are constructed using the Dronology UI." .
:DRONE-52 sao:status "To Do" .
:DRONE-52 sao:creationdate "2023-05-13T17:12:07.054-0300" .
:DRONE-52 sao:lastupdate "2023-05-13T17:13:11.322-0300" .
:DRONE-52 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-52" .
:DRONE-52 sao:explains :DRONE-49 .
:DRONE-51 rdf:type owl:NamedIndividual .
:DRONE-51 rdf:type sao:DesignDefinition .
:DRONE-51 rdfs:label "The GCS uses the services of Dronekit Python to transform waypoint requests into Mavlink and to transmit those commands to the UAV pixhawk controller." .
:DRONE-51 sao:status "To Do" .
:DRONE-51 sao:creationdate "2023-05-13T17:12:06.481-0300" .
:DRONE-51 sao:lastupdate "2023-05-13T17:13:11.127-0300" .
:DRONE-51 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-51" .
:DRONE-51 sao:realizes :DRONE-49 .
:DRONE-50 rdf:type owl:NamedIndividual .
:DRONE-50 rdf:type sao:DesignDefinition .
:DRONE-50 rdfs:label "Waypoints generated via the Dronology UI are validated to check that their altitude is greater than zero." .
:DRONE-50 rdfs:comment "Waypoints are created in the Dronology UI where their altitude is checked to determine that it is greater than zero." .
:DRONE-50 sao:status "To Do" .
:DRONE-50 sao:creationdate "2023-05-13T17:12:05.887-0300" .
:DRONE-50 sao:lastupdate "2023-05-15T10:58:50.255-0300" .
:DRONE-50 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-50" .
:DRONE-50 sao:realizes :DRONE-49 .
:DRONE-50 sao:isImplementedBy :Component10040 .
:Component10040 sao:implements :DRONE-50 .
:DRONE-49 rdf:type owl:NamedIndividual .
:DRONE-49 rdf:type sao:SafetyRequirement .
:DRONE-49 rdfs:label "Waypoint commands sent to the UAV will represent valid coordinates that will not cause collisions with the terrain." .
:DRONE-49 rdfs:comment "All waypoint directives issued by Dronology to a UAV will represent valid coordinates that will not cause the UAV to fly into the terrain." .
:DRONE-49 sao:status "To Do" .
:DRONE-49 sao:creationdate "2023-05-13T17:12:05.348-0300" .
:DRONE-49 sao:lastupdate "2023-05-13T17:13:17.127-0300" .
:DRONE-49 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-49" .
:DRONE-49 sao:isExplainedBy :DRONE-52 .
:DRONE-49 sao:isExplainedBy :DRONE-53 .
:DRONE-49 sao:mitigates :DRONE-19 .
:DRONE-49 sao:isRealizedBy :DRONE-50 .
:DRONE-49 sao:isRealizedBy :DRONE-51 .
:DRONE-49 sao:isRealizedBy :DRONE-80 .
:DRONE-49 sao:isRealizedBy :DRONE-83 .
:DRONE-49 sao:isRealizedBy :DRONE-86 .
:DRONE-48 rdf:type owl:NamedIndividual .
:DRONE-48 rdf:type sao:Context .
:DRONE-48 rdfs:label "UAVs are not equipped with ground facing sensors" .
:DRONE-48 rdfs:comment "Currently, UAVs are not equipped with ground facing sensors and are therefore not able to detect changes in terrain altitude." .
:DRONE-48 sao:status "To Do" .
:DRONE-48 sao:creationdate "2023-05-13T17:12:04.807-0300" .
:DRONE-48 sao:lastupdate "2023-05-15T09:59:32.332-0300" .
:DRONE-48 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-48" .
:DRONE-48 sao:contextualizes :DRONE-23 .
:DRONE-47 rdf:type owl:NamedIndividual .
:DRONE-47 rdf:type sao:DesignDefinition .
:DRONE-47 rdfs:label "Altitude commands use relative altitude which is defined relative to the onground coordinates of the UAV prior to takeoff." .
:DRONE-47 rdfs:comment "Altitude commands use relative altitude which is defined relative to the onground coordinates of the UAV prior to takeoff." .
:DRONE-47 sao:status "To Do" .
:DRONE-47 sao:creationdate "2023-05-13T17:12:04.211-0300" .
:DRONE-47 sao:lastupdate "2023-05-15T10:58:49.870-0300" .
:DRONE-47 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-47" .
:DRONE-47 sao:isContextualizedBy :DRONE-58 .
:DRONE-47 sao:realizes :DRONE-23 .
:DRONE-47 sao:isImplementedBy :Component10038 .
:Component10038 sao:implements :DRONE-47 .
:DRONE-47 sao:isImplementedBy :Component10039 .
:Component10039 sao:implements :DRONE-47 .
:DRONE-46 rdf:type owl:NamedIndividual .
:DRONE-46 rdf:type sao:Requirement .
:DRONE-46 rdfs:label "Operator only assigns flight routes with waypoints above terrain level" .
:DRONE-46 rdfs:comment "When the flying area includes hilly terrain, the operator inspects all assigned flight routes to ensure that waypoints are above the highest terrain level." .
:DRONE-46 sao:status "To Do" .
:DRONE-46 sao:creationdate "2023-05-13T17:12:03.640-0300" .
:DRONE-46 sao:lastupdate "2023-05-13T17:13:10.237-0300" .
:DRONE-46 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-46" .
:DRONE-46 sao:refines :DRONE-23 .
:DRONE-45 rdf:type owl:NamedIndividual .
:DRONE-45 rdf:type sao:Assumption .
:DRONE-45 rdfs:label "Mission planner UAV calibration" .
:DRONE-45 rdfs:comment "UAV is calibrated using Mission Planner or QGroundControl 3rd party software." .
:DRONE-45 sao:status "To Do" .
:DRONE-45 sao:creationdate "2023-05-13T17:12:03.060-0300" .
:DRONE-45 sao:lastupdate "2023-05-13T17:13:10.062-0300" .
:DRONE-45 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-45" .
:DRONE-45 sao:explains :DRONE-44 .
:DRONE-44 rdf:type owl:NamedIndividual .
:DRONE-44 rdf:type sao:SafetyRequirement .
:DRONE-44 rdfs:label "UAV is calibrated prior to flight" .
:DRONE-44 rdfs:comment "The UAV passes all mandatory calibration tests prior to flight including compass, accelerometer. (List more)" .
:DRONE-44 sao:status "To Do" .
:DRONE-44 sao:creationdate "2023-05-13T17:12:02.476-0300" .
:DRONE-44 sao:lastupdate "2023-05-13T17:13:10.117-0300" .
:DRONE-44 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-44" .
:DRONE-44 sao:isExplainedBy :DRONE-45 .
:DRONE-44 sao:mitigates :DRONE-26 .
:DRONE-43 rdf:type owl:NamedIndividual .
:DRONE-43 rdf:type sao:Assumption .
:DRONE-43 rdfs:label "River searches are more effective in a downstream direction." .
:DRONE-43 sao:status "To Do" .
:DRONE-43 sao:creationdate "2023-05-13T17:12:01.789-0300" .
:DRONE-43 sao:lastupdate "2023-05-13T17:13:09.704-0300" .
:DRONE-43 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-43" .
:DRONE-43 sao:explains :DRONE-108 .
:DRONE-42 rdf:type owl:NamedIndividual .
:DRONE-42 rdf:type sao:Assumption .
:DRONE-42 rdfs:label "UAVs used for search and rescue can fly 10km on a full battery." .
:DRONE-42 rdfs:comment "A drone can fly for 20 minutes at 20 miles per hour on a full battery." .
:DRONE-42 sao:status "To Do" .
:DRONE-42 sao:creationdate "2023-05-13T17:12:01.232-0300" .
:DRONE-42 sao:lastupdate "2023-05-13T17:13:09.528-0300" .
:DRONE-42 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-42" .
:DRONE-42 sao:explains :DRONE-110 .
:DRONE-41 rdf:type owl:NamedIndividual .
:DRONE-41 rdf:type sao:DesignDefinition .
:DRONE-41 rdfs:label "Evaluate route allocations for safety violations" .
:DRONE-41 rdfs:comment "Check that the route allocation does not viollate the set of previously identified constraints." .
:DRONE-41 sao:status "To Do" .
:DRONE-41 sao:creationdate "2023-05-13T17:12:00.623-0300" .
:DRONE-41 sao:lastupdate "2023-05-15T14:48:23.465-0300" .
:DRONE-41 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-41" .
:DRONE-41 sao:realizes :DRONE-34 .
:DRONE-41 sao:realizes :DRONE-110 .
:DRONE-40 rdf:type owl:NamedIndividual .
:DRONE-40 rdf:type sao:DesignDefinition .
:DRONE-40 rdfs:label "Estimate the quality of a route allocation by computing a fitness function based on diverse coverage metrics." .
:DRONE-40 rdfs:comment "When a route allocation has been computed for the available UAVs and a given region, estimate the quality of a route allocation by computing a fitness function." .
:DRONE-40 sao:status "To Do" .
:DRONE-40 sao:creationdate "2023-05-13T17:12:00.017-0300" .
:DRONE-40 sao:lastupdate "2023-05-15T14:43:35.392-0300" .
:DRONE-40 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-40" .
:DRONE-40 sao:realizes :DRONE-34 .
:DRONE-40 sao:realizes :DRONE-106 .
:DRONE-40 sao:realizes :DRONE-108 .
:DRONE-40 sao:realizes :DRONE-109 .
:DRONE-40 sao:realizes :DRONE-111 .
:DRONE-40 sao:realizes :DRONE-112 .
:DRONE-40 sao:realizes :DRONE-154 .
:DRONE-39 rdf:type owl:NamedIndividual .
:DRONE-39 rdf:type sao:Context .
:DRONE-39 rdfs:label "A successful search finds a live victim as quickly as possible while minimizing risk to the rescuers." .
:DRONE-39 sao:status "To Do" .
:DRONE-39 sao:creationdate "2023-05-13T17:11:59.506-0300" .
:DRONE-39 sao:lastupdate "2023-05-15T10:00:29.377-0300" .
:DRONE-39 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-39" .
:DRONE-39 sao:contextualizes :DRONE-38 .
:DRONE-38 rdf:type owl:NamedIndividual .
:DRONE-38 rdf:type sao:Assumption .
:DRONE-38 rdfs:label "Optimize chance of successful search through allocation of routes to available UAVs" .
:DRONE-38 rdfs:comment "Given a set of candidate routes and a set of available UAVs, allocate the routes to the UAVs in a way that optimizes the likelihood of a successful search." .
:DRONE-38 sao:status "To Do" .
:DRONE-38 sao:creationdate "2023-05-13T17:11:58.963-0300" .
:DRONE-38 sao:lastupdate "2023-05-15T10:00:29.306-0300" .
:DRONE-38 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-38" .
:DRONE-38 sao:isContextualizedBy :DRONE-39 .
:DRONE-38 sao:explains :DRONE-36 .
:DRONE-37 rdf:type owl:NamedIndividual .
:DRONE-37 rdf:type sao:Assumption .
:DRONE-37 rdfs:label "Given a demarcated region of the river,  generate a set of candidate flight routes" .
:DRONE-37 rdfs:comment "Given a region of the river demarcated by both river banks, generate flight routes that cover river banks, central parts of the river, and priority areas." .
:DRONE-37 sao:status "To Do" .
:DRONE-37 sao:creationdate "2023-05-13T17:11:58.445-0300" .
:DRONE-37 sao:lastupdate "2023-05-13T17:13:08.564-0300" .
:DRONE-37 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-37" .
:DRONE-37 sao:explains :DRONE-36 .
:DRONE-36 rdf:type owl:NamedIndividual .
:DRONE-36 rdf:type sao:Assumption .
:DRONE-36 rdfs:label "Routes are automatically generated, allocated to UAVs, and executed during  search and rescue" .
:DRONE-36 sao:status "To Do" .
:DRONE-36 sao:creationdate "2023-05-13T17:11:57.920-0300" .
:DRONE-36 sao:lastupdate "2023-05-13T17:13:08.805-0300" .
:DRONE-36 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-36" .
:DRONE-36 sao:explains :DRONE-34 .
:DRONE-36 sao:isExplainedBy :DRONE-37 .
:DRONE-36 sao:isExplainedBy :DRONE-38 .
:DRONE-35 rdf:type owl:NamedIndividual .
:DRONE-35 rdf:type sao:Assumption .
:DRONE-35 rdfs:label "User Interface must be intuitive for user under time pressure and use outside in the search area." .
:DRONE-35 rdfs:comment "A trained river rescuer with basic training in the area mapping feature will intuitively be able to retrieve and modify previously mapped regions of the river, map new regions, and dispatch UAVs to search the region." .
:DRONE-35 sao:status "To Do" .
:DRONE-35 sao:creationdate "2023-05-13T17:11:57.351-0300" .
:DRONE-35 sao:lastupdate "2023-05-13T17:13:08.160-0300" .
:DRONE-35 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-35" .
:DRONE-35 sao:explains :DRONE-33 .
:DRONE-34 rdf:type owl:NamedIndividual .
:DRONE-34 rdf:type sao:SafetyRequirement .
:DRONE-34 rdfs:label "Automate the process of generating routes for river search" .
:DRONE-34 rdfs:comment "Automate the process of generating routes for river search in a predefined section of the river." .
:DRONE-34 sao:status "To Do" .
:DRONE-34 sao:creationdate "2023-05-13T17:11:56.801-0300" .
:DRONE-34 sao:lastupdate "2023-05-15T14:28:30.315-0300" .
:DRONE-34 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-34" .
:DRONE-34 sao:isExplainedBy :DRONE-36 .
:DRONE-34 sao:isExplainedBy :DRONE-134 .
:DRONE-34 sao:mitigates :DRONE-135 .
:DRONE-34 sao:isRealizedBy :DRONE-40 .
:DRONE-34 sao:isRealizedBy :DRONE-41 .
:DRONE-34 sao:isRealizedBy :DRONE-103 .
:DRONE-34 sao:isRealizedBy :DRONE-104 .
:DRONE-34 sao:isRealizedBy :DRONE-113 .
:DRONE-34 sao:isRealizedBy :DRONE-115 .
:DRONE-34 sao:isRefinedBy :DRONE-33 .
:DRONE-33 rdf:type owl:NamedIndividual .
:DRONE-33 rdf:type sao:Requirement .
:DRONE-33 rdfs:label "UI enables the user to map river region over which the search will be conducted" .
:DRONE-33 rdfs:comment "The user shall utilize the UI to map the river banks in order to demarcate a region of the river to be searched." .
:DRONE-33 sao:status "To Do" .
:DRONE-33 sao:creationdate "2023-05-13T17:11:56.275-0300" .
:DRONE-33 sao:lastupdate "2023-05-15T14:30:01.355-0300" .
:DRONE-33 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-33" .
:DRONE-33 sao:isExplainedBy :DRONE-35 .
:DRONE-33 sao:refines :DRONE-34 .
:DRONE-33 sao:isRefinedBy :DRONE-114 .
:DRONE-32 rdf:type owl:NamedIndividual .
:DRONE-32 rdf:type sao:Context .
:DRONE-32 rdfs:label "Public use of Dronology is limited to specific events, limiting the opportunity for rogue UAVs to activate in the system." .
:DRONE-32 rdfs:comment "When used in public settings, Dronology is activated for limited periods of time to support specific events such as River Rescues, significantly decreasing the opportunity for rogue UAVs to attempt to register." .
:DRONE-32 sao:status "To Do" .
:DRONE-32 sao:creationdate "2023-05-13T17:11:55.725-0300" .
:DRONE-32 sao:lastupdate "2023-05-15T09:59:58.929-0300" .
:DRONE-32 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-32" .
:DRONE-32 sao:contextualizes :DRONE-27 .
:DRONE-31 rdf:type owl:NamedIndividual .
:DRONE-31 rdf:type sao:SafetyRequirement .
:DRONE-31 rdfs:label "UAVs connect to dronology via a well defined handshake protocol" .
:DRONE-31 rdfs:comment "UAVs connect to dronology via a GCS which leverages a well defined handshake protocol with Dronology's Ground-Station middleware." .
:DRONE-31 sao:status "To Do" .
:DRONE-31 sao:creationdate "2023-05-13T17:11:55.176-0300" .
:DRONE-31 sao:lastupdate "2023-05-13T17:13:13.463-0300" .
:DRONE-31 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-31" .
:DRONE-31 sao:isExplainedBy :DRONE-59 .
:DRONE-31 sao:isExplainedBy :DRONE-63 .
:DRONE-31 sao:isExplainedBy :DRONE-64 .
:DRONE-31 sao:mitigates :DRONE-27 .
:DRONE-30 rdf:type owl:NamedIndividual .
:DRONE-30 rdf:type sao:Assumption .
:DRONE-30 rdfs:label "Routes that are free of collisions with simulated UAVs will also be free of collisions with physical UAVs." .
:DRONE-30 rdfs:comment "The fidelity of the simulator is sufficient such that collision free routes set at a minimum of 8 meters separation in the simulation will also be collision free in the physical worls." .
:DRONE-30 sao:status "To Do" .
:DRONE-30 sao:creationdate "2023-05-13T17:11:54.614-0300" .
:DRONE-30 sao:lastupdate "2023-05-13T17:13:07.148-0300" .
:DRONE-30 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-30" .
:DRONE-30 sao:explains :DRONE-66 .
:DRONE-29 rdf:type owl:NamedIndividual .
:DRONE-29 rdf:type sao:Requirement .
:DRONE-29 rdfs:label "Dronology operator will manually disable GCS in case of unknown UAV activation" .
:DRONE-29 sao:status "To Do" .
:DRONE-29 sao:creationdate "2023-05-13T17:11:54.108-0300" .
:DRONE-29 sao:lastupdate "2023-05-13T17:13:06.947-0300" .
:DRONE-29 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-29" .
:DRONE-29 sao:mitigates :DRONE-27 .
:DRONE-28 rdf:type owl:NamedIndividual .
:DRONE-28 rdf:type sao:SafetyRequirement .
:DRONE-28 rdfs:label "When Dronology service is active it shall be monitored by a human operator." .
:DRONE-28 rdfs:comment "Dronology provides features to allow a human operator to monitor active flights." .
:DRONE-28 sao:status "To Do" .
:DRONE-28 sao:creationdate "2023-05-13T17:11:53.550-0300" .
:DRONE-28 sao:lastupdate "2023-05-13T17:13:19.937-0300" .
:DRONE-28 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-28" .
:DRONE-28 sao:isExplainedBy :DRONE-75 .
:DRONE-28 sao:mitigates :DRONE-27 .
:DRONE-28 sao:isRealizedBy :DRONE-76 .
:DRONE-28 sao:isRealizedBy :DRONE-97 .
:DRONE-28 sao:isRealizedBy :DRONE-98 .
:DRONE-28 sao:isRealizedBy :DRONE-99 .
:DRONE-28 sao:isRealizedBy :DRONE-100 .
:DRONE-27 rdf:type owl:NamedIndividual .
:DRONE-27 rdf:type sao:Hazard .
:DRONE-27 rdfs:label "An untrusted UAV registers with Dronology, fails to comply with commands, and creates chaos in the airspace." .
:DRONE-27 rdfs:comment "An untrusted UAV registers with Dronology, fails to comply with commands, and creates chaos in the airspace. <Probability>Probability of hazard occurring is negligible given current flying locations.</Probability>" .
:DRONE-27 sao:status "To Do" .
:DRONE-27 sao:creationdate "2023-05-13T17:11:53.018-0300" .
:DRONE-27 sao:lastupdate "2023-05-15T09:59:58.864-0300" .
:DRONE-27 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-27" .
:DRONE-27 sao:isContextualizedBy :DRONE-32 .
:DRONE-27 sao:isMitigatedBy :DRONE-28 .
:DRONE-27 sao:isMitigatedBy :DRONE-29 .
:DRONE-27 sao:isMitigatedBy :DRONE-31 .
:DRONE-26 rdf:type owl:NamedIndividual .
:DRONE-26 rdf:type sao:Hazard .
:DRONE-26 rdfs:label "UAV compass calibration error causes UAV to fly in incorrect direction" .
:DRONE-26 rdfs:comment "UAV compass is not adequately calibrated and UAV flies in incorrect direction." .
:DRONE-26 sao:status "To Do" .
:DRONE-26 sao:creationdate "2023-05-13T17:11:52.462-0300" .
:DRONE-26 sao:lastupdate "2023-05-13T17:13:28.336-0300" .
:DRONE-26 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-26" .
:DRONE-26 sao:isMitigatedBy :DRONE-44 .
:DRONE-26 sao:isMitigatedBy :DRONE-69 .
:DRONE-26 sao:isMitigatedBy :DRONE-70 .
:DRONE-26 sao:isMitigatedBy :DRONE-152 .
:DRONE-25 rdf:type owl:NamedIndividual .
:DRONE-25 rdf:type sao:Hazard .
:DRONE-25 rdfs:label "Satellite signals are lost causing the UAV to lose accurate localization and fly in seemingly random directions to achieve its target waypoint." .
:DRONE-25 sao:status "To Do" .
:DRONE-25 sao:creationdate "2023-05-13T17:11:51.886-0300" .
:DRONE-25 sao:lastupdate "2023-05-13T17:13:28.141-0300" .
:DRONE-25 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-25" .
:DRONE-25 sao:isExplainedBy :DRONE-127 .
:DRONE-25 sao:isMitigatedBy :DRONE-152 .
:DRONE-24 rdf:type owl:NamedIndividual .
:DRONE-24 rdf:type sao:Hazard .
:DRONE-24 rdfs:label "Motor fails during UAV flight" .
:DRONE-24 rdfs:comment "Motor fails during flight." .
:DRONE-24 sao:status "To Do" .
:DRONE-24 sao:creationdate "2023-05-13T17:11:51.309-0300" .
:DRONE-24 sao:lastupdate "2023-05-13T17:11:51.773-0300" .
:DRONE-24 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-24" .
:DRONE-23 rdf:type owl:NamedIndividual .
:DRONE-23 rdf:type sao:SafetyRequirement .
:DRONE-23 rdfs:label "All waypoints in flight routes assigned to UAV must be at least 3 meters above the highest terrain in the flying zone." .
:DRONE-23 rdfs:comment "All waypoints in flight routes assigned to UAV must be at least 3 meters above the highest terrain in the flying zone" .
:DRONE-23 sao:status "To Do" .
:DRONE-23 sao:creationdate "2023-05-13T17:11:50.706-0300" .
:DRONE-23 sao:lastupdate "2023-05-15T09:59:32.265-0300" .
:DRONE-23 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-23" .
:DRONE-23 sao:isContextualizedBy :DRONE-48 .
:DRONE-23 sao:mitigates :DRONE-19 .
:DRONE-23 sao:isRealizedBy :DRONE-47 .
:DRONE-23 sao:isRefinedBy :DRONE-46 .
:DRONE-22 rdf:type owl:NamedIndividual .
:DRONE-22 rdf:type sao:Hazard .
:DRONE-22 rdfs:label "Midair collision during flight execution" .
:DRONE-22 sao:status "To Do" .
:DRONE-22 sao:creationdate "2023-05-13T17:11:50.183-0300" .
:DRONE-22 sao:lastupdate "2023-05-13T17:13:14.003-0300" .
:DRONE-22 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-22" .
:DRONE-22 sao:isMitigatedBy :DRONE-54 .
:DRONE-22 sao:isMitigatedBy :DRONE-66 .
:DRONE-22 sao:isMitigatedBy :DRONE-67 .
:DRONE-21 rdf:type owl:NamedIndividual .
:DRONE-21 rdf:type sao:Hazard .
:DRONE-21 rdfs:label "UAVs collide with each other during landing" .
:DRONE-21 sao:status "To Do" .
:DRONE-21 sao:creationdate "2023-05-13T17:11:49.632-0300" .
:DRONE-21 sao:lastupdate "2023-05-13T17:11:50.080-0300" .
:DRONE-21 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-21" .
:DRONE-20 rdf:type owl:NamedIndividual .
:DRONE-20 rdf:type sao:Hazard .
:DRONE-20 rdfs:label "UAV flies into a fixed stationary object such as a building or tree" .
:DRONE-20 sao:status "To Do" .
:DRONE-20 sao:creationdate "2023-05-13T17:11:49.078-0300" .
:DRONE-20 sao:lastupdate "2023-05-13T17:13:26.979-0300" .
:DRONE-20 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-20" .
:DRONE-20 sao:isExplainedBy :DRONE-127 .
:DRONE-20 sao:isMitigatedBy :DRONE-143 .
:DRONE-19 rdf:type owl:NamedIndividual .
:DRONE-19 rdf:type sao:Hazard .
:DRONE-19 rdfs:label "UAV receives a goto directive that causes it to fly into terrain" .
:DRONE-19 rdfs:comment "UAV receives a waypoint command that causes it to fly into terrain" .
:DRONE-19 sao:status "To Do" .
:DRONE-19 sao:creationdate "2023-05-13T17:11:48.474-0300" .
:DRONE-19 sao:lastupdate "2023-05-13T17:13:23.801-0300" .
:DRONE-19 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-19" .
:DRONE-19 sao:isExplainedBy :DRONE-127 .
:DRONE-19 sao:isMitigatedBy :DRONE-23 .
:DRONE-19 sao:isMitigatedBy :DRONE-49 .
:DRONE-18 rdf:type owl:NamedIndividual .
:DRONE-18 rdf:type sao:Hazard .
:DRONE-18 rdfs:label "UAV collides with a flying animal (e.g., a goose)" .
:DRONE-18 sao:status "To Do" .
:DRONE-18 sao:creationdate "2023-05-13T17:11:47.746-0300" .
:DRONE-18 sao:lastupdate "2023-05-13T17:11:48.357-0300" .
:DRONE-18 sao:externaluri "https://arcade-dare.atlassian.net/browse/DRONE-18" .
:Component10041 rdf:type owl:NamedIndividual .
:Component10041 rdf:type sao:Component .
:Component10041 rdfs:label "ncore.collisionavoidance" .
:Component10041 rdfs:comment "" .
:Component10038 rdf:type owl:NamedIndividual .
:Component10038 rdf:type sao:Component .
:Component10038 rdfs:label "ncore.coordinate" .
:Component10038 rdfs:comment "" .
:Component10048 rdf:type owl:NamedIndividual .
:Component10048 rdf:type sao:Component .
:Component10048 rdfs:label "ncore.flight.internal" .
:Component10048 rdfs:comment "" .
:Component10047 rdf:type owl:NamedIndividual .
:Component10047 rdf:type sao:Component .
:Component10047 rdfs:label "ncore.flightzone" .
:Component10047 rdfs:comment "" .
:Component10039 rdf:type owl:NamedIndividual .
:Component10039 rdf:type sao:Component .
:Component10039 rdfs:label "ncore.vehicle" .
:Component10039 rdfs:comment "" .
:Component10042 rdf:type owl:NamedIndividual .
:Component10042 rdf:type sao:Component .
:Component10042 rdfs:label "ngstation.connector.messages" .
:Component10042 rdfs:comment "" .
:Component10050 rdf:type owl:NamedIndividual .
:Component10050 rdf:type sao:Component .
:Component10050 rdfs:label "nservices.areamapping" .
:Component10050 rdfs:comment "" .
:Component10051 rdf:type owl:NamedIndividual .
:Component10051 rdf:type sao:Component .
:Component10051 rdfs:label "nservices.core.areamapping" .
:Component10051 rdfs:comment "" .
:Component10053 rdf:type owl:NamedIndividual .
:Component10053 rdf:type sao:Component .
:Component10053 rdfs:label "nservices.core.items" .
:Component10053 rdfs:comment "" .
:Component10052 rdf:type owl:NamedIndividual .
:Component10052 rdf:type sao:Component .
:Component10052 rdfs:label "nservices.extensions.areamapping" .
:Component10052 rdfs:comment "" .
:Component10046 rdf:type owl:NamedIndividual .
:Component10046 rdf:type sao:Component .
:Component10046 rdfs:label "nservices.extensions.missionplanning" .
:Component10046 rdfs:comment "" .
:Component10054 rdf:type owl:NamedIndividual .
:Component10054 rdf:type sao:Component .
:Component10054 rdfs:label "nservices.instances.areamapping" .
:Component10054 rdfs:comment "" .
:Component10045 rdf:type owl:NamedIndividual .
:Component10045 rdf:type sao:Component .
:Component10045 rdfs:label "nservices.missionplanning" .
:Component10045 rdfs:comment "" .
:Component10043 rdf:type owl:NamedIndividual .
:Component10043 rdf:type sao:Component .
:Component10043 rdfs:label "nui.vaadin.activeflights" .
:Component10043 rdfs:comment "" .
:Component10049 rdf:type owl:NamedIndividual .
:Component10049 rdf:type sao:Component .
:Component10049 rdfs:label "nui.vaadin.areamapping" .
:Component10049 rdfs:comment "" .
:Component10040 rdf:type owl:NamedIndividual .
:Component10040 rdf:type sao:Component .
:Component10040 rdfs:label "nui.vaadin.flightroutes" .
:Component10040 rdfs:comment "" .
:Component10044 rdf:type owl:NamedIndividual .
:Component10044 rdf:type sao:Component .
:Component10044 rdfs:label "nui.vaadin.start" .
:Component10044 rdfs:comment "" .
```
