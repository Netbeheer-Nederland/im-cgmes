# NonlinearShuntCompensator


_A non linear shunt compensator has bank or section admittance values that differ. The attributes g, b, g0 and b0 of the associated NonlinearShuntCompensatorPoint describe the total conductance and admittance of a NonlinearShuntCompensatorPoint at a section number specified by NonlinearShuntCompensatorPoint.sectionNumber._





**URI**: [cim:NonlinearShuntCompensator](http://iec.ch/TC57/CIM100#NonlinearShuntCompensator)<br />
**Type**: Class




```mermaid
 classDiagram
    class NonlinearShuntCompensator
      ShuntCompensator <|-- NonlinearShuntCompensator
      
      NonlinearShuntCompensator : RegulatingCondEq.controlEnabled
        
      NonlinearShuntCompensator : Equipment.inService
        
      NonlinearShuntCompensator : IdentifiedObject.mRID
        
      NonlinearShuntCompensator : ShuntCompensator.sections
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * [RegulatingCondEq](RegulatingCondEq.md)
                        * [ShuntCompensator](ShuntCompensator.md)
                            * **NonlinearShuntCompensator**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| sections | [cim:ShuntCompensator.sections](http://iec.ch/TC57/CIM100#ShuntCompensator.sections) | 1..1 <br />  float  | Shunt compensator sections in use | [ShuntCompensator](ShuntCompensator.md) |
| controlEnabled | [cim:RegulatingCondEq.controlEnabled](http://iec.ch/TC57/CIM100#RegulatingCondEq.controlEnabled) | 1..1 <br />  boolean  | Specifies the regulation status of the equipment | [RegulatingCondEq](RegulatingCondEq.md) |
| inService | [cim:Equipment.inService](http://iec.ch/TC57/CIM100#Equipment.inService) | 1..1 <br />  boolean  | Specifies the availability of the equipment | [Equipment](Equipment.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:NonlinearShuntCompensator |
| native | this:NonlinearShuntCompensator |




