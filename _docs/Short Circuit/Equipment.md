# Equipment


_The parts of a power system that are physical devices, electronic or mechanical._





**URI**: [cim:Equipment](http://iec.ch/TC57/CIM100#Equipment)<br />
**Type**: Class




```mermaid
 classDiagram
    class Equipment
      PowerSystemResource <|-- Equipment
      

      Equipment <|-- ConductingEquipment
      
      
      Equipment : IdentifiedObject.mRID
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * **Equipment**
            * [ConductingEquipment](ConductingEquipment.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/ShortCircuit-EU#Package_ShortCircuitProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Equipment |
| native | this:Equipment |




