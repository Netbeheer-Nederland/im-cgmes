# RatioTapChangerTablePoint


_Describes each tap step in the ratio tap changer tabular curve._





**URI**: [cim:RatioTapChangerTablePoint](http://iec.ch/TC57/CIM100#RatioTapChangerTablePoint)<br />
**Type**: Class




```mermaid
 classDiagram
    class RatioTapChangerTablePoint
    click RatioTapChangerTablePoint href "../RatioTapChangerTablePoint"
      TapChangerTablePoint <|-- RatioTapChangerTablePoint
        click TapChangerTablePoint href "../TapChangerTablePoint"
      
      RatioTapChangerTablePoint : TapChangerTablePoint.b
        
          RatioTapChangerTablePoint --> PerCent : TapChangerTablePoint.b
          click PerCent href "../PerCent"
        
      RatioTapChangerTablePoint : TapChangerTablePoint.g
        
          RatioTapChangerTablePoint --> PerCent : TapChangerTablePoint.g
          click PerCent href "../PerCent"
        
      RatioTapChangerTablePoint : TapChangerTablePoint.r
        
          RatioTapChangerTablePoint --> PerCent : TapChangerTablePoint.r
          click PerCent href "../PerCent"
        
      RatioTapChangerTablePoint : TapChangerTablePoint.ratio
        
      RatioTapChangerTablePoint : RatioTapChangerTablePoint.RatioTapChangerTable
        
          RatioTapChangerTablePoint --> RatioTapChangerTable : RatioTapChangerTablePoint.RatioTapChangerTable
          click RatioTapChangerTable href "../RatioTapChangerTable"
        
      RatioTapChangerTablePoint : TapChangerTablePoint.step
        
      RatioTapChangerTablePoint : TapChangerTablePoint.x
        
          RatioTapChangerTablePoint --> PerCent : TapChangerTablePoint.x
          click PerCent href "../PerCent"
        
      
```





## Inheritance
* [TapChangerTablePoint](TapChangerTablePoint.md)
    * **RatioTapChangerTablePoint**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| RatioTapChangerTable | [cim:RatioTapChangerTablePoint.RatioTapChangerTable](http://iec.ch/TC57/CIM100#RatioTapChangerTablePoint.RatioTapChangerTable) | 1 <br />  [RatioTapChangerTable](RatioTapChangerTable.md)  | Table of this point | direct |
| b | [cim:TapChangerTablePoint.b](http://iec.ch/TC57/CIM100#TapChangerTablePoint.b) | 0..1 <br />  [PerCent](PerCent.md)  | The magnetizing branch susceptance deviation as a percentage of nominal value | [TapChangerTablePoint](TapChangerTablePoint.md) |
| g | [cim:TapChangerTablePoint.g](http://iec.ch/TC57/CIM100#TapChangerTablePoint.g) | 0..1 <br />  [PerCent](PerCent.md)  | The magnetizing branch conductance deviation as a percentage of nominal value | [TapChangerTablePoint](TapChangerTablePoint.md) |
| r | [cim:TapChangerTablePoint.r](http://iec.ch/TC57/CIM100#TapChangerTablePoint.r) | 0..1 <br />  [PerCent](PerCent.md)  | The resistance deviation as a percentage of nominal value | [TapChangerTablePoint](TapChangerTablePoint.md) |
| ratio | [cim:TapChangerTablePoint.ratio](http://iec.ch/TC57/CIM100#TapChangerTablePoint.ratio) | 0..1 <br />  float  | The voltage at the tap step divided by rated voltage of the transformer end h... | [TapChangerTablePoint](TapChangerTablePoint.md) |
| step | [cim:TapChangerTablePoint.step](http://iec.ch/TC57/CIM100#TapChangerTablePoint.step) | 1 <br />  integer  | The tap step | [TapChangerTablePoint](TapChangerTablePoint.md) |
| x | [cim:TapChangerTablePoint.x](http://iec.ch/TC57/CIM100#TapChangerTablePoint.x) | 0..1 <br />  [PerCent](PerCent.md)  | The series reactance deviation as a percentage of nominal value | [TapChangerTablePoint](TapChangerTablePoint.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [RatioTapChangerTable](RatioTapChangerTable.md) | RatioTapChangerTablePoint | range | [RatioTapChangerTablePoint](RatioTapChangerTablePoint.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:RatioTapChangerTablePoint |
| native | this:RatioTapChangerTablePoint |




