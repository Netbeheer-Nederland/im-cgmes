# PFVArType2IEEEVArController


_IEEE VAR controller type 2 which is a summing point type controller. It makes up the outside loop of a two-loop system. This controller is implemented as a slow PI type controller, and the voltage regulator forms the inner loop and is implemented as a fast controller._

_Reference: IEEE 421.5-2005, 11.5._





**URI**: [cim:PFVArType2IEEEVArController](http://iec.ch/TC57/CIM100#PFVArType2IEEEVArController)<br />
**Type**: Class




```mermaid
 classDiagram
    class PFVArType2IEEEVArController
      PFVArControllerType2Dynamics <|-- PFVArType2IEEEVArController
      
      PFVArType2IEEEVArController : IdentifiedObject.description
        
      PFVArType2IEEEVArController : DynamicsFunctionBlock.enabled
        
      PFVArType2IEEEVArController : PFVArControllerType2Dynamics.ExcitationSystemDynamics
        
          PFVArType2IEEEVArController --> ExcitationSystemDynamics : PFVArControllerType2Dynamics.ExcitationSystemDynamics
        
      PFVArType2IEEEVArController : PFVArType2IEEEVArController.exlon
        
      PFVArType2IEEEVArController : PFVArType2IEEEVArController.ki
        
          PFVArType2IEEEVArController --> PU : PFVArType2IEEEVArController.ki
        
      PFVArType2IEEEVArController : PFVArType2IEEEVArController.kp
        
          PFVArType2IEEEVArController --> PU : PFVArType2IEEEVArController.kp
        
      PFVArType2IEEEVArController : IdentifiedObject.mRID
        
      PFVArType2IEEEVArController : IdentifiedObject.name
        
      PFVArType2IEEEVArController : PFVArType2IEEEVArController.qref
        
          PFVArType2IEEEVArController --> PU : PFVArType2IEEEVArController.qref
        
      PFVArType2IEEEVArController : PFVArType2IEEEVArController.vclmt
        
          PFVArType2IEEEVArController --> PU : PFVArType2IEEEVArController.vclmt
        
      PFVArType2IEEEVArController : PFVArType2IEEEVArController.vref
        
          PFVArType2IEEEVArController --> PU : PFVArType2IEEEVArController.vref
        
      PFVArType2IEEEVArController : PFVArType2IEEEVArController.vs
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md)
            * **PFVArType2IEEEVArController**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| qref | [cim:PFVArType2IEEEVArController.qref](http://iec.ch/TC57/CIM100#PFVArType2IEEEVArController.qref) | 1..1 <br />  [PU](PU.md)  | Reactive power reference (<i>Q</i><i><sub>REF</sub></i>) | direct |
| vref | [cim:PFVArType2IEEEVArController.vref](http://iec.ch/TC57/CIM100#PFVArType2IEEEVArController.vref) | 1..1 <br />  [PU](PU.md)  | Voltage regulator reference (<i>V</i><i><sub>REF</sub></i>) | direct |
| vclmt | [cim:PFVArType2IEEEVArController.vclmt](http://iec.ch/TC57/CIM100#PFVArType2IEEEVArController.vclmt) | 1..1 <br />  [PU](PU.md)  | Maximum output of the pf controller (<i>V</i><i><sub>CLMT</sub></i>) | direct |
| kp | [cim:PFVArType2IEEEVArController.kp](http://iec.ch/TC57/CIM100#PFVArType2IEEEVArController.kp) | 1..1 <br />  [PU](PU.md)  | Proportional gain of the pf controller (<i>K</i><i><sub>P</sub></i>) | direct |
| ki | [cim:PFVArType2IEEEVArController.ki](http://iec.ch/TC57/CIM100#PFVArType2IEEEVArController.ki) | 1..1 <br />  [PU](PU.md)  | Integral gain of the pf controller (<i>K</i><i><sub>I</sub></i>) | direct |
| vs | [cim:PFVArType2IEEEVArController.vs](http://iec.ch/TC57/CIM100#PFVArType2IEEEVArController.vs) | 1..1 <br />  float  | Generator sensing voltage (<i>V</i><i><sub>S</sub></i>) | direct |
| exlon | [cim:PFVArType2IEEEVArController.exlon](http://iec.ch/TC57/CIM100#PFVArType2IEEEVArController.exlon) | 1..1 <br />  boolean  | Overexcitation or under excitation flag (<i>EXLON</i>) | direct |
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
| self | cim:PFVArType2IEEEVArController |
| native | this:PFVArType2IEEEVArController |




