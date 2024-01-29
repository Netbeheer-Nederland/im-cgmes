# ConductingEquipment


_The parts of the AC power system that are designed to carry current or that are conductively connected through terminals._





**URI**: [cim:ConductingEquipment](http://iec.ch/TC57/CIM100#ConductingEquipment)<br />
**Type**: Class




```mermaid
 classDiagram
    class ConductingEquipment
      Equipment <|-- ConductingEquipment
      

      ConductingEquipment <|-- ACDCConverter
      ConductingEquipment <|-- Clamp
      ConductingEquipment <|-- Conductor
      ConductingEquipment <|-- Connector
      ConductingEquipment <|-- EarthFaultCompensator
      ConductingEquipment <|-- EnergyConnection
      ConductingEquipment <|-- EquivalentEquipment
      ConductingEquipment <|-- Ground
      ConductingEquipment <|-- PowerTransformer
      ConductingEquipment <|-- SeriesCompensator
      ConductingEquipment <|-- Switch
      
      
      ConductingEquipment : Equipment.aggregate
        
      ConductingEquipment : ConductingEquipment.BaseVoltage
        
          ConductingEquipment --> BaseVoltage : ConductingEquipment.BaseVoltage
        
      ConductingEquipment : IdentifiedObject.description
        
      ConductingEquipment : IdentifiedObject.energyIdentCodeEic
        
      ConductingEquipment : Equipment.EquipmentContainer
        
          ConductingEquipment --> EquipmentContainer : Equipment.EquipmentContainer
        
      ConductingEquipment : IdentifiedObject.mRID
        
      ConductingEquipment : IdentifiedObject.name
        
      ConductingEquipment : Equipment.normallyInService
        
      ConductingEquipment : Equipment.OperationalLimitSet
        
          ConductingEquipment --> OperationalLimitSet : Equipment.OperationalLimitSet
        
      ConductingEquipment : IdentifiedObject.shortName
        
      ConductingEquipment : ConductingEquipment.Terminals
        
          ConductingEquipment --> Terminal : ConductingEquipment.Terminals
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * **ConductingEquipment**
                * [ACDCConverter](ACDCConverter.md)
                * [Clamp](Clamp.md)
                * [Conductor](Conductor.md)
                * [Connector](Connector.md)
                * [EarthFaultCompensator](EarthFaultCompensator.md)
                * [EnergyConnection](EnergyConnection.md)
                * [EquivalentEquipment](EquivalentEquipment.md)
                * [Ground](Ground.md)
                * [PowerTransformer](PowerTransformer.md)
                * [SeriesCompensator](SeriesCompensator.md)
                * [Switch](Switch.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| BaseVoltage | [cim:ConductingEquipment.BaseVoltage](http://iec.ch/TC57/CIM100#ConductingEquipment.BaseVoltage) | 0..1 <br />  [BaseVoltage](BaseVoltage.md)  | Base voltage of this conducting equipment | direct |
| Terminals | [cim:ConductingEquipment.Terminals](http://iec.ch/TC57/CIM100#ConductingEquipment.Terminals) | 0..* <br />  [Terminal](Terminal.md)  | Conducting equipment have terminals that may be connected to other conducting... | direct |
| aggregate | [cim:Equipment.aggregate](http://iec.ch/TC57/CIM100#Equipment.aggregate) | 0..1 <br />  boolean  | The aggregate flag provides an alternative way of representing an aggregated ... | [Equipment](Equipment.md) |
| normallyInService | [cim:Equipment.normallyInService](http://iec.ch/TC57/CIM100#Equipment.normallyInService) | 0..1 <br />  boolean  | Specifies the availability of the equipment under normal operating conditions | [Equipment](Equipment.md) |
| EquipmentContainer | [cim:Equipment.EquipmentContainer](http://iec.ch/TC57/CIM100#Equipment.EquipmentContainer) | 0..1 <br />  [EquipmentContainer](EquipmentContainer.md)  | Container of this equipment | [Equipment](Equipment.md) |
| OperationalLimitSet | [cim:Equipment.OperationalLimitSet](http://iec.ch/TC57/CIM100#Equipment.OperationalLimitSet) | 0..* <br />  [OperationalLimitSet](OperationalLimitSet.md)  | The operational limit sets associated with this equipment | [Equipment](Equipment.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [BaseVoltage](BaseVoltage.md) | ConductingEquipment | range | [ConductingEquipment](ConductingEquipment.md) |
| [Terminal](Terminal.md) | ConductingEquipment | range | [ConductingEquipment](ConductingEquipment.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ConductingEquipment |
| native | this:ConductingEquipment |




