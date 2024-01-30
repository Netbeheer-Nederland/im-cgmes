# Fuse


_An overcurrent protective device with a circuit opening fusible part that is heated and severed by the passage of overcurrent through it. A fuse is considered a switching device because it breaks current._





**URI**: [cim:Fuse](http://iec.ch/TC57/CIM100#Fuse)<br />
**Type**: Class




```mermaid
 classDiagram
    class Fuse
      Switch <|-- Fuse
      
      Fuse : Equipment.inService
        
      Fuse : Switch.locked
        
      Fuse : IdentifiedObject.mRID
        
      Fuse : Switch.open
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [Switch](Switch.md)
                    * **Fuse**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| open | [cim:Switch.open](http://iec.ch/TC57/CIM100#Switch.open) | 1..1 <br />  boolean  | The attribute tells if the switch is considered open when used as input to to... | [Switch](Switch.md) |
| locked | [cim:Switch.locked](http://iec.ch/TC57/CIM100#Switch.locked) | 1..1 <br />  boolean  | If true, the switch is locked | [Switch](Switch.md) |
| inService | [cim:Equipment.inService](http://iec.ch/TC57/CIM100#Equipment.inService) | 1..1 <br />  boolean  | Specifies the availability of the equipment | [Equipment](Equipment.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Fuse |
| native | this:Fuse |




