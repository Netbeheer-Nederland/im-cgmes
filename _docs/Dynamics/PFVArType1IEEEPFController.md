# PFVArType1IEEEPFController


_IEEE PF controller type 1 which operates by moving the voltage reference directly._

_Reference: IEEE 421.5-2005, 11.2._





**URI**: [cim:PFVArType1IEEEPFController](http://iec.ch/TC57/CIM100#PFVArType1IEEEPFController)<br />
**Type**: Class




```mermaid
 classDiagram
    class PFVArType1IEEEPFController
      PFVArControllerType1Dynamics <|-- PFVArType1IEEEPFController
      
      PFVArType1IEEEPFController : IdentifiedObject.description
        
      PFVArType1IEEEPFController : DynamicsFunctionBlock.enabled
        
      PFVArType1IEEEPFController : PFVArControllerType1Dynamics.ExcitationSystemDynamics
        
          PFVArType1IEEEPFController --> ExcitationSystemDynamics : PFVArControllerType1Dynamics.ExcitationSystemDynamics
        
      PFVArType1IEEEPFController : IdentifiedObject.mRID
        
      PFVArType1IEEEPFController : IdentifiedObject.name
        
      PFVArType1IEEEPFController : PFVArType1IEEEPFController.ovex
        
      PFVArType1IEEEPFController : PFVArControllerType1Dynamics.RemoteInputSignal
        
          PFVArType1IEEEPFController --> RemoteInputSignal : PFVArControllerType1Dynamics.RemoteInputSignal
        
      PFVArType1IEEEPFController : PFVArType1IEEEPFController.tpfc
        
          PFVArType1IEEEPFController --> Seconds : PFVArType1IEEEPFController.tpfc
        
      PFVArType1IEEEPFController : PFVArType1IEEEPFController.vitmin
        
          PFVArType1IEEEPFController --> PU : PFVArType1IEEEPFController.vitmin
        
      PFVArType1IEEEPFController : PFVArControllerType1Dynamics.VoltageAdjusterDynamics
        
          PFVArType1IEEEPFController --> VoltageAdjusterDynamics : PFVArControllerType1Dynamics.VoltageAdjusterDynamics
        
      PFVArType1IEEEPFController : PFVArType1IEEEPFController.vpf
        
          PFVArType1IEEEPFController --> PU : PFVArType1IEEEPFController.vpf
        
      PFVArType1IEEEPFController : PFVArType1IEEEPFController.vpfcbw
        
      PFVArType1IEEEPFController : PFVArType1IEEEPFController.vpfref
        
          PFVArType1IEEEPFController --> PU : PFVArType1IEEEPFController.vpfref
        
      PFVArType1IEEEPFController : PFVArType1IEEEPFController.vvtmax
        
          PFVArType1IEEEPFController --> PU : PFVArType1IEEEPFController.vvtmax
        
      PFVArType1IEEEPFController : PFVArType1IEEEPFController.vvtmin
        
          PFVArType1IEEEPFController --> PU : PFVArType1IEEEPFController.vvtmin
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md)
            * **PFVArType1IEEEPFController**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ovex | [cim:PFVArType1IEEEPFController.ovex](http://iec.ch/TC57/CIM100#PFVArType1IEEEPFController.ovex) | 1..1 <br />  boolean  | Overexcitation Flag (<i>OVEX</i>) | direct |
| tpfc | [cim:PFVArType1IEEEPFController.tpfc](http://iec.ch/TC57/CIM100#PFVArType1IEEEPFController.tpfc) | 1..1 <br />  [Seconds](Seconds.md)  | PF controller time delay (<i>T</i><i><sub>PFC</sub></i>) (&gt;= 0) | direct |
| vitmin | [cim:PFVArType1IEEEPFController.vitmin](http://iec.ch/TC57/CIM100#PFVArType1IEEEPFController.vitmin) | 1..1 <br />  [PU](PU.md)  | Minimum machine terminal current needed to enable pf/var controller (<i>V</i>... | direct |
| vpf | [cim:PFVArType1IEEEPFController.vpf](http://iec.ch/TC57/CIM100#PFVArType1IEEEPFController.vpf) | 1..1 <br />  [PU](PU.md)  | Synchronous machine power factor (<i>V</i><i><sub>PF</sub></i>) | direct |
| vpfcbw | [cim:PFVArType1IEEEPFController.vpfcbw](http://iec.ch/TC57/CIM100#PFVArType1IEEEPFController.vpfcbw) | 1..1 <br />  float  | PF controller deadband (<i>V</i><i><sub>PFC_BW</sub></i>) | direct |
| vpfref | [cim:PFVArType1IEEEPFController.vpfref](http://iec.ch/TC57/CIM100#PFVArType1IEEEPFController.vpfref) | 1..1 <br />  [PU](PU.md)  | PF controller reference (<i>V</i><i><sub>PFREF</sub></i>) | direct |
| vvtmax | [cim:PFVArType1IEEEPFController.vvtmax](http://iec.ch/TC57/CIM100#PFVArType1IEEEPFController.vvtmax) | 1..1 <br />  [PU](PU.md)  | Maximum machine terminal voltage needed for pf/var controller to be enabled (... | direct |
| vvtmin | [cim:PFVArType1IEEEPFController.vvtmin](http://iec.ch/TC57/CIM100#PFVArType1IEEEPFController.vvtmin) | 1..1 <br />  [PU](PU.md)  | Minimum machine terminal voltage needed to enable pf/var controller (<i>V</i>... | direct |
| RemoteInputSignal | [cim:PFVArControllerType1Dynamics.RemoteInputSignal](http://iec.ch/TC57/CIM100#PFVArControllerType1Dynamics.RemoteInputSignal) | 0..1 <br />  [RemoteInputSignal](RemoteInputSignal.md)  | Remote input signal used by this power factor or VAr controller type 1 model | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| ExcitationSystemDynamics | [cim:PFVArControllerType1Dynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#PFVArControllerType1Dynamics.ExcitationSystemDynamics) | 1..1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model with which this power actor or VAr controller type 1 ... | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
| VoltageAdjusterDynamics | [cim:PFVArControllerType1Dynamics.VoltageAdjusterDynamics](http://iec.ch/TC57/CIM100#PFVArControllerType1Dynamics.VoltageAdjusterDynamics) | 0..1 <br />  [VoltageAdjusterDynamics](VoltageAdjusterDynamics.md)  | Voltage adjuster model associated with this power factor or VAr controller ty... | [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md) |
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
| self | cim:PFVArType1IEEEPFController |
| native | this:PFVArType1IEEEPFController |




