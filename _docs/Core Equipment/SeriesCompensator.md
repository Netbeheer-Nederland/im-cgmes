# SeriesCompensator


_A Series Compensator is a series capacitor or reactor or an AC transmission line without charging susceptance.  It is a two terminal device._





**URI**: [cim:SeriesCompensator](http://iec.ch/TC57/CIM100#SeriesCompensator)<br />
**Type**: Class




```mermaid
 classDiagram
    class SeriesCompensator
    click SeriesCompensator href "../SeriesCompensator"
      ConductingEquipment <|-- SeriesCompensator
        click ConductingEquipment href "../ConductingEquipment"
      
      SeriesCompensator : Equipment.aggregate
        
      SeriesCompensator : ConductingEquipment.BaseVoltage
        
          SeriesCompensator --> BaseVoltage : ConductingEquipment.BaseVoltage
          click BaseVoltage href "../BaseVoltage"
        
      SeriesCompensator : IdentifiedObject.description
        
      SeriesCompensator : IdentifiedObject.energyIdentCodeEic
        
      SeriesCompensator : Equipment.EquipmentContainer
        
          SeriesCompensator --> EquipmentContainer : Equipment.EquipmentContainer
          click EquipmentContainer href "../EquipmentContainer"
        
      SeriesCompensator : IdentifiedObject.mRID
        
      SeriesCompensator : IdentifiedObject.name
        
      SeriesCompensator : Equipment.normallyInService
        
      SeriesCompensator : Equipment.OperationalLimitSet
        
          SeriesCompensator --> OperationalLimitSet : Equipment.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      SeriesCompensator : SeriesCompensator.r
        
          SeriesCompensator --> Resistance : SeriesCompensator.r
          click Resistance href "../Resistance"
        
      SeriesCompensator : IdentifiedObject.shortName
        
      SeriesCompensator : ConductingEquipment.Terminals
        
          SeriesCompensator --> Terminal : ConductingEquipment.Terminals
          click Terminal href "../Terminal"
        
      SeriesCompensator : SeriesCompensator.x
        
          SeriesCompensator --> Reactance : SeriesCompensator.x
          click Reactance href "../Reactance"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * **SeriesCompensator**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| r | [cim:SeriesCompensator.r](http://iec.ch/TC57/CIM100#SeriesCompensator.r) | 1 <br />  [Resistance](Resistance.md)  | Positive sequence resistance | direct |
| x | [cim:SeriesCompensator.x](http://iec.ch/TC57/CIM100#SeriesCompensator.x) | 1 <br />  [Reactance](Reactance.md)  | Positive sequence reactance | direct |
| BaseVoltage | [cim:ConductingEquipment.BaseVoltage](http://iec.ch/TC57/CIM100#ConductingEquipment.BaseVoltage) | 0..1 <br />  [BaseVoltage](BaseVoltage.md)  | Base voltage of this conducting equipment | [ConductingEquipment](ConductingEquipment.md) |
| Terminals | [cim:ConductingEquipment.Terminals](http://iec.ch/TC57/CIM100#ConductingEquipment.Terminals) | * <br />  [Terminal](Terminal.md)  | Conducting equipment have terminals that may be connected to other conducting... | [ConductingEquipment](ConductingEquipment.md) |
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
| self | cim:SeriesCompensator |
| native | this:SeriesCompensator |




