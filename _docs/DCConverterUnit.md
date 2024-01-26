# DCConverterUnit


_Indivisible operative unit comprising all equipment between the point of common coupling on the AC side and the point of common coupling – DC side, essentially one or more converters, together with one or more converter transformers, converter control equipment, essential protective and switching devices and auxiliaries, if any, used for conversion._





**URI**: [cim:DCConverterUnit](http://iec.ch/TC57/CIM100#DCConverterUnit)<br />
**Type**: Class




```mermaid
 classDiagram
    class DCConverterUnit
      DCEquipmentContainer <|-- DCConverterUnit
      
      DCConverterUnit : ConnectivityNodeContainer.ConnectivityNodes
        
          DCConverterUnit --> ConnectivityNode : ConnectivityNodeContainer.ConnectivityNodes
        
      DCConverterUnit : DCEquipmentContainer.DCNodes
        
          DCConverterUnit --> DCNode : DCEquipmentContainer.DCNodes
        
      DCConverterUnit : IdentifiedObject.description
        
      DCConverterUnit : IdentifiedObject.energyIdentCodeEic
        
      DCConverterUnit : EquipmentContainer.Equipments
        
          DCConverterUnit --> Equipment : EquipmentContainer.Equipments
        
      DCConverterUnit : IdentifiedObject.mRID
        
      DCConverterUnit : IdentifiedObject.name
        
      DCConverterUnit : DCConverterUnit.operationMode
        
          DCConverterUnit --> DCConverterOperatingModeKind : DCConverterUnit.operationMode
        
      DCConverterUnit : IdentifiedObject.shortName
        
      DCConverterUnit : DCConverterUnit.Substation
        
          DCConverterUnit --> Substation : DCConverterUnit.Substation
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [ConnectivityNodeContainer](ConnectivityNodeContainer.md)
            * [EquipmentContainer](EquipmentContainer.md)
                * [DCEquipmentContainer](DCEquipmentContainer.md)
                    * **DCConverterUnit**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| operationMode | [cim:DCConverterUnit.operationMode](http://iec.ch/TC57/CIM100#DCConverterUnit.operationMode) | 1..1 <br />  [DCConverterOperatingModeKind](DCConverterOperatingModeKind.md)  | The operating mode of an HVDC bipole (bipolar, monopolar metallic return, etc... | direct |
| Substation | [cim:DCConverterUnit.Substation](http://iec.ch/TC57/CIM100#DCConverterUnit.Substation) | 0..1 <br />  [Substation](Substation.md)  | The containing substation of the DC converter unit | direct |
| DCNodes | [cim:DCEquipmentContainer.DCNodes](http://iec.ch/TC57/CIM100#DCEquipmentContainer.DCNodes) | 0..* <br />  [DCNode](DCNode.md)  | The DC nodes contained in the DC equipment container | [DCEquipmentContainer](DCEquipmentContainer.md) |
| Equipments | [cim:EquipmentContainer.Equipments](http://iec.ch/TC57/CIM100#EquipmentContainer.Equipments) | 0..* <br />  [Equipment](Equipment.md)  | Contained equipment | [EquipmentContainer](EquipmentContainer.md) |
| ConnectivityNodes | [cim:ConnectivityNodeContainer.ConnectivityNodes](http://iec.ch/TC57/CIM100#ConnectivityNodeContainer.ConnectivityNodes) | 0..* <br />  [ConnectivityNode](ConnectivityNode.md)  | Connectivity nodes which belong to this connectivity node container | [ConnectivityNodeContainer](ConnectivityNodeContainer.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [Substation](Substation.md) | DCConverterUnit | range | [DCConverterUnit](DCConverterUnit.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:DCConverterUnit |
| native | this:DCConverterUnit |




