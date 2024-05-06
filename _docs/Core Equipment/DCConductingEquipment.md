# DCConductingEquipment


_The parts of the DC power system that are designed to carry current or that are conductively connected through DC terminals._





**URI**: [cim:DCConductingEquipment](http://iec.ch/TC57/CIM100#DCConductingEquipment)<br />
**Type**: Class




```mermaid
 classDiagram
    class DCConductingEquipment
    click DCConductingEquipment href "../DCConductingEquipment"
      Equipment <|-- DCConductingEquipment
        click Equipment href "../Equipment"
      

      DCConductingEquipment <|-- DCBusbar
        click DCBusbar href "../DCBusbar"
      DCConductingEquipment <|-- DCChopper
        click DCChopper href "../DCChopper"
      DCConductingEquipment <|-- DCGround
        click DCGround href "../DCGround"
      DCConductingEquipment <|-- DCLineSegment
        click DCLineSegment href "../DCLineSegment"
      DCConductingEquipment <|-- DCSeriesDevice
        click DCSeriesDevice href "../DCSeriesDevice"
      DCConductingEquipment <|-- DCShunt
        click DCShunt href "../DCShunt"
      DCConductingEquipment <|-- DCSwitch
        click DCSwitch href "../DCSwitch"
      
      
      DCConductingEquipment : Equipment.aggregate
        
      DCConductingEquipment : DCConductingEquipment.DCTerminals
        
          DCConductingEquipment --> DCTerminal : DCConductingEquipment.DCTerminals
          click DCTerminal href "../DCTerminal"
        
      DCConductingEquipment : IdentifiedObject.description
        
      DCConductingEquipment : IdentifiedObject.energyIdentCodeEic
        
      DCConductingEquipment : Equipment.EquipmentContainer
        
          DCConductingEquipment --> EquipmentContainer : Equipment.EquipmentContainer
          click EquipmentContainer href "../EquipmentContainer"
        
      DCConductingEquipment : IdentifiedObject.mRID
        
      DCConductingEquipment : IdentifiedObject.name
        
      DCConductingEquipment : Equipment.normallyInService
        
      DCConductingEquipment : Equipment.OperationalLimitSet
        
          DCConductingEquipment --> OperationalLimitSet : Equipment.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      DCConductingEquipment : DCConductingEquipment.ratedUdc
        
          DCConductingEquipment --> Voltage : DCConductingEquipment.ratedUdc
          click Voltage href "../Voltage"
        
      DCConductingEquipment : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * **DCConductingEquipment**
                * [DCBusbar](DCBusbar.md)
                * [DCChopper](DCChopper.md)
                * [DCGround](DCGround.md)
                * [DCLineSegment](DCLineSegment.md)
                * [DCSeriesDevice](DCSeriesDevice.md)
                * [DCShunt](DCShunt.md)
                * [DCSwitch](DCSwitch.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ratedUdc | [cim:DCConductingEquipment.ratedUdc](http://iec.ch/TC57/CIM100#DCConductingEquipment.ratedUdc) | 1 <br />  [Voltage](Voltage.md)  | Rated DC device voltage | direct |
| DCTerminals | [cim:DCConductingEquipment.DCTerminals](http://iec.ch/TC57/CIM100#DCConductingEquipment.DCTerminals) | * <br />  [DCTerminal](DCTerminal.md)  | A DC conducting equipment has DC terminals | direct |
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
| [DCTerminal](DCTerminal.md) | DCConductingEquipment | range | [DCConductingEquipment](DCConductingEquipment.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:DCConductingEquipment |
| native | this:DCConductingEquipment |




