# PFVArType2IEEEPFController


_IEEE PF controller type 2 which is a summing point type controller making up the outside loop of a two-loop system. This controller is implemented as a slow PI type controller. The voltage regulator forms the inner loop and is implemented as a fast controller._

_Reference: IEEE 421.5-2005, 11.4._





**URI**: [cim:PFVArType2IEEEPFController](http://iec.ch/TC57/CIM100#PFVArType2IEEEPFController)<br />
**Type**: Class




```mermaid
 classDiagram
    class PFVArType2IEEEPFController
      PFVArControllerType2Dynamics <|-- PFVArType2IEEEPFController
      
      PFVArType2IEEEPFController : IdentifiedObject.description
        
      PFVArType2IEEEPFController : DynamicsFunctionBlock.enabled
        
      PFVArType2IEEEPFController : PFVArControllerType2Dynamics.ExcitationSystemDynamics
        
          PFVArType2IEEEPFController --> ExcitationSystemDynamics : PFVArControllerType2Dynamics.ExcitationSystemDynamics
        
      PFVArType2IEEEPFController : PFVArType2IEEEPFController.exlon
        
      PFVArType2IEEEPFController : PFVArType2IEEEPFController.ki
        
          PFVArType2IEEEPFController --> PU : PFVArType2IEEEPFController.ki
        
      PFVArType2IEEEPFController : PFVArType2IEEEPFController.kp
        
          PFVArType2IEEEPFController --> PU : PFVArType2IEEEPFController.kp
        
      PFVArType2IEEEPFController : IdentifiedObject.mRID
        
      PFVArType2IEEEPFController : IdentifiedObject.name
        
      PFVArType2IEEEPFController : PFVArType2IEEEPFController.pfref
        
          PFVArType2IEEEPFController --> PU : PFVArType2IEEEPFController.pfref
        
      PFVArType2IEEEPFController : PFVArType2IEEEPFController.vclmt
        
          PFVArType2IEEEPFController --> PU : PFVArType2IEEEPFController.vclmt
        
      PFVArType2IEEEPFController : PFVArType2IEEEPFController.vref
        
          PFVArType2IEEEPFController --> PU : PFVArType2IEEEPFController.vref
        
      PFVArType2IEEEPFController : PFVArType2IEEEPFController.vs
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md)
            * **PFVArType2IEEEPFController**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| pfref | [cim:PFVArType2IEEEPFController.pfref](http://iec.ch/TC57/CIM100#PFVArType2IEEEPFController.pfref) | 1..1 <br />  [PU](PU.md)  | Power factor reference (<i>P</i><i><sub>FREF</sub></i>) | direct |
| vref | [cim:PFVArType2IEEEPFController.vref](http://iec.ch/TC57/CIM100#PFVArType2IEEEPFController.vref) | 1..1 <br />  [PU](PU.md)  | Voltage regulator reference (<i>V</i><i><sub>REF</sub></i>) | direct |
| vclmt | [cim:PFVArType2IEEEPFController.vclmt](http://iec.ch/TC57/CIM100#PFVArType2IEEEPFController.vclmt) | 1..1 <br />  [PU](PU.md)  | Maximum output of the pf controller (<i>V</i><i><sub>CLMT</sub></i>) | direct |
| kp | [cim:PFVArType2IEEEPFController.kp](http://iec.ch/TC57/CIM100#PFVArType2IEEEPFController.kp) | 1..1 <br />  [PU](PU.md)  | Proportional gain of the pf controller (<i>K</i><i><sub>P</sub></i>) | direct |
| ki | [cim:PFVArType2IEEEPFController.ki](http://iec.ch/TC57/CIM100#PFVArType2IEEEPFController.ki) | 1..1 <br />  [PU](PU.md)  | Integral gain of the pf controller (<i>K</i><i><sub>I</sub></i>) | direct |
| vs | [cim:PFVArType2IEEEPFController.vs](http://iec.ch/TC57/CIM100#PFVArType2IEEEPFController.vs) | 1..1 <br />  float  | Generator sensing voltage (<i>V</i><i><sub>S</sub></i>) | direct |
| exlon | [cim:PFVArType2IEEEPFController.exlon](http://iec.ch/TC57/CIM100#PFVArType2IEEEPFController.exlon) | 1..1 <br />  boolean  | Overexcitation or under excitation flag (<i>EXLON</i>) | direct |
| ExcitationSystemDynamics | [cim:PFVArControllerType2Dynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#PFVArControllerType2Dynamics.ExcitationSystemDynamics) | 1..1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this power factor or VAr controller type 2... | [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md) |
| enabled | [cim:DynamicsFunctionBlock.enabled](http://iec.ch/TC57/CIM100#DynamicsFunctionBlock.enabled) | 1..1 <br />  boolean  | Function block used indicator | [DynamicsFunctionBlock](DynamicsFunctionBlock.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:PFVArType2IEEEPFController |
| native | this:PFVArType2IEEEPFController |




