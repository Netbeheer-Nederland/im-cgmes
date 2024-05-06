# BasicIntervalSchedule


_Schedule of values at points in time._





**URI**: [cim:BasicIntervalSchedule](http://iec.ch/TC57/CIM100#BasicIntervalSchedule)<br />
**Type**: Class




```mermaid
 classDiagram
    class BasicIntervalSchedule
    click BasicIntervalSchedule href "../BasicIntervalSchedule"
      IdentifiedObject <|-- BasicIntervalSchedule
        click IdentifiedObject href "../IdentifiedObject"
      

      BasicIntervalSchedule <|-- RegularIntervalSchedule
        click RegularIntervalSchedule href "../RegularIntervalSchedule"
      
      
      BasicIntervalSchedule : IdentifiedObject.description
        
      BasicIntervalSchedule : IdentifiedObject.energyIdentCodeEic
        
      BasicIntervalSchedule : IdentifiedObject.mRID
        
      BasicIntervalSchedule : IdentifiedObject.name
        
      BasicIntervalSchedule : IdentifiedObject.shortName
        
      BasicIntervalSchedule : BasicIntervalSchedule.startTime
        
      BasicIntervalSchedule : BasicIntervalSchedule.value1Unit
        
          BasicIntervalSchedule --> UnitSymbol : BasicIntervalSchedule.value1Unit
          click UnitSymbol href "../UnitSymbol"
        
      BasicIntervalSchedule : BasicIntervalSchedule.value2Unit
        
          BasicIntervalSchedule --> UnitSymbol : BasicIntervalSchedule.value2Unit
          click UnitSymbol href "../UnitSymbol"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **BasicIntervalSchedule**
        * [RegularIntervalSchedule](RegularIntervalSchedule.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| startTime | [cim:BasicIntervalSchedule.startTime](http://iec.ch/TC57/CIM100#BasicIntervalSchedule.startTime) | 1 <br />  date  | The time for the first time point | direct |
| value1Unit | [cim:BasicIntervalSchedule.value1Unit](http://iec.ch/TC57/CIM100#BasicIntervalSchedule.value1Unit) | 1 <br />  [UnitSymbol](UnitSymbol.md)  | Value1 units of measure | direct |
| value2Unit | [cim:BasicIntervalSchedule.value2Unit](http://iec.ch/TC57/CIM100#BasicIntervalSchedule.value2Unit) | 0..1 <br />  [UnitSymbol](UnitSymbol.md)  | Value2 units of measure | direct |
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
| self | cim:BasicIntervalSchedule |
| native | this:BasicIntervalSchedule |




