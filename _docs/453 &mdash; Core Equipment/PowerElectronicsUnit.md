# PowerElectronicsUnit


_A generating unit or battery or aggregation that connects to the AC network using power electronics rather than rotating machines._





**URI**: [cim:PowerElectronicsUnit](http://iec.ch/TC57/CIM100#PowerElectronicsUnit)<br />
**Type**: Class




```mermaid
 classDiagram
    class PowerElectronicsUnit
      Equipment <|-- PowerElectronicsUnit
      

      PowerElectronicsUnit <|-- BatteryUnit
      PowerElectronicsUnit <|-- PhotoVoltaicUnit
      PowerElectronicsUnit <|-- PowerElectronicsWindUnit
      
      
      PowerElectronicsUnit : Equipment.aggregate
        
      PowerElectronicsUnit : IdentifiedObject.description
        
      PowerElectronicsUnit : IdentifiedObject.energyIdentCodeEic
        
      PowerElectronicsUnit : Equipment.EquipmentContainer
        
          PowerElectronicsUnit --> EquipmentContainer : Equipment.EquipmentContainer
        
      PowerElectronicsUnit : PowerElectronicsUnit.maxP
        
          PowerElectronicsUnit --> ActivePower : PowerElectronicsUnit.maxP
        
      PowerElectronicsUnit : PowerElectronicsUnit.minP
        
          PowerElectronicsUnit --> ActivePower : PowerElectronicsUnit.minP
        
      PowerElectronicsUnit : IdentifiedObject.mRID
        
      PowerElectronicsUnit : IdentifiedObject.name
        
      PowerElectronicsUnit : Equipment.normallyInService
        
      PowerElectronicsUnit : Equipment.OperationalLimitSet
        
          PowerElectronicsUnit --> OperationalLimitSet : Equipment.OperationalLimitSet
        
      PowerElectronicsUnit : PowerElectronicsUnit.PowerElectronicsConnection
        
          PowerElectronicsUnit --> PowerElectronicsConnection : PowerElectronicsUnit.PowerElectronicsConnection
        
      PowerElectronicsUnit : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * **PowerElectronicsUnit**
                * [BatteryUnit](BatteryUnit.md)
                * [PhotoVoltaicUnit](PhotoVoltaicUnit.md)
                * [PowerElectronicsWindUnit](PowerElectronicsWindUnit.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| PowerElectronicsConnection | [cim:PowerElectronicsUnit.PowerElectronicsConnection](http://iec.ch/TC57/CIM100#PowerElectronicsUnit.PowerElectronicsConnection) | 1..1 <br />  [PowerElectronicsConnection](PowerElectronicsConnection.md)  | A power electronics unit has a connection to the AC network | direct |
| maxP | [cim:PowerElectronicsUnit.maxP](http://iec.ch/TC57/CIM100#PowerElectronicsUnit.maxP) | 0..1 <br />  [ActivePower](ActivePower.md)  | Maximum active power limit | direct |
| minP | [cim:PowerElectronicsUnit.minP](http://iec.ch/TC57/CIM100#PowerElectronicsUnit.minP) | 0..1 <br />  [ActivePower](ActivePower.md)  | Minimum active power limit | direct |
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
| [PowerElectronicsConnection](PowerElectronicsConnection.md) | PowerElectronicsUnit | range | [PowerElectronicsUnit](PowerElectronicsUnit.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:PowerElectronicsUnit |
| native | this:PowerElectronicsUnit |




