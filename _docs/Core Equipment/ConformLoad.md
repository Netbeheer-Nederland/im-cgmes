# ConformLoad


_ConformLoad represent loads that follow a daily load change pattern where the pattern can be used to scale the load with a system load._





**URI**: [cim:ConformLoad](http://iec.ch/TC57/CIM100#ConformLoad)<br />
**Type**: Class




```mermaid
 classDiagram
    class ConformLoad
    click ConformLoad href "../ConformLoad"
      EnergyConsumer <|-- ConformLoad
        click EnergyConsumer href "../EnergyConsumer"
      
      ConformLoad : Equipment.aggregate
        
      ConformLoad : ConductingEquipment.BaseVoltage
        
          ConformLoad --> BaseVoltage : ConductingEquipment.BaseVoltage
          click BaseVoltage href "../BaseVoltage"
        
      ConformLoad : IdentifiedObject.description
        
      ConformLoad : IdentifiedObject.energyIdentCodeEic
        
      ConformLoad : Equipment.EquipmentContainer
        
          ConformLoad --> EquipmentContainer : Equipment.EquipmentContainer
          click EquipmentContainer href "../EquipmentContainer"
        
      ConformLoad : ConformLoad.LoadGroup
        
          ConformLoad --> ConformLoadGroup : ConformLoad.LoadGroup
          click ConformLoadGroup href "../ConformLoadGroup"
        
      ConformLoad : EnergyConsumer.LoadResponse
        
          ConformLoad --> LoadResponseCharacteristic : EnergyConsumer.LoadResponse
          click LoadResponseCharacteristic href "../LoadResponseCharacteristic"
        
      ConformLoad : IdentifiedObject.mRID
        
      ConformLoad : IdentifiedObject.name
        
      ConformLoad : Equipment.normallyInService
        
      ConformLoad : Equipment.OperationalLimitSet
        
          ConformLoad --> OperationalLimitSet : Equipment.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      ConformLoad : EnergyConsumer.pfixed
        
          ConformLoad --> ActivePower : EnergyConsumer.pfixed
          click ActivePower href "../ActivePower"
        
      ConformLoad : EnergyConsumer.pfixedPct
        
          ConformLoad --> PerCent : EnergyConsumer.pfixedPct
          click PerCent href "../PerCent"
        
      ConformLoad : EnergyConsumer.qfixed
        
          ConformLoad --> ReactivePower : EnergyConsumer.qfixed
          click ReactivePower href "../ReactivePower"
        
      ConformLoad : EnergyConsumer.qfixedPct
        
          ConformLoad --> PerCent : EnergyConsumer.qfixedPct
          click PerCent href "../PerCent"
        
      ConformLoad : IdentifiedObject.shortName
        
      ConformLoad : ConductingEquipment.Terminals
        
          ConformLoad --> Terminal : ConductingEquipment.Terminals
          click Terminal href "../Terminal"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * [EnergyConsumer](EnergyConsumer.md)
                        * **ConformLoad**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| LoadGroup | [cim:ConformLoad.LoadGroup](http://iec.ch/TC57/CIM100#ConformLoad.LoadGroup) | 1 <br />  [ConformLoadGroup](ConformLoadGroup.md)  | Group of this ConformLoad | direct |
| pfixed | [cim:EnergyConsumer.pfixed](http://iec.ch/TC57/CIM100#EnergyConsumer.pfixed) | 0..1 <br />  [ActivePower](ActivePower.md)  | Active power of the load that is a fixed quantity and does not vary as load g... | [EnergyConsumer](EnergyConsumer.md) |
| pfixedPct | [cim:EnergyConsumer.pfixedPct](http://iec.ch/TC57/CIM100#EnergyConsumer.pfixedPct) | 0..1 <br />  [PerCent](PerCent.md)  | Fixed active power as a percentage of load group fixed active power | [EnergyConsumer](EnergyConsumer.md) |
| qfixed | [cim:EnergyConsumer.qfixed](http://iec.ch/TC57/CIM100#EnergyConsumer.qfixed) | 0..1 <br />  [ReactivePower](ReactivePower.md)  | Reactive power of the load that is a fixed quantity and does not vary as load... | [EnergyConsumer](EnergyConsumer.md) |
| qfixedPct | [cim:EnergyConsumer.qfixedPct](http://iec.ch/TC57/CIM100#EnergyConsumer.qfixedPct) | 0..1 <br />  [PerCent](PerCent.md)  | Fixed reactive power as a percentage of load group fixed reactive power | [EnergyConsumer](EnergyConsumer.md) |
| LoadResponse | [cim:EnergyConsumer.LoadResponse](http://iec.ch/TC57/CIM100#EnergyConsumer.LoadResponse) | 0..1 <br />  [LoadResponseCharacteristic](LoadResponseCharacteristic.md)  | The load response characteristic of this load | [EnergyConsumer](EnergyConsumer.md) |
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





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ConformLoadGroup](ConformLoadGroup.md) | EnergyConsumers | range | [ConformLoad](ConformLoad.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ConformLoad |
| native | this:ConformLoad |




