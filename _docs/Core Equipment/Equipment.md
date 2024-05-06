# Equipment


_The parts of a power system that are physical devices, electronic or mechanical._





**URI**: [cim:Equipment](http://iec.ch/TC57/CIM100#Equipment)<br />
**Type**: Class




```mermaid
 classDiagram
    class Equipment
    click Equipment href "../Equipment"
      PowerSystemResource <|-- Equipment
        click PowerSystemResource href "../PowerSystemResource"
      

      Equipment <|-- AuxiliaryEquipment
        click AuxiliaryEquipment href "../AuxiliaryEquipment"
      Equipment <|-- ConductingEquipment
        click ConductingEquipment href "../ConductingEquipment"
      Equipment <|-- DCConductingEquipment
        click DCConductingEquipment href "../DCConductingEquipment"
      Equipment <|-- GeneratingUnit
        click GeneratingUnit href "../GeneratingUnit"
      Equipment <|-- HydroPump
        click HydroPump href "../HydroPump"
      Equipment <|-- PowerElectronicsUnit
        click PowerElectronicsUnit href "../PowerElectronicsUnit"
      
      
      Equipment : Equipment.aggregate
        
      Equipment : IdentifiedObject.description
        
      Equipment : IdentifiedObject.energyIdentCodeEic
        
      Equipment : Equipment.EquipmentContainer
        
          Equipment --> EquipmentContainer : Equipment.EquipmentContainer
          click EquipmentContainer href "../EquipmentContainer"
        
      Equipment : IdentifiedObject.mRID
        
      Equipment : IdentifiedObject.name
        
      Equipment : Equipment.normallyInService
        
      Equipment : Equipment.OperationalLimitSet
        
          Equipment --> OperationalLimitSet : Equipment.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      Equipment : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * **Equipment**
            * [AuxiliaryEquipment](AuxiliaryEquipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
            * [DCConductingEquipment](DCConductingEquipment.md)
            * [GeneratingUnit](GeneratingUnit.md)
            * [HydroPump](HydroPump.md)
            * [PowerElectronicsUnit](PowerElectronicsUnit.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| aggregate | [cim:Equipment.aggregate](http://iec.ch/TC57/CIM100#Equipment.aggregate) | 0..1 <br />  boolean  | The aggregate flag provides an alternative way of representing an aggregated ... | direct |
| normallyInService | [cim:Equipment.normallyInService](http://iec.ch/TC57/CIM100#Equipment.normallyInService) | 0..1 <br />  boolean  | Specifies the availability of the equipment under normal operating conditions | direct |
| EquipmentContainer | [cim:Equipment.EquipmentContainer](http://iec.ch/TC57/CIM100#Equipment.EquipmentContainer) | 0..1 <br />  [EquipmentContainer](EquipmentContainer.md)  | Container of this equipment | direct |
| OperationalLimitSet | [cim:Equipment.OperationalLimitSet](http://iec.ch/TC57/CIM100#Equipment.OperationalLimitSet) | * <br />  [OperationalLimitSet](OperationalLimitSet.md)  | The operational limit sets associated with this equipment | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [Bay](Bay.md) | Equipments | range | [Equipment](Equipment.md) |
| [DCConverterUnit](DCConverterUnit.md) | Equipments | range | [Equipment](Equipment.md) |
| [DCEquipmentContainer](DCEquipmentContainer.md) | Equipments | range | [Equipment](Equipment.md) |
| [DCLine](DCLine.md) | Equipments | range | [Equipment](Equipment.md) |
| [EquipmentContainer](EquipmentContainer.md) | Equipments | range | [Equipment](Equipment.md) |
| [Line](Line.md) | Equipments | range | [Equipment](Equipment.md) |
| [OperationalLimitSet](OperationalLimitSet.md) | Equipment | range | [Equipment](Equipment.md) |
| [Substation](Substation.md) | Equipments | range | [Equipment](Equipment.md) |
| [VoltageLevel](VoltageLevel.md) | Equipments | range | [Equipment](Equipment.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Equipment |
| native | this:Equipment |




