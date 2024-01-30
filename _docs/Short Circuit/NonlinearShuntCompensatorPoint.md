# NonlinearShuntCompensatorPoint


_A non linear shunt compensator bank or section admittance value. The number of NonlinearShuntCompenstorPoint instances associated with a NonlinearShuntCompensator shall be equal to ShuntCompensator.maximumSections. ShuntCompensator.sections shall only be set to one of the NonlinearShuntCompenstorPoint.sectionNumber. There is no interpolation between NonlinearShuntCompenstorPoint-s._





**URI**: [cim:NonlinearShuntCompensatorPoint](http://iec.ch/TC57/CIM100#NonlinearShuntCompensatorPoint)<br />
**Type**: Class




```mermaid
 classDiagram
    class NonlinearShuntCompensatorPoint
      NonlinearShuntCompensatorPoint : NonlinearShuntCompensatorPoint.b0
        
          NonlinearShuntCompensatorPoint --> Susceptance : NonlinearShuntCompensatorPoint.b0
        
      NonlinearShuntCompensatorPoint : NonlinearShuntCompensatorPoint.g0
        
          NonlinearShuntCompensatorPoint --> Conductance : NonlinearShuntCompensatorPoint.g0
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| b0 | [cim:NonlinearShuntCompensatorPoint.b0](http://iec.ch/TC57/CIM100#NonlinearShuntCompensatorPoint.b0) | 1..1 <br />  [Susceptance](Susceptance.md)  | Zero sequence shunt (charging) susceptance per section | direct |
| g0 | [cim:NonlinearShuntCompensatorPoint.g0](http://iec.ch/TC57/CIM100#NonlinearShuntCompensatorPoint.g0) | 1..1 <br />  [Conductance](Conductance.md)  | Zero sequence shunt (charging) conductance per section | direct |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/ShortCircuit-EU#Package_ShortCircuitProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:NonlinearShuntCompensatorPoint |
| native | this:NonlinearShuntCompensatorPoint |




