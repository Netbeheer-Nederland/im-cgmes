# PhaseTapChangerSymmetrical


_Describes a symmetrical phase shifting transformer tap model in which the voltage magnitude of both sides is the same. The difference voltage magnitude is the base in an equal-sided triangle where the sides corresponds to the primary and secondary voltages. The phase angle difference corresponds to the top angle and can be expressed as twice the arctangent of half the total difference voltage._





**URI**: [cim:PhaseTapChangerSymmetrical](http://iec.ch/TC57/CIM100#PhaseTapChangerSymmetrical)<br />
**Type**: Class




```mermaid
 classDiagram
    class PhaseTapChangerSymmetrical
    click PhaseTapChangerSymmetrical href "../PhaseTapChangerSymmetrical"
      PhaseTapChangerNonLinear <|-- PhaseTapChangerSymmetrical
        click PhaseTapChangerNonLinear href "../PhaseTapChangerNonLinear"
      
      PhaseTapChangerSymmetrical : IdentifiedObject.description
        
      PhaseTapChangerSymmetrical : IdentifiedObject.energyIdentCodeEic
        
      PhaseTapChangerSymmetrical : TapChanger.highStep
        
      PhaseTapChangerSymmetrical : TapChanger.lowStep
        
      PhaseTapChangerSymmetrical : TapChanger.ltcFlag
        
      PhaseTapChangerSymmetrical : IdentifiedObject.mRID
        
      PhaseTapChangerSymmetrical : IdentifiedObject.name
        
      PhaseTapChangerSymmetrical : TapChanger.neutralStep
        
      PhaseTapChangerSymmetrical : TapChanger.neutralU
        
          PhaseTapChangerSymmetrical --> Voltage : TapChanger.neutralU
          click Voltage href "../Voltage"
        
      PhaseTapChangerSymmetrical : TapChanger.normalStep
        
      PhaseTapChangerSymmetrical : IdentifiedObject.shortName
        
      PhaseTapChangerSymmetrical : TapChanger.TapChangerControl
        
          PhaseTapChangerSymmetrical --> TapChangerControl : TapChanger.TapChangerControl
          click TapChangerControl href "../TapChangerControl"
        
      PhaseTapChangerSymmetrical : TapChanger.TapSchedules
        
          PhaseTapChangerSymmetrical --> TapSchedule : TapChanger.TapSchedules
          click TapSchedule href "../TapSchedule"
        
      PhaseTapChangerSymmetrical : PhaseTapChanger.TransformerEnd
        
          PhaseTapChangerSymmetrical --> TransformerEnd : PhaseTapChanger.TransformerEnd
          click TransformerEnd href "../TransformerEnd"
        
      PhaseTapChangerSymmetrical : PhaseTapChangerNonLinear.voltageStepIncrement
        
          PhaseTapChangerSymmetrical --> PerCent : PhaseTapChangerNonLinear.voltageStepIncrement
          click PerCent href "../PerCent"
        
      PhaseTapChangerSymmetrical : PhaseTapChangerNonLinear.xMax
        
          PhaseTapChangerSymmetrical --> Reactance : PhaseTapChangerNonLinear.xMax
          click Reactance href "../Reactance"
        
      PhaseTapChangerSymmetrical : PhaseTapChangerNonLinear.xMin
        
          PhaseTapChangerSymmetrical --> Reactance : PhaseTapChangerNonLinear.xMin
          click Reactance href "../Reactance"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [TapChanger](TapChanger.md)
            * [PhaseTapChanger](PhaseTapChanger.md)
                * [PhaseTapChangerNonLinear](PhaseTapChangerNonLinear.md)
                    * **PhaseTapChangerSymmetrical**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| voltageStepIncrement | [cim:PhaseTapChangerNonLinear.voltageStepIncrement](http://iec.ch/TC57/CIM100#PhaseTapChangerNonLinear.voltageStepIncrement) | 1 <br />  [PerCent](PerCent.md)  | The voltage step increment on the out of phase winding (the PowerTransformerE... | [PhaseTapChangerNonLinear](PhaseTapChangerNonLinear.md) |
| xMax | [cim:PhaseTapChangerNonLinear.xMax](http://iec.ch/TC57/CIM100#PhaseTapChangerNonLinear.xMax) | 1 <br />  [Reactance](Reactance.md)  | The reactance depends on the tap position according to a "u" shaped curve | [PhaseTapChangerNonLinear](PhaseTapChangerNonLinear.md) |
| xMin | [cim:PhaseTapChangerNonLinear.xMin](http://iec.ch/TC57/CIM100#PhaseTapChangerNonLinear.xMin) | 1 <br />  [Reactance](Reactance.md)  | The reactance depend on the tap position according to a "u" shaped curve | [PhaseTapChangerNonLinear](PhaseTapChangerNonLinear.md) |
| TransformerEnd | [cim:PhaseTapChanger.TransformerEnd](http://iec.ch/TC57/CIM100#PhaseTapChanger.TransformerEnd) | 1 <br />  [TransformerEnd](TransformerEnd.md)  | Transformer end to which this phase tap changer belongs | [PhaseTapChanger](PhaseTapChanger.md) |
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









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:PhaseTapChangerSymmetrical |
| native | this:PhaseTapChangerSymmetrical |




