# PhaseTapChanger


_A transformer phase shifting tap model that controls the phase angle difference across the power transformer and potentially the active power flow through the power transformer.  This phase tap model may also impact the voltage magnitude._





**URI**: [cim:PhaseTapChanger](http://iec.ch/TC57/CIM100#PhaseTapChanger)<br />
**Type**: Class




```mermaid
 classDiagram
    class PhaseTapChanger
    click PhaseTapChanger href "../PhaseTapChanger"
      TapChanger <|-- PhaseTapChanger
        click TapChanger href "../TapChanger"
      

      PhaseTapChanger <|-- PhaseTapChangerLinear
        click PhaseTapChangerLinear href "../PhaseTapChangerLinear"
      PhaseTapChanger <|-- PhaseTapChangerNonLinear
        click PhaseTapChangerNonLinear href "../PhaseTapChangerNonLinear"
      PhaseTapChanger <|-- PhaseTapChangerTabular
        click PhaseTapChangerTabular href "../PhaseTapChangerTabular"
      
      
      PhaseTapChanger : IdentifiedObject.description
        
      PhaseTapChanger : IdentifiedObject.energyIdentCodeEic
        
      PhaseTapChanger : TapChanger.highStep
        
      PhaseTapChanger : TapChanger.lowStep
        
      PhaseTapChanger : TapChanger.ltcFlag
        
      PhaseTapChanger : IdentifiedObject.mRID
        
      PhaseTapChanger : IdentifiedObject.name
        
      PhaseTapChanger : TapChanger.neutralStep
        
      PhaseTapChanger : TapChanger.neutralU
        
          PhaseTapChanger --> Voltage : TapChanger.neutralU
          click Voltage href "../Voltage"
        
      PhaseTapChanger : TapChanger.normalStep
        
      PhaseTapChanger : IdentifiedObject.shortName
        
      PhaseTapChanger : TapChanger.TapChangerControl
        
          PhaseTapChanger --> TapChangerControl : TapChanger.TapChangerControl
          click TapChangerControl href "../TapChangerControl"
        
      PhaseTapChanger : TapChanger.TapSchedules
        
          PhaseTapChanger --> TapSchedule : TapChanger.TapSchedules
          click TapSchedule href "../TapSchedule"
        
      PhaseTapChanger : PhaseTapChanger.TransformerEnd
        
          PhaseTapChanger --> TransformerEnd : PhaseTapChanger.TransformerEnd
          click TransformerEnd href "../TransformerEnd"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [TapChanger](TapChanger.md)
            * **PhaseTapChanger**
                * [PhaseTapChangerLinear](PhaseTapChangerLinear.md)
                * [PhaseTapChangerNonLinear](PhaseTapChangerNonLinear.md)
                * [PhaseTapChangerTabular](PhaseTapChangerTabular.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| TransformerEnd | [cim:PhaseTapChanger.TransformerEnd](http://iec.ch/TC57/CIM100#PhaseTapChanger.TransformerEnd) | 1 <br />  [TransformerEnd](TransformerEnd.md)  | Transformer end to which this phase tap changer belongs | direct |
| TapSchedules | [cim:TapChanger.TapSchedules](http://iec.ch/TC57/CIM100#TapChanger.TapSchedules) | * <br />  [TapSchedule](TapSchedule.md)  | A TapChanger can have TapSchedules | [TapChanger](TapChanger.md) |
| highStep | [cim:TapChanger.highStep](http://iec.ch/TC57/CIM100#TapChanger.highStep) | 1 <br />  integer  | Highest possible tap step position, advance from neutral | [TapChanger](TapChanger.md) |
| lowStep | [cim:TapChanger.lowStep](http://iec.ch/TC57/CIM100#TapChanger.lowStep) | 1 <br />  integer  | Lowest possible tap step position, retard from neutral | [TapChanger](TapChanger.md) |
| ltcFlag | [cim:TapChanger.ltcFlag](http://iec.ch/TC57/CIM100#TapChanger.ltcFlag) | 1 <br />  boolean  | Specifies whether or not a TapChanger has load tap changing capabilities | [TapChanger](TapChanger.md) |
| neutralStep | [cim:TapChanger.neutralStep](http://iec.ch/TC57/CIM100#TapChanger.neutralStep) | 1 <br />  integer  | The neutral tap step position for this winding | [TapChanger](TapChanger.md) |
| neutralU | [cim:TapChanger.neutralU](http://iec.ch/TC57/CIM100#TapChanger.neutralU) | 1 <br />  [Voltage](Voltage.md)  | Voltage at which the winding operates at the neutral tap setting | [TapChanger](TapChanger.md) |
| normalStep | [cim:TapChanger.normalStep](http://iec.ch/TC57/CIM100#TapChanger.normalStep) | 1 <br />  integer  | The tap step position used in "normal" network operation for this winding | [TapChanger](TapChanger.md) |
| TapChangerControl | [cim:TapChanger.TapChangerControl](http://iec.ch/TC57/CIM100#TapChanger.TapChangerControl) | 0..1 <br />  [TapChangerControl](TapChangerControl.md)  | The regulating control scheme in which this tap changer participates | [TapChanger](TapChanger.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [PowerTransformerEnd](PowerTransformerEnd.md) | PhaseTapChanger | range | [PhaseTapChanger](PhaseTapChanger.md) |
| [TransformerEnd](TransformerEnd.md) | PhaseTapChanger | range | [PhaseTapChanger](PhaseTapChanger.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:PhaseTapChanger |
| native | this:PhaseTapChanger |




