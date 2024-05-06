# RegulatingCondEq


_A type of conducting equipment that can regulate a quantity (i.e. voltage or flow) at a specific point in the network._





**URI**: [cim:RegulatingCondEq](http://iec.ch/TC57/CIM100#RegulatingCondEq)<br />
**Type**: Class




```mermaid
 classDiagram
    class RegulatingCondEq
    click RegulatingCondEq href "../RegulatingCondEq"
      EnergyConnection <|-- RegulatingCondEq
        click EnergyConnection href "../EnergyConnection"
      

      RegulatingCondEq <|-- ExternalNetworkInjection
        click ExternalNetworkInjection href "../ExternalNetworkInjection"
      RegulatingCondEq <|-- PowerElectronicsConnection
        click PowerElectronicsConnection href "../PowerElectronicsConnection"
      RegulatingCondEq <|-- RotatingMachine
        click RotatingMachine href "../RotatingMachine"
      RegulatingCondEq <|-- ShuntCompensator
        click ShuntCompensator href "../ShuntCompensator"
      RegulatingCondEq <|-- StaticVarCompensator
        click StaticVarCompensator href "../StaticVarCompensator"
      
      
      RegulatingCondEq : Equipment.aggregate
        
      RegulatingCondEq : ConductingEquipment.BaseVoltage
        
          RegulatingCondEq --> BaseVoltage : ConductingEquipment.BaseVoltage
          click BaseVoltage href "../BaseVoltage"
        
      RegulatingCondEq : IdentifiedObject.description
        
      RegulatingCondEq : IdentifiedObject.energyIdentCodeEic
        
      RegulatingCondEq : Equipment.EquipmentContainer
        
          RegulatingCondEq --> EquipmentContainer : Equipment.EquipmentContainer
          click EquipmentContainer href "../EquipmentContainer"
        
      RegulatingCondEq : IdentifiedObject.mRID
        
      RegulatingCondEq : IdentifiedObject.name
        
      RegulatingCondEq : Equipment.normallyInService
        
      RegulatingCondEq : Equipment.OperationalLimitSet
        
          RegulatingCondEq --> OperationalLimitSet : Equipment.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      RegulatingCondEq : RegulatingCondEq.RegulatingControl
        
          RegulatingCondEq --> RegulatingControl : RegulatingCondEq.RegulatingControl
          click RegulatingControl href "../RegulatingControl"
        
      RegulatingCondEq : IdentifiedObject.shortName
        
      RegulatingCondEq : ConductingEquipment.Terminals
        
          RegulatingCondEq --> Terminal : ConductingEquipment.Terminals
          click Terminal href "../Terminal"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EnergyConnection](EnergyConnection.md)
                    * **RegulatingCondEq**
                        * [ExternalNetworkInjection](ExternalNetworkInjection.md)
                        * [PowerElectronicsConnection](PowerElectronicsConnection.md)
                        * [RotatingMachine](RotatingMachine.md)
                        * [ShuntCompensator](ShuntCompensator.md)
                        * [StaticVarCompensator](StaticVarCompensator.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| RegulatingControl | [cim:RegulatingCondEq.RegulatingControl](http://iec.ch/TC57/CIM100#RegulatingCondEq.RegulatingControl) | 0..1 <br />  [RegulatingControl](RegulatingControl.md)  | The regulating control scheme in which this equipment participates | direct |
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
| [RegulatingControl](RegulatingControl.md) | RegulatingCondEq | range | [RegulatingCondEq](RegulatingCondEq.md) |
| [TapChangerControl](TapChangerControl.md) | RegulatingCondEq | range | [RegulatingCondEq](RegulatingCondEq.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:RegulatingCondEq |
| native | this:RegulatingCondEq |




