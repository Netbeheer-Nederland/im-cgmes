# PhaseTapChangerLinear


_Describes a tap changer with a linear relation between the tap step and the phase angle difference across the transformer. This is a mathematical model that is an approximation of a real phase tap changer._

_The phase angle is computed as stepPhaseShiftIncrement times the tap position._

_The voltage magnitude of both sides is the same._





**URI**: [cim:PhaseTapChangerLinear](http://iec.ch/TC57/CIM100#PhaseTapChangerLinear)<br />
**Type**: Class




```mermaid
 classDiagram
    class PhaseTapChangerLinear
    click PhaseTapChangerLinear href "../PhaseTapChangerLinear"
      PhaseTapChanger <|-- PhaseTapChangerLinear
        click PhaseTapChanger href "../PhaseTapChanger"
      
      PhaseTapChangerLinear : TapChanger.controlEnabled
        
      PhaseTapChangerLinear : IdentifiedObject.mRID
        
      PhaseTapChangerLinear : TapChanger.step
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [TapChanger](TapChanger.md)
            * [PhaseTapChanger](PhaseTapChanger.md)
                * **PhaseTapChangerLinear**



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
| self | cim:PhaseTapChangerLinear |
| native | this:PhaseTapChangerLinear |




