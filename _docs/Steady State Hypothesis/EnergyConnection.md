# EnergyConnection


_A connection of energy generation or consumption on the power system model._





**URI**: [cim:EnergyConnection](http://iec.ch/TC57/CIM100#EnergyConnection)<br />
**Type**: Class




```mermaid
 classDiagram
    class EnergyConnection
      ConductingEquipment <|-- EnergyConnection
      

      EnergyConnection <|-- EnergyConsumer
      EnergyConnection <|-- EnergySource
      EnergyConnection <|-- RegulatingCondEq
      
      
      EnergyConnection : Equipment.inService
        
      EnergyConnection : IdentifiedObject.mRID
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * **EnergyConnection**
                    * [EnergyConsumer](EnergyConsumer.md)
                    * [EnergySource](EnergySource.md)
                    * [RegulatingCondEq](RegulatingCondEq.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| inService | [cim:Equipment.inService](http://iec.ch/TC57/CIM100#Equipment.inService) | 1..1 <br />  boolean  | Specifies the availability of the equipment | [Equipment](Equipment.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:EnergyConnection |
| native | this:EnergyConnection |




