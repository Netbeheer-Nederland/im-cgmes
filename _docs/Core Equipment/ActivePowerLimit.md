# ActivePowerLimit


_Limit on active power flow._





**URI**: [cim:ActivePowerLimit](http://iec.ch/TC57/CIM100#ActivePowerLimit)<br />
**Type**: Class




```mermaid
 classDiagram
    class ActivePowerLimit
    click ActivePowerLimit href "../ActivePowerLimit"
      OperationalLimit <|-- ActivePowerLimit
        click OperationalLimit href "../OperationalLimit"
      
      ActivePowerLimit : IdentifiedObject.description
        
      ActivePowerLimit : IdentifiedObject.energyIdentCodeEic
        
      ActivePowerLimit : IdentifiedObject.mRID
        
      ActivePowerLimit : IdentifiedObject.name
        
      ActivePowerLimit : ActivePowerLimit.normalValue
        
          ActivePowerLimit --> ActivePower : ActivePowerLimit.normalValue
          click ActivePower href "../ActivePower"
        
      ActivePowerLimit : OperationalLimit.OperationalLimitSet
        
          ActivePowerLimit --> OperationalLimitSet : OperationalLimit.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      ActivePowerLimit : OperationalLimit.OperationalLimitType
        
          ActivePowerLimit --> OperationalLimitType : OperationalLimit.OperationalLimitType
          click OperationalLimitType href "../OperationalLimitType"
        
      ActivePowerLimit : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [OperationalLimit](OperationalLimit.md)
        * **ActivePowerLimit**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| normalValue | [cim:ActivePowerLimit.normalValue](http://iec.ch/TC57/CIM100#ActivePowerLimit.normalValue) | 1 <br />  [ActivePower](ActivePower.md)  | The normal value of active power limit | direct |
| OperationalLimitSet | [cim:OperationalLimit.OperationalLimitSet](http://iec.ch/TC57/CIM100#OperationalLimit.OperationalLimitSet) | 1 <br />  [OperationalLimitSet](OperationalLimitSet.md)  | The limit set to which the limit values belong | [OperationalLimit](OperationalLimit.md) |
| OperationalLimitType | [cim:OperationalLimit.OperationalLimitType](http://iec.ch/TC57/CIM100#OperationalLimit.OperationalLimitType) | 1 <br />  [OperationalLimitType](OperationalLimitType.md)  | The limit type associated with this limit | [OperationalLimit](OperationalLimit.md) |
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
| self | cim:ActivePowerLimit |
| native | this:ActivePowerLimit |




