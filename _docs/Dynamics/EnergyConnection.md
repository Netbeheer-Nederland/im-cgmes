# EnergyConnection


_A connection of energy generation or consumption on the power system model._





**URI**: [cim:EnergyConnection](http://iec.ch/TC57/CIM100#EnergyConnection)<br />
**Type**: Class




```mermaid
 classDiagram
    class EnergyConnection
      ConductingEquipment <|-- EnergyConnection
      

      EnergyConnection <|-- EnergyConsumer
      EnergyConnection <|-- RegulatingCondEq
      
      
      EnergyConnection : IdentifiedObject.description
        
      EnergyConnection : IdentifiedObject.mRID
        
      EnergyConnection : IdentifiedObject.name
        
      EnergyConnection : ConductingEquipment.Terminals
        
          EnergyConnection --> Terminal : ConductingEquipment.Terminals
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * **EnergyConnection**
                    * [EnergyConsumer](EnergyConsumer.md)
                    * [RegulatingCondEq](RegulatingCondEq.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Terminals | [cim:ConductingEquipment.Terminals](http://iec.ch/TC57/CIM100#ConductingEquipment.Terminals) | 0..* <br />  [Terminal](Terminal.md)  | Conducting equipment have terminals that may be connected to other conducting... | [ConductingEquipment](ConductingEquipment.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:EnergyConnection |
| native | this:EnergyConnection |




