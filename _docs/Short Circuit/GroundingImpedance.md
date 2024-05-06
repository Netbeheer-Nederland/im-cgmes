# GroundingImpedance


_A fixed impedance device used for grounding._





**URI**: [cim:GroundingImpedance](http://iec.ch/TC57/CIM100#GroundingImpedance)<br />
**Type**: Class




```mermaid
 classDiagram
    class GroundingImpedance
    click GroundingImpedance href "../GroundingImpedance"
      EarthFaultCompensator <|-- GroundingImpedance
        click EarthFaultCompensator href "../EarthFaultCompensator"
      
      GroundingImpedance : IdentifiedObject.mRID
        
      GroundingImpedance : EarthFaultCompensator.r
        
          GroundingImpedance --> Resistance : EarthFaultCompensator.r
          click Resistance href "../Resistance"
        
      GroundingImpedance : GroundingImpedance.x
        
          GroundingImpedance --> Reactance : GroundingImpedance.x
          click Reactance href "../Reactance"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EarthFaultCompensator](EarthFaultCompensator.md)
                    * **GroundingImpedance**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| x | [cim:GroundingImpedance.x](http://iec.ch/TC57/CIM100#GroundingImpedance.x) | 1 <br />  [Reactance](Reactance.md)  | Reactance of device | direct |
| r | [cim:EarthFaultCompensator.r](http://iec.ch/TC57/CIM100#EarthFaultCompensator.r) | 0..1 <br />  [Resistance](Resistance.md)  | Nominal resistance of device | [EarthFaultCompensator](EarthFaultCompensator.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/ShortCircuit-EU#Package_ShortCircuitProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:GroundingImpedance |
| native | this:GroundingImpedance |




