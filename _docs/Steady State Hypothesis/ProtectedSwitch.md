# ProtectedSwitch


_A ProtectedSwitch is a switching device that can be operated by ProtectionEquipment._





**URI**: [cim:ProtectedSwitch](http://iec.ch/TC57/CIM100#ProtectedSwitch)<br />
**Type**: Class




```mermaid
 classDiagram
    class ProtectedSwitch
      Switch <|-- ProtectedSwitch
      

      ProtectedSwitch <|-- Breaker
      ProtectedSwitch <|-- LoadBreakSwitch
      
      
      ProtectedSwitch : Equipment.inService
        
      ProtectedSwitch : Switch.locked
        
      ProtectedSwitch : IdentifiedObject.mRID
        
      ProtectedSwitch : Switch.open
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [Switch](Switch.md)
                    * **ProtectedSwitch**
                        * [Breaker](Breaker.md)
                        * [LoadBreakSwitch](LoadBreakSwitch.md)



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
| self | cim:ProtectedSwitch |
| native | this:ProtectedSwitch |




