# RatioTapChanger


_A tap changer that changes the voltage ratio impacting the voltage magnitude but not the phase angle across the transformer._

__

_Angle sign convention (general): Positive value indicates a positive phase shift from the winding where the tap is located to the other winding (for a two-winding transformer)._





**URI**: [cim:RatioTapChanger](http://iec.ch/TC57/CIM100#RatioTapChanger)<br />
**Type**: Class




```mermaid
 classDiagram
    class RatioTapChanger
      TapChanger <|-- RatioTapChanger
      
      RatioTapChanger : IdentifiedObject.description
        
      RatioTapChanger : IdentifiedObject.energyIdentCodeEic
        
      RatioTapChanger : TapChanger.highStep
        
      RatioTapChanger : TapChanger.lowStep
        
      RatioTapChanger : TapChanger.ltcFlag
        
      RatioTapChanger : IdentifiedObject.mRID
        
      RatioTapChanger : IdentifiedObject.name
        
      RatioTapChanger : TapChanger.neutralStep
        
      RatioTapChanger : TapChanger.neutralU
        
          RatioTapChanger --> Voltage : TapChanger.neutralU
        
      RatioTapChanger : TapChanger.normalStep
        
      RatioTapChanger : RatioTapChanger.RatioTapChangerTable
        
          RatioTapChanger --> RatioTapChangerTable : RatioTapChanger.RatioTapChangerTable
        
      RatioTapChanger : IdentifiedObject.shortName
        
      RatioTapChanger : RatioTapChanger.stepVoltageIncrement
        
          RatioTapChanger --> PerCent : RatioTapChanger.stepVoltageIncrement
        
      RatioTapChanger : TapChanger.TapChangerControl
        
          RatioTapChanger --> TapChangerControl : TapChanger.TapChangerControl
        
      RatioTapChanger : TapChanger.TapSchedules
        
          RatioTapChanger --> TapSchedule : TapChanger.TapSchedules
        
      RatioTapChanger : RatioTapChanger.TransformerEnd
        
          RatioTapChanger --> TransformerEnd : RatioTapChanger.TransformerEnd
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [TapChanger](TapChanger.md)
            * **RatioTapChanger**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| stepVoltageIncrement | [cim:RatioTapChanger.stepVoltageIncrement](http://iec.ch/TC57/CIM100#RatioTapChanger.stepVoltageIncrement) | 1..1 <br />  [PerCent](PerCent.md)  | Tap step increment, in per cent of rated voltage of the power transformer end... | direct |
| RatioTapChangerTable | [cim:RatioTapChanger.RatioTapChangerTable](http://iec.ch/TC57/CIM100#RatioTapChanger.RatioTapChangerTable) | 0..1 <br />  [RatioTapChangerTable](RatioTapChangerTable.md)  | The tap ratio table for this ratio  tap changer | direct |
| TransformerEnd | [cim:RatioTapChanger.TransformerEnd](http://iec.ch/TC57/CIM100#RatioTapChanger.TransformerEnd) | 1..1 <br />  [TransformerEnd](TransformerEnd.md)  | Transformer end to which this ratio tap changer belongs | direct |
| TapSchedules | [cim:TapChanger.TapSchedules](http://iec.ch/TC57/CIM100#TapChanger.TapSchedules) | 0..* <br />  [TapSchedule](TapSchedule.md)  | A TapChanger can have TapSchedules | [TapChanger](TapChanger.md) |
| highStep | [cim:TapChanger.highStep](http://iec.ch/TC57/CIM100#TapChanger.highStep) | 1..1 <br />  integer  | Highest possible tap step position, advance from neutral | [TapChanger](TapChanger.md) |
| lowStep | [cim:TapChanger.lowStep](http://iec.ch/TC57/CIM100#TapChanger.lowStep) | 1..1 <br />  integer  | Lowest possible tap step position, retard from neutral | [TapChanger](TapChanger.md) |
| ltcFlag | [cim:TapChanger.ltcFlag](http://iec.ch/TC57/CIM100#TapChanger.ltcFlag) | 1..1 <br />  boolean  | Specifies whether or not a TapChanger has load tap changing capabilities | [TapChanger](TapChanger.md) |
| neutralStep | [cim:TapChanger.neutralStep](http://iec.ch/TC57/CIM100#TapChanger.neutralStep) | 1..1 <br />  integer  | The neutral tap step position for this winding | [TapChanger](TapChanger.md) |
| neutralU | [cim:TapChanger.neutralU](http://iec.ch/TC57/CIM100#TapChanger.neutralU) | 1..1 <br />  [Voltage](Voltage.md)  | Voltage at which the winding operates at the neutral tap setting | [TapChanger](TapChanger.md) |
| normalStep | [cim:TapChanger.normalStep](http://iec.ch/TC57/CIM100#TapChanger.normalStep) | 1..1 <br />  integer  | The tap step position used in "normal" network operation for this winding | [TapChanger](TapChanger.md) |
| TapChangerControl | [cim:TapChanger.TapChangerControl](http://iec.ch/TC57/CIM100#TapChanger.TapChangerControl) | 0..1 <br />  [TapChangerControl](TapChangerControl.md)  | The regulating control scheme in which this tap changer participates | [TapChanger](TapChanger.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [PowerTransformerEnd](PowerTransformerEnd.md) | RatioTapChanger | range | [RatioTapChanger](RatioTapChanger.md) |
| [RatioTapChangerTable](RatioTapChangerTable.md) | RatioTapChanger | range | [RatioTapChanger](RatioTapChanger.md) |
| [TransformerEnd](TransformerEnd.md) | RatioTapChanger | range | [RatioTapChanger](RatioTapChanger.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:RatioTapChanger |
| native | this:RatioTapChanger |




