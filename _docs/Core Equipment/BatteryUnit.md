# BatteryUnit


_An electrochemical energy storage device._





**URI**: [cim:BatteryUnit](http://iec.ch/TC57/CIM100#BatteryUnit)<br />
**Type**: Class




```mermaid
 classDiagram
    class BatteryUnit
    click BatteryUnit href "../BatteryUnit"
      PowerElectronicsUnit <|-- BatteryUnit
        click PowerElectronicsUnit href "../PowerElectronicsUnit"
      
      BatteryUnit : Equipment.aggregate
        
      BatteryUnit : IdentifiedObject.description
        
      BatteryUnit : IdentifiedObject.energyIdentCodeEic
        
      BatteryUnit : Equipment.EquipmentContainer
        
          BatteryUnit --> EquipmentContainer : Equipment.EquipmentContainer
          click EquipmentContainer href "../EquipmentContainer"
        
      BatteryUnit : PowerElectronicsUnit.maxP
        
          BatteryUnit --> ActivePower : PowerElectronicsUnit.maxP
          click ActivePower href "../ActivePower"
        
      BatteryUnit : PowerElectronicsUnit.minP
        
          BatteryUnit --> ActivePower : PowerElectronicsUnit.minP
          click ActivePower href "../ActivePower"
        
      BatteryUnit : IdentifiedObject.mRID
        
      BatteryUnit : IdentifiedObject.name
        
      BatteryUnit : Equipment.normallyInService
        
      BatteryUnit : Equipment.OperationalLimitSet
        
          BatteryUnit --> OperationalLimitSet : Equipment.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      BatteryUnit : PowerElectronicsUnit.PowerElectronicsConnection
        
          BatteryUnit --> PowerElectronicsConnection : PowerElectronicsUnit.PowerElectronicsConnection
          click PowerElectronicsConnection href "../PowerElectronicsConnection"
        
      BatteryUnit : BatteryUnit.ratedE
        
          BatteryUnit --> RealEnergy : BatteryUnit.ratedE
          click RealEnergy href "../RealEnergy"
        
      BatteryUnit : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [PowerElectronicsUnit](PowerElectronicsUnit.md)
                * **BatteryUnit**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ratedE | [cim:BatteryUnit.ratedE](http://iec.ch/TC57/CIM100#BatteryUnit.ratedE) | 1 <br />  [RealEnergy](RealEnergy.md)  | Full energy storage capacity of the battery | direct |
| PowerElectronicsConnection | [cim:PowerElectronicsUnit.PowerElectronicsConnection](http://iec.ch/TC57/CIM100#PowerElectronicsUnit.PowerElectronicsConnection) | 1 <br />  [PowerElectronicsConnection](PowerElectronicsConnection.md)  | A power electronics unit has a connection to the AC network | [PowerElectronicsUnit](PowerElectronicsUnit.md) |
| maxP | [cim:PowerElectronicsUnit.maxP](http://iec.ch/TC57/CIM100#PowerElectronicsUnit.maxP) | 0..1 <br />  [ActivePower](ActivePower.md)  | Maximum active power limit | [PowerElectronicsUnit](PowerElectronicsUnit.md) |
| minP | [cim:PowerElectronicsUnit.minP](http://iec.ch/TC57/CIM100#PowerElectronicsUnit.minP) | 0..1 <br />  [ActivePower](ActivePower.md)  | Minimum active power limit | [PowerElectronicsUnit](PowerElectronicsUnit.md) |
| aggregate | [cim:Equipment.aggregate](http://iec.ch/TC57/CIM100#Equipment.aggregate) | 0..1 <br />  boolean  | The aggregate flag provides an alternative way of representing an aggregated ... | [Equipment](Equipment.md) |
| normallyInService | [cim:Equipment.normallyInService](http://iec.ch/TC57/CIM100#Equipment.normallyInService) | 0..1 <br />  boolean  | Specifies the availability of the equipment under normal operating conditions | [Equipment](Equipment.md) |
| EquipmentContainer | [cim:Equipment.EquipmentContainer](http://iec.ch/TC57/CIM100#Equipment.EquipmentContainer) | 0..1 <br />  [EquipmentContainer](EquipmentContainer.md)  | Container of this equipment | [Equipment](Equipment.md) |
| OperationalLimitSet | [cim:Equipment.OperationalLimitSet](http://iec.ch/TC57/CIM100#Equipment.OperationalLimitSet) | * <br />  [OperationalLimitSet](OperationalLimitSet.md)  | The operational limit sets associated with this equipment | [Equipment](Equipment.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:BatteryUnit |
| native | this:BatteryUnit |




