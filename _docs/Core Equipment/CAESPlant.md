# CAESPlant


_Compressed air energy storage plant._





**URI**: [cim:CAESPlant](http://iec.ch/TC57/CIM100#CAESPlant)<br />
**Type**: Class




```mermaid
 classDiagram
    class CAESPlant
    click CAESPlant href "../CAESPlant"
      PowerSystemResource <|-- CAESPlant
        click PowerSystemResource href "../PowerSystemResource"
      
      CAESPlant : IdentifiedObject.description
        
      CAESPlant : IdentifiedObject.energyIdentCodeEic
        
      CAESPlant : IdentifiedObject.mRID
        
      CAESPlant : IdentifiedObject.name
        
      CAESPlant : IdentifiedObject.shortName
        
      CAESPlant : CAESPlant.ThermalGeneratingUnit
        
          CAESPlant --> ThermalGeneratingUnit : CAESPlant.ThermalGeneratingUnit
          click ThermalGeneratingUnit href "../ThermalGeneratingUnit"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * **CAESPlant**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ThermalGeneratingUnit | [cim:CAESPlant.ThermalGeneratingUnit](http://iec.ch/TC57/CIM100#CAESPlant.ThermalGeneratingUnit) | 0..1 <br />  [ThermalGeneratingUnit](ThermalGeneratingUnit.md)  | A thermal generating unit may be a member of a compressed air energy storage ... | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ThermalGeneratingUnit](ThermalGeneratingUnit.md) | CAESPlant | range | [CAESPlant](CAESPlant.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:CAESPlant |
| native | this:CAESPlant |




