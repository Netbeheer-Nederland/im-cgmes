# NonlinearShuntCompensatorPoint


_A non linear shunt compensator bank or section admittance value. The number of NonlinearShuntCompenstorPoint instances associated with a NonlinearShuntCompensator shall be equal to ShuntCompensator.maximumSections. ShuntCompensator.sections shall only be set to one of the NonlinearShuntCompenstorPoint.sectionNumber. There is no interpolation between NonlinearShuntCompenstorPoint-s._





**URI**: [cim:NonlinearShuntCompensatorPoint](http://iec.ch/TC57/CIM100#NonlinearShuntCompensatorPoint)<br />
**Type**: Class




```mermaid
 classDiagram
    class NonlinearShuntCompensatorPoint
      NonlinearShuntCompensatorPoint : NonlinearShuntCompensatorPoint.b
        
          NonlinearShuntCompensatorPoint --> Susceptance : NonlinearShuntCompensatorPoint.b
        
      NonlinearShuntCompensatorPoint : NonlinearShuntCompensatorPoint.g
        
          NonlinearShuntCompensatorPoint --> Conductance : NonlinearShuntCompensatorPoint.g
        
      NonlinearShuntCompensatorPoint : NonlinearShuntCompensatorPoint.NonlinearShuntCompensator
        
          NonlinearShuntCompensatorPoint --> NonlinearShuntCompensator : NonlinearShuntCompensatorPoint.NonlinearShuntCompensator
        
      NonlinearShuntCompensatorPoint : NonlinearShuntCompensatorPoint.sectionNumber
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| NonlinearShuntCompensator | [cim:NonlinearShuntCompensatorPoint.NonlinearShuntCompensator](http://iec.ch/TC57/CIM100#NonlinearShuntCompensatorPoint.NonlinearShuntCompensator) | 1..1 <br />  [NonlinearShuntCompensator](NonlinearShuntCompensator.md)  | Non-linear shunt compensator owning this point | direct |
| b | [cim:NonlinearShuntCompensatorPoint.b](http://iec.ch/TC57/CIM100#NonlinearShuntCompensatorPoint.b) | 1..1 <br />  [Susceptance](Susceptance.md)  | Positive sequence shunt (charging) susceptance per section | direct |
| g | [cim:NonlinearShuntCompensatorPoint.g](http://iec.ch/TC57/CIM100#NonlinearShuntCompensatorPoint.g) | 1..1 <br />  [Conductance](Conductance.md)  | Positive sequence shunt (charging) conductance per section | direct |
| sectionNumber | [cim:NonlinearShuntCompensatorPoint.sectionNumber](http://iec.ch/TC57/CIM100#NonlinearShuntCompensatorPoint.sectionNumber) | 1..1 <br />  integer  | The number of the section | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [NonlinearShuntCompensator](NonlinearShuntCompensator.md) | NonlinearShuntCompensatorPoints | range | [NonlinearShuntCompensatorPoint](NonlinearShuntCompensatorPoint.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:NonlinearShuntCompensatorPoint |
| native | this:NonlinearShuntCompensatorPoint |




