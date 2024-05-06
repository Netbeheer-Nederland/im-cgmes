# ShuntCompensator


_A shunt capacitor or reactor or switchable bank of shunt capacitors or reactors. A section of a shunt compensator is an individual capacitor or reactor. A negative value for bPerSection indicates that the compensator is a reactor. ShuntCompensator is a single terminal device.  Ground is implied._





**URI**: [cim:ShuntCompensator](http://iec.ch/TC57/CIM100#ShuntCompensator)<br />
**Type**: Class




```mermaid
 classDiagram
    class ShuntCompensator
    click ShuntCompensator href "../ShuntCompensator"
      RegulatingCondEq <|-- ShuntCompensator
        click RegulatingCondEq href "../RegulatingCondEq"
      

      ShuntCompensator <|-- LinearShuntCompensator
        click LinearShuntCompensator href "../LinearShuntCompensator"
      ShuntCompensator <|-- NonlinearShuntCompensator
        click NonlinearShuntCompensator href "../NonlinearShuntCompensator"
      
      
      ShuntCompensator : RegulatingCondEq.controlEnabled
        
      ShuntCompensator : Equipment.inService
        
      ShuntCompensator : IdentifiedObject.mRID
        
      ShuntCompensator : ShuntCompensator.sections
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * [RegulatingCondEq](RegulatingCondEq.md)
                        * **ShuntCompensator**
                            * [LinearShuntCompensator](LinearShuntCompensator.md)
                            * [NonlinearShuntCompensator](NonlinearShuntCompensator.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| sections | [cim:ShuntCompensator.sections](http://iec.ch/TC57/CIM100#ShuntCompensator.sections) | 1 <br />  float  | Shunt compensator sections in use | direct |
| controlEnabled | [cim:RegulatingCondEq.controlEnabled](http://iec.ch/TC57/CIM100#RegulatingCondEq.controlEnabled) | 1 <br />  boolean  | Specifies the regulation status of the equipment | [RegulatingCondEq](RegulatingCondEq.md) |
| inService | [cim:Equipment.inService](http://iec.ch/TC57/CIM100#Equipment.inService) | 1 <br />  boolean  | Specifies the availability of the equipment | [Equipment](Equipment.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ShuntCompensator |
| native | this:ShuntCompensator |




