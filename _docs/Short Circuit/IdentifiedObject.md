# IdentifiedObject


_This is a root class to provide common identification for all classes needing identification and naming attributes._





**URI**: [cim:IdentifiedObject](http://iec.ch/TC57/CIM100#IdentifiedObject)<br />
**Type**: Class




```mermaid
 classDiagram
    class IdentifiedObject
      IdentifiedObject <|-- ACDCTerminal
      IdentifiedObject <|-- MutualCoupling
      IdentifiedObject <|-- PowerSystemResource
      IdentifiedObject <|-- TransformerEnd
      
      IdentifiedObject : IdentifiedObject.mRID
        
      
```





## Inheritance
* **IdentifiedObject**
    * [ACDCTerminal](ACDCTerminal.md)
    * [MutualCoupling](MutualCoupling.md)
    * [PowerSystemResource](PowerSystemResource.md)
    * [TransformerEnd](TransformerEnd.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | direct |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/ShortCircuit-EU#Package_ShortCircuitProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:IdentifiedObject |
| native | this:IdentifiedObject |




