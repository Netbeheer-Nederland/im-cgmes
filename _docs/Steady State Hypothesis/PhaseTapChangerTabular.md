# PhaseTapChangerTabular


_Describes a tap changer with a table defining the relation between the tap step and the phase angle difference across the transformer._





**URI**: [cim:PhaseTapChangerTabular](http://iec.ch/TC57/CIM100#PhaseTapChangerTabular)<br />
**Type**: Class




```mermaid
 classDiagram
    class PhaseTapChangerTabular
    click PhaseTapChangerTabular href "../PhaseTapChangerTabular"
      PhaseTapChanger <|-- PhaseTapChangerTabular
        click PhaseTapChanger href "../PhaseTapChanger"
      
      PhaseTapChangerTabular : TapChanger.controlEnabled
        
      PhaseTapChangerTabular : IdentifiedObject.mRID
        
      PhaseTapChangerTabular : TapChanger.step
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [TapChanger](TapChanger.md)
            * [PhaseTapChanger](PhaseTapChanger.md)
                * **PhaseTapChangerTabular**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| controlEnabled | [cim:TapChanger.controlEnabled](http://iec.ch/TC57/CIM100#TapChanger.controlEnabled) | 1 <br />  boolean  | Specifies the regulation status of the equipment | [TapChanger](TapChanger.md) |
| step | [cim:TapChanger.step](http://iec.ch/TC57/CIM100#TapChanger.step) | 1 <br />  float  | Tap changer position | [TapChanger](TapChanger.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:PhaseTapChangerTabular |
| native | this:PhaseTapChangerTabular |




