# EquivalentEquipment


_The class represents equivalent objects that are the result of a network reduction. The class is the base for equivalent objects of different types._





**URI**: [cim:EquivalentEquipment](http://iec.ch/TC57/CIM100#EquivalentEquipment)<br />
**Type**: Class




```mermaid
 classDiagram
    class EquivalentEquipment
    click EquivalentEquipment href "../EquivalentEquipment"
      ConductingEquipment <|-- EquivalentEquipment
        click ConductingEquipment href "../ConductingEquipment"
      

      EquivalentEquipment <|-- EquivalentBranch
        click EquivalentBranch href "../EquivalentBranch"
      EquivalentEquipment <|-- EquivalentInjection
        click EquivalentInjection href "../EquivalentInjection"
      
      
      EquivalentEquipment : IdentifiedObject.mRID
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * **EquivalentEquipment**
                    * [EquivalentBranch](EquivalentBranch.md)
                    * [EquivalentInjection](EquivalentInjection.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/ShortCircuit-EU#Package_ShortCircuitProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:EquivalentEquipment |
| native | this:EquivalentEquipment |




