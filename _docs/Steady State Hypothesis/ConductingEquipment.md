# ConductingEquipment


_The parts of the AC power system that are designed to carry current or that are conductively connected through terminals._





**URI**: [cim:ConductingEquipment](http://iec.ch/TC57/CIM100#ConductingEquipment)<br />
**Type**: Class




```mermaid
 classDiagram
    class ConductingEquipment
    click ConductingEquipment href "../ConductingEquipment"
      Equipment <|-- ConductingEquipment
        click Equipment href "../Equipment"
      

      ConductingEquipment <|-- ACDCConverter
        click ACDCConverter href "../ACDCConverter"
      ConductingEquipment <|-- EnergyConnection
        click EnergyConnection href "../EnergyConnection"
      ConductingEquipment <|-- EquivalentEquipment
        click EquivalentEquipment href "../EquivalentEquipment"
      ConductingEquipment <|-- Switch
        click Switch href "../Switch"
      
      
      ConductingEquipment : Equipment.inService
        
      ConductingEquipment : IdentifiedObject.mRID
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * **ConductingEquipment**
                * [ACDCConverter](ACDCConverter.md)
                * [EnergyConnection](EnergyConnection.md)
                * [EquivalentEquipment](EquivalentEquipment.md)
                * [Switch](Switch.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| inService | [cim:Equipment.inService](http://iec.ch/TC57/CIM100#Equipment.inService) | 1 <br />  boolean  | Specifies the availability of the equipment | [Equipment](Equipment.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ConductingEquipment |
| native | this:ConductingEquipment |




