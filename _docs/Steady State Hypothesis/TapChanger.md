# TapChanger


_Mechanism for changing transformer winding tap positions._





**URI**: [cim:TapChanger](http://iec.ch/TC57/CIM100#TapChanger)<br />
**Type**: Class




```mermaid
 classDiagram
    class TapChanger
      PowerSystemResource <|-- TapChanger
      

      TapChanger <|-- PhaseTapChanger
      TapChanger <|-- RatioTapChanger
      
      
      TapChanger : TapChanger.controlEnabled
        
      TapChanger : IdentifiedObject.mRID
        
      TapChanger : TapChanger.step
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * **TapChanger**
            * [PhaseTapChanger](PhaseTapChanger.md)
            * [RatioTapChanger](RatioTapChanger.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| controlEnabled | [cim:TapChanger.controlEnabled](http://iec.ch/TC57/CIM100#TapChanger.controlEnabled) | 1..1 <br />  boolean  | Specifies the regulation status of the equipment | direct |
| step | [cim:TapChanger.step](http://iec.ch/TC57/CIM100#TapChanger.step) | 1..1 <br />  float  | Tap changer position | direct |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:TapChanger |
| native | this:TapChanger |




