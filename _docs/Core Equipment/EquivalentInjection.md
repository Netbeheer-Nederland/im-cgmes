# EquivalentInjection


_This class represents equivalent injections (generation or load).  Voltage regulation is allowed only at the point of connection._





**URI**: [cim:EquivalentInjection](http://iec.ch/TC57/CIM100#EquivalentInjection)<br />
**Type**: Class




```mermaid
 classDiagram
    class EquivalentInjection
    click EquivalentInjection href "../EquivalentInjection"
      EquivalentEquipment <|-- EquivalentInjection
        click EquivalentEquipment href "../EquivalentEquipment"
      
      EquivalentInjection : Equipment.aggregate
        
      EquivalentInjection : ConductingEquipment.BaseVoltage
        
          EquivalentInjection --> BaseVoltage : ConductingEquipment.BaseVoltage
          click BaseVoltage href "../BaseVoltage"
        
      EquivalentInjection : IdentifiedObject.description
        
      EquivalentInjection : IdentifiedObject.energyIdentCodeEic
        
      EquivalentInjection : Equipment.EquipmentContainer
        
          EquivalentInjection --> EquipmentContainer : Equipment.EquipmentContainer
          click EquipmentContainer href "../EquipmentContainer"
        
      EquivalentInjection : EquivalentEquipment.EquivalentNetwork
        
          EquivalentInjection --> EquivalentNetwork : EquivalentEquipment.EquivalentNetwork
          click EquivalentNetwork href "../EquivalentNetwork"
        
      EquivalentInjection : EquivalentInjection.maxP
        
          EquivalentInjection --> ActivePower : EquivalentInjection.maxP
          click ActivePower href "../ActivePower"
        
      EquivalentInjection : EquivalentInjection.maxQ
        
          EquivalentInjection --> ReactivePower : EquivalentInjection.maxQ
          click ReactivePower href "../ReactivePower"
        
      EquivalentInjection : EquivalentInjection.minP
        
          EquivalentInjection --> ActivePower : EquivalentInjection.minP
          click ActivePower href "../ActivePower"
        
      EquivalentInjection : EquivalentInjection.minQ
        
          EquivalentInjection --> ReactivePower : EquivalentInjection.minQ
          click ReactivePower href "../ReactivePower"
        
      EquivalentInjection : IdentifiedObject.mRID
        
      EquivalentInjection : IdentifiedObject.name
        
      EquivalentInjection : Equipment.normallyInService
        
      EquivalentInjection : Equipment.OperationalLimitSet
        
          EquivalentInjection --> OperationalLimitSet : Equipment.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      EquivalentInjection : EquivalentInjection.ReactiveCapabilityCurve
        
          EquivalentInjection --> ReactiveCapabilityCurve : EquivalentInjection.ReactiveCapabilityCurve
          click ReactiveCapabilityCurve href "../ReactiveCapabilityCurve"
        
      EquivalentInjection : EquivalentInjection.regulationCapability
        
      EquivalentInjection : IdentifiedObject.shortName
        
      EquivalentInjection : ConductingEquipment.Terminals
        
          EquivalentInjection --> Terminal : ConductingEquipment.Terminals
          click Terminal href "../Terminal"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EquivalentEquipment](EquivalentEquipment.md)
                    * **EquivalentInjection**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| maxP | [cim:EquivalentInjection.maxP](http://iec.ch/TC57/CIM100#EquivalentInjection.maxP) | 0..1 <br />  [ActivePower](ActivePower.md)  | Maximum active power of the injection | direct |
| maxQ | [cim:EquivalentInjection.maxQ](http://iec.ch/TC57/CIM100#EquivalentInjection.maxQ) | 0..1 <br />  [ReactivePower](ReactivePower.md)  | Maximum reactive power of the injection | direct |
| minP | [cim:EquivalentInjection.minP](http://iec.ch/TC57/CIM100#EquivalentInjection.minP) | 0..1 <br />  [ActivePower](ActivePower.md)  | Minimum active power of the injection | direct |
| minQ | [cim:EquivalentInjection.minQ](http://iec.ch/TC57/CIM100#EquivalentInjection.minQ) | 0..1 <br />  [ReactivePower](ReactivePower.md)  | Minimum reactive power of the injection | direct |
| regulationCapability | [cim:EquivalentInjection.regulationCapability](http://iec.ch/TC57/CIM100#EquivalentInjection.regulationCapability) | 1 <br />  boolean  | Specifies whether or not the EquivalentInjection has the capability to regula... | direct |
| ReactiveCapabilityCurve | [cim:EquivalentInjection.ReactiveCapabilityCurve](http://iec.ch/TC57/CIM100#EquivalentInjection.ReactiveCapabilityCurve) | 0..1 <br />  [ReactiveCapabilityCurve](ReactiveCapabilityCurve.md)  | The reactive capability curve used by this equivalent injection | direct |
| EquivalentNetwork | [cim:EquivalentEquipment.EquivalentNetwork](http://iec.ch/TC57/CIM100#EquivalentEquipment.EquivalentNetwork) | 0..1 <br />  [EquivalentNetwork](EquivalentNetwork.md)  | The equivalent where the reduced model belongs | [EquivalentEquipment](EquivalentEquipment.md) |
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
| [ReactiveCapabilityCurve](ReactiveCapabilityCurve.md) | EquivalentInjection | range | [EquivalentInjection](EquivalentInjection.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:EquivalentInjection |
| native | this:EquivalentInjection |




