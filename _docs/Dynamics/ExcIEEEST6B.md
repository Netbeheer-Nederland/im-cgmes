# ExcIEEEST6B


_IEEE 421.5-2005 type ST6B model. This model consists of a PI voltage regulator with an inner loop field voltage regulator and pre-control. The field voltage regulator implements a proportional control. The pre-control and the delay in the feedback circuit increase the dynamic response._

_Reference: IEEE 421.5-2005, 7.6._





**URI**: [cim:ExcIEEEST6B](http://iec.ch/TC57/CIM100#ExcIEEEST6B)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcIEEEST6B
      ExcitationSystemDynamics <|-- ExcIEEEST6B
      
      ExcIEEEST6B : IdentifiedObject.description
        
      ExcIEEEST6B : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcIEEEST6B --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
      ExcIEEEST6B : DynamicsFunctionBlock.enabled
        
      ExcIEEEST6B : ExcIEEEST6B.ilr
        
          ExcIEEEST6B --> PU : ExcIEEEST6B.ilr
        
      ExcIEEEST6B : ExcIEEEST6B.kci
        
          ExcIEEEST6B --> PU : ExcIEEEST6B.kci
        
      ExcIEEEST6B : ExcIEEEST6B.kff
        
          ExcIEEEST6B --> PU : ExcIEEEST6B.kff
        
      ExcIEEEST6B : ExcIEEEST6B.kg
        
          ExcIEEEST6B --> PU : ExcIEEEST6B.kg
        
      ExcIEEEST6B : ExcIEEEST6B.kia
        
          ExcIEEEST6B --> PU : ExcIEEEST6B.kia
        
      ExcIEEEST6B : ExcIEEEST6B.klr
        
          ExcIEEEST6B --> PU : ExcIEEEST6B.klr
        
      ExcIEEEST6B : ExcIEEEST6B.km
        
          ExcIEEEST6B --> PU : ExcIEEEST6B.km
        
      ExcIEEEST6B : ExcIEEEST6B.kpa
        
          ExcIEEEST6B --> PU : ExcIEEEST6B.kpa
        
      ExcIEEEST6B : IdentifiedObject.mRID
        
      ExcIEEEST6B : IdentifiedObject.name
        
      ExcIEEEST6B : ExcIEEEST6B.oelin
        
          ExcIEEEST6B --> ExcST6BOELselectorKind : ExcIEEEST6B.oelin
        
      ExcIEEEST6B : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcIEEEST6B --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
      ExcIEEEST6B : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcIEEEST6B --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
      ExcIEEEST6B : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcIEEEST6B --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
      ExcIEEEST6B : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcIEEEST6B --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
      ExcIEEEST6B : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcIEEEST6B --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
        
      ExcIEEEST6B : ExcIEEEST6B.tg
        
          ExcIEEEST6B --> Seconds : ExcIEEEST6B.tg
        
      ExcIEEEST6B : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcIEEEST6B --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
      ExcIEEEST6B : ExcIEEEST6B.vamax
        
          ExcIEEEST6B --> PU : ExcIEEEST6B.vamax
        
      ExcIEEEST6B : ExcIEEEST6B.vamin
        
          ExcIEEEST6B --> PU : ExcIEEEST6B.vamin
        
      ExcIEEEST6B : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcIEEEST6B --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
      ExcIEEEST6B : ExcIEEEST6B.vrmax
        
          ExcIEEEST6B --> PU : ExcIEEEST6B.vrmax
        
      ExcIEEEST6B : ExcIEEEST6B.vrmin
        
          ExcIEEEST6B --> PU : ExcIEEEST6B.vrmin
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcIEEEST6B**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ilr | [cim:ExcIEEEST6B.ilr](http://iec.ch/TC57/CIM100#ExcIEEEST6B.ilr) | 1..1 <br />  [PU](PU.md)  | Exciter output current limit reference (<i>I</i><i><sub>LR</sub></i>) (&gt; 0... | direct |
| kci | [cim:ExcIEEEST6B.kci](http://iec.ch/TC57/CIM100#ExcIEEEST6B.kci) | 1..1 <br />  [PU](PU.md)  | Exciter output current limit adjustment (<i>K</i><i><sub>CI</sub></i>) (&gt; ... | direct |
| kff | [cim:ExcIEEEST6B.kff](http://iec.ch/TC57/CIM100#ExcIEEEST6B.kff) | 1..1 <br />  [PU](PU.md)  | Pre-control gain constant of the inner loop field regulator (<i>K</i><i><sub>... | direct |
| kg | [cim:ExcIEEEST6B.kg](http://iec.ch/TC57/CIM100#ExcIEEEST6B.kg) | 1..1 <br />  [PU](PU.md)  | Feedback gain constant of the inner loop field regulator (<i>K</i><i><sub>G</... | direct |
| kia | [cim:ExcIEEEST6B.kia](http://iec.ch/TC57/CIM100#ExcIEEEST6B.kia) | 1..1 <br />  [PU](PU.md)  | Voltage regulator integral gain (<i>K</i><i><sub>IA</sub></i>) (&gt; 0) | direct |
| klr | [cim:ExcIEEEST6B.klr](http://iec.ch/TC57/CIM100#ExcIEEEST6B.klr) | 1..1 <br />  [PU](PU.md)  | Exciter output current limiter gain (<i>K</i><i><sub>LR</sub></i>) (&gt; 0) | direct |
| km | [cim:ExcIEEEST6B.km](http://iec.ch/TC57/CIM100#ExcIEEEST6B.km) | 1..1 <br />  [PU](PU.md)  | Forward gain constant of the inner loop field regulator (<i>K</i><i><sub>M</s... | direct |
| kpa | [cim:ExcIEEEST6B.kpa](http://iec.ch/TC57/CIM100#ExcIEEEST6B.kpa) | 1..1 <br />  [PU](PU.md)  | Voltage regulator proportional gain (<u>K</u><u><sub>PA</sub></u>) (&gt; 0) | direct |
| oelin | [cim:ExcIEEEST6B.oelin](http://iec.ch/TC57/CIM100#ExcIEEEST6B.oelin) | 1..1 <br />  [ExcST6BOELselectorKind](ExcST6BOELselectorKind.md)  | OEL input selector (<i>OELin</i>) | direct |
| tg | [cim:ExcIEEEST6B.tg](http://iec.ch/TC57/CIM100#ExcIEEEST6B.tg) | 1..1 <br />  [Seconds](Seconds.md)  | Feedback time constant of inner loop field voltage regulator (<i>T</i><i><sub... | direct |
| vamax | [cim:ExcIEEEST6B.vamax](http://iec.ch/TC57/CIM100#ExcIEEEST6B.vamax) | 1..1 <br />  [PU](PU.md)  | Maximum voltage regulator output (V<i><sub>AMAX</sub></i>) (&gt; 0) | direct |
| vamin | [cim:ExcIEEEST6B.vamin](http://iec.ch/TC57/CIM100#ExcIEEEST6B.vamin) | 1..1 <br />  [PU](PU.md)  | Minimum voltage regulator output (<i>V</i><i><sub>AMIN</sub></i>) (&lt; 0) | direct |
| vrmax | [cim:ExcIEEEST6B.vrmax](http://iec.ch/TC57/CIM100#ExcIEEEST6B.vrmax) | 1..1 <br />  [PU](PU.md)  | Maximum voltage regulator output (<i>V</i><i><sub>RMAX</sub></i>) (&gt; 0) | direct |
| vrmin | [cim:ExcIEEEST6B.vrmin](http://iec.ch/TC57/CIM100#ExcIEEEST6B.vrmin) | 1..1 <br />  [PU](PU.md)  | Minimum voltage regulator output (<i>V</i><i><sub>RMIN</sub></i>) (&lt; 0) | direct |
| SynchronousMachineDynamics | [cim:ExcitationSystemDynamics.SynchronousMachineDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.SynchronousMachineDynamics) | 1..1 <br />  [SynchronousMachineDynamics](SynchronousMachineDynamics.md)  | Synchronous machine model with which this excitation system model is associat... | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| VoltageCompensatorDynamics | [cim:ExcitationSystemDynamics.VoltageCompensatorDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.VoltageCompensatorDynamics) | 1..1 <br />  [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md)  | Voltage compensator model associated with this excitation system model | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| OverexcitationLimiterDynamics | [cim:ExcitationSystemDynamics.OverexcitationLimiterDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.OverexcitationLimiterDynamics) | 0..1 <br />  [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md)  | Overexcitation limiter model associated with this excitation system model | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| PFVArControllerType2Dynamics | [cim:ExcitationSystemDynamics.PFVArControllerType2Dynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.PFVArControllerType2Dynamics) | 0..1 <br />  [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md)  | Power factor or VAr controller type 2 model associated with this excitation s... | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| DiscontinuousExcitationControlDynamics | [cim:ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics) | 0..1 <br />  [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md)  | Discontinuous excitation control model associated with this excitation system... | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| PowerSystemStabilizerDynamics | [cim:ExcitationSystemDynamics.PowerSystemStabilizerDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.PowerSystemStabilizerDynamics) | 0..1 <br />  [PowerSystemStabilizerDynamics](PowerSystemStabilizerDynamics.md)  | Power system stabilizer model associated with this excitation system model | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| UnderexcitationLimiterDynamics | [cim:ExcitationSystemDynamics.UnderexcitationLimiterDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.UnderexcitationLimiterDynamics) | 0..1 <br />  [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md)  | Undrexcitation limiter model associated with this excitation system model | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| PFVArControllerType1Dynamics | [cim:ExcitationSystemDynamics.PFVArControllerType1Dynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.PFVArControllerType1Dynamics) | 0..1 <br />  [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md)  | Power factor or VAr controller type 1 model associated with this excitation s... | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
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
| self | cim:ExcIEEEST6B |
| native | this:ExcIEEEST6B |




