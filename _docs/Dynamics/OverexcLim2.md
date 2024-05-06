# OverexcLim2


_Different from LimIEEEOEL, LimOEL2 has a fixed pickup threshold and reduces the excitation set-point by means of a non-windup integral regulator._

_<i>Irated</i> is the rated machine excitation current (calculated from nameplate conditions: <i>V</i><i><sub>nom</sub></i>, <i>P</i><i><sub>nom</sub></i>, <i>CosPhi</i><i><sub>nom</sub></i>)._





**URI**: [cim:OverexcLim2](http://iec.ch/TC57/CIM100#OverexcLim2)<br />
**Type**: Class




```mermaid
 classDiagram
    class OverexcLim2
    click OverexcLim2 href "../OverexcLim2"
      OverexcitationLimiterDynamics <|-- OverexcLim2
        click OverexcitationLimiterDynamics href "../OverexcitationLimiterDynamics"
      
      OverexcLim2 : IdentifiedObject.description
        
      OverexcLim2 : DynamicsFunctionBlock.enabled
        
      OverexcLim2 : OverexcitationLimiterDynamics.ExcitationSystemDynamics
        
          OverexcLim2 --> ExcitationSystemDynamics : OverexcitationLimiterDynamics.ExcitationSystemDynamics
          click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
        
      OverexcLim2 : OverexcLim2.ifdlim
        
          OverexcLim2 --> PU : OverexcLim2.ifdlim
          click PU href "../PU"
        
      OverexcLim2 : OverexcLim2.koi
        
          OverexcLim2 --> PU : OverexcLim2.koi
          click PU href "../PU"
        
      OverexcLim2 : IdentifiedObject.mRID
        
      OverexcLim2 : IdentifiedObject.name
        
      OverexcLim2 : OverexcLim2.voimax
        
          OverexcLim2 --> PU : OverexcLim2.voimax
          click PU href "../PU"
        
      OverexcLim2 : OverexcLim2.voimin
        
          OverexcLim2 --> PU : OverexcLim2.voimin
          click PU href "../PU"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md)
            * **OverexcLim2**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| koi | [cim:OverexcLim2.koi](http://iec.ch/TC57/CIM100#OverexcLim2.koi) | 1 <br />  [PU](PU.md)  | Gain Over excitation limiter (<i>K</i><i><sub>OI</sub></i>) | direct |
| voimax | [cim:OverexcLim2.voimax](http://iec.ch/TC57/CIM100#OverexcLim2.voimax) | 1 <br />  [PU](PU.md)  | Maximum error signal (<i>V</i><i><sub>OIMAX</sub></i>) (&gt; OverexcLim2 | direct |
| voimin | [cim:OverexcLim2.voimin](http://iec.ch/TC57/CIM100#OverexcLim2.voimin) | 1 <br />  [PU](PU.md)  | Minimum error signal (<i>V</i><i><sub>OIMIN</sub></i>) (&lt; OverexcLim2 | direct |
| ifdlim | [cim:OverexcLim2.ifdlim](http://iec.ch/TC57/CIM100#OverexcLim2.ifdlim) | 1 <br />  [PU](PU.md)  | Limit value of rated field current (<i>I</i><i><sub>FDLIM</sub></i>) | direct |
| ExcitationSystemDynamics | [cim:OverexcitationLimiterDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#OverexcitationLimiterDynamics.ExcitationSystemDynamics) | 1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this overexcitation limiter model is assoc... | [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:OverexcLim2 |
| native | this:OverexcLim2 |




