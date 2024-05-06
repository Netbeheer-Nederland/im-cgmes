# LinearShuntCompensator


_A linear shunt compensator has banks or sections with equal admittance values._





**URI**: [cim:LinearShuntCompensator](http://iec.ch/TC57/CIM100#LinearShuntCompensator)<br />
**Type**: Class




```mermaid
 classDiagram
    class LinearShuntCompensator
    click LinearShuntCompensator href "../LinearShuntCompensator"
      ShuntCompensator <|-- LinearShuntCompensator
        click ShuntCompensator href "../ShuntCompensator"
      
      LinearShuntCompensator : RegulatingCondEq.controlEnabled
        
      LinearShuntCompensator : Equipment.inService
        
      LinearShuntCompensator : IdentifiedObject.mRID
        
      LinearShuntCompensator : ShuntCompensator.sections
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * [RegulatingCondEq](RegulatingCondEq.md)
                        * [ShuntCompensator](ShuntCompensator.md)
                            * **LinearShuntCompensator**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| sections | [cim:ShuntCompensator.sections](http://iec.ch/TC57/CIM100#ShuntCompensator.sections) | 1 <br />  float  | Shunt compensator sections in use | [ShuntCompensator](ShuntCompensator.md) |
| controlEnabled | [cim:RegulatingCondEq.controlEnabled](http://iec.ch/TC57/CIM100#RegulatingCondEq.controlEnabled) | 1 <br />  boolean  | Specifies the regulation status of the equipment | [RegulatingCondEq](RegulatingCondEq.md) |
| inService | [cim:Equipment.inService](http://iec.ch/TC57/CIM100#Equipment.inService) | 1 <br />  boolean  | Specifies the availability of the equipment | [Equipment](Equipment.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:LinearShuntCompensator |
| native | this:LinearShuntCompensator |




