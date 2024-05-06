# RatioTapChanger


_A tap changer that changes the voltage ratio impacting the voltage magnitude but not the phase angle across the transformer._

__

_Angle sign convention (general): Positive value indicates a positive phase shift from the winding where the tap is located to the other winding (for a two-winding transformer)._





**URI**: [cim:RatioTapChanger](http://iec.ch/TC57/CIM100#RatioTapChanger)<br />
**Type**: Class




```mermaid
 classDiagram
    class RatioTapChanger
    click RatioTapChanger href "../RatioTapChanger"
      TapChanger <|-- RatioTapChanger
        click TapChanger href "../TapChanger"
      
      RatioTapChanger : TapChanger.controlEnabled
        
      RatioTapChanger : IdentifiedObject.mRID
        
      RatioTapChanger : TapChanger.step
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [TapChanger](TapChanger.md)
            * **RatioTapChanger**



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
| self | cim:RatioTapChanger |
| native | this:RatioTapChanger |




