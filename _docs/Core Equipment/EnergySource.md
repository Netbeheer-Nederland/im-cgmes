# EnergySource


_A generic equivalent for an energy supplier on a transmission or distribution voltage level._





**URI**: [cim:EnergySource](http://iec.ch/TC57/CIM100#EnergySource)<br />
**Type**: Class




```mermaid
 classDiagram
    class EnergySource
      EnergyConnection <|-- EnergySource
      
      EnergySource : Equipment.aggregate
        
      EnergySource : ConductingEquipment.BaseVoltage
        
          EnergySource --> BaseVoltage : ConductingEquipment.BaseVoltage
        
      EnergySource : IdentifiedObject.description
        
      EnergySource : IdentifiedObject.energyIdentCodeEic
        
      EnergySource : EnergySource.EnergySchedulingType
        
          EnergySource --> EnergySchedulingType : EnergySource.EnergySchedulingType
        
      EnergySource : Equipment.EquipmentContainer
        
          EnergySource --> EquipmentContainer : Equipment.EquipmentContainer
        
      EnergySource : IdentifiedObject.mRID
        
      EnergySource : IdentifiedObject.name
        
      EnergySource : EnergySource.nominalVoltage
        
          EnergySource --> Voltage : EnergySource.nominalVoltage
        
      EnergySource : Equipment.normallyInService
        
      EnergySource : Equipment.OperationalLimitSet
        
          EnergySource --> OperationalLimitSet : Equipment.OperationalLimitSet
        
      EnergySource : EnergySource.pMax
        
          EnergySource --> ActivePower : EnergySource.pMax
        
      EnergySource : EnergySource.pMin
        
          EnergySource --> ActivePower : EnergySource.pMin
        
      EnergySource : IdentifiedObject.shortName
        
      EnergySource : ConductingEquipment.Terminals
        
          EnergySource --> Terminal : ConductingEquipment.Terminals
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * **EnergySource**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| EnergySchedulingType | [cim:EnergySource.EnergySchedulingType](http://iec.ch/TC57/CIM100#EnergySource.EnergySchedulingType) | 0..1 <br />  [EnergySchedulingType](EnergySchedulingType.md)  | Energy Scheduling Type of an Energy Source | direct |
| nominalVoltage | [cim:EnergySource.nominalVoltage](http://iec.ch/TC57/CIM100#EnergySource.nominalVoltage) | 0..1 <br />  [Voltage](Voltage.md)  | Phase-to-phase nominal voltage | direct |
| pMin | [cim:EnergySource.pMin](http://iec.ch/TC57/CIM100#EnergySource.pMin) | 0..1 <br />  [ActivePower](ActivePower.md)  | This is the minimum active power that can be produced by the source | direct |
| pMax | [cim:EnergySource.pMax](http://iec.ch/TC57/CIM100#EnergySource.pMax) | 0..1 <br />  [ActivePower](ActivePower.md)  | This is the maximum active power that can be produced by the source | direct |
| BaseVoltage | [cim:ConductingEquipment.BaseVoltage](http://iec.ch/TC57/CIM100#ConductingEquipment.BaseVoltage) | 0..1 <br />  [BaseVoltage](BaseVoltage.md)  | Base voltage of this conducting equipment | [ConductingEquipment](ConductingEquipment.md) |
| Terminals | [cim:ConductingEquipment.Terminals](http://iec.ch/TC57/CIM100#ConductingEquipment.Terminals) | 0..* <br />  [Terminal](Terminal.md)  | Conducting equipment have terminals that may be connected to other conducting... | [ConductingEquipment](ConductingEquipment.md) |
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
| [EnergySchedulingType](EnergySchedulingType.md) | EnergySource | range | [EnergySource](EnergySource.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:EnergySource |
| native | this:EnergySource |




