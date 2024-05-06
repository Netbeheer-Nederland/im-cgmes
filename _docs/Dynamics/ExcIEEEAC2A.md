# ExcIEEEAC2A


_IEEE 421.5-2005 type AC2A model. The model represents a high initial response field-controlled alternator-rectifier excitation system. The alternator main exciter is used with non-controlled rectifiers. The type AC2A model is similar to that of type AC1A except for the inclusion of exciter time constant compensation and exciter field current limiting elements._

_Reference: IEEE 421.5-2005, 6.2._





**URI**: [cim:ExcIEEEAC2A](http://iec.ch/TC57/CIM100#ExcIEEEAC2A)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcIEEEAC2A
    click ExcIEEEAC2A href "../ExcIEEEAC2A"
      ExcitationSystemDynamics <|-- ExcIEEEAC2A
        click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
      
      ExcIEEEAC2A : IdentifiedObject.description
        
      ExcIEEEAC2A : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcIEEEAC2A --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
          click DiscontinuousExcitationControlDynamics href "../DiscontinuousExcitationControlDynamics"
        
      ExcIEEEAC2A : DynamicsFunctionBlock.enabled
        
      ExcIEEEAC2A : ExcIEEEAC2A.ka
        
          ExcIEEEAC2A --> PU : ExcIEEEAC2A.ka
          click PU href "../PU"
        
      ExcIEEEAC2A : ExcIEEEAC2A.kb
        
          ExcIEEEAC2A --> PU : ExcIEEEAC2A.kb
          click PU href "../PU"
        
      ExcIEEEAC2A : ExcIEEEAC2A.kc
        
          ExcIEEEAC2A --> PU : ExcIEEEAC2A.kc
          click PU href "../PU"
        
      ExcIEEEAC2A : ExcIEEEAC2A.kd
        
          ExcIEEEAC2A --> PU : ExcIEEEAC2A.kd
          click PU href "../PU"
        
      ExcIEEEAC2A : ExcIEEEAC2A.ke
        
          ExcIEEEAC2A --> PU : ExcIEEEAC2A.ke
          click PU href "../PU"
        
      ExcIEEEAC2A : ExcIEEEAC2A.kf
        
          ExcIEEEAC2A --> PU : ExcIEEEAC2A.kf
          click PU href "../PU"
        
      ExcIEEEAC2A : ExcIEEEAC2A.kh
        
          ExcIEEEAC2A --> PU : ExcIEEEAC2A.kh
          click PU href "../PU"
        
      ExcIEEEAC2A : IdentifiedObject.mRID
        
      ExcIEEEAC2A : IdentifiedObject.name
        
      ExcIEEEAC2A : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcIEEEAC2A --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
          click OverexcitationLimiterDynamics href "../OverexcitationLimiterDynamics"
        
      ExcIEEEAC2A : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcIEEEAC2A --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
          click PFVArControllerType1Dynamics href "../PFVArControllerType1Dynamics"
        
      ExcIEEEAC2A : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcIEEEAC2A --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
          click PFVArControllerType2Dynamics href "../PFVArControllerType2Dynamics"
        
      ExcIEEEAC2A : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcIEEEAC2A --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
          click PowerSystemStabilizerDynamics href "../PowerSystemStabilizerDynamics"
        
      ExcIEEEAC2A : ExcIEEEAC2A.seve1
        
      ExcIEEEAC2A : ExcIEEEAC2A.seve2
        
      ExcIEEEAC2A : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcIEEEAC2A --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
          click SynchronousMachineDynamics href "../SynchronousMachineDynamics"
        
      ExcIEEEAC2A : ExcIEEEAC2A.ta
        
          ExcIEEEAC2A --> Seconds : ExcIEEEAC2A.ta
          click Seconds href "../Seconds"
        
      ExcIEEEAC2A : ExcIEEEAC2A.tb
        
          ExcIEEEAC2A --> Seconds : ExcIEEEAC2A.tb
          click Seconds href "../Seconds"
        
      ExcIEEEAC2A : ExcIEEEAC2A.tc
        
          ExcIEEEAC2A --> Seconds : ExcIEEEAC2A.tc
          click Seconds href "../Seconds"
        
      ExcIEEEAC2A : ExcIEEEAC2A.te
        
          ExcIEEEAC2A --> Seconds : ExcIEEEAC2A.te
          click Seconds href "../Seconds"
        
      ExcIEEEAC2A : ExcIEEEAC2A.tf
        
          ExcIEEEAC2A --> Seconds : ExcIEEEAC2A.tf
          click Seconds href "../Seconds"
        
      ExcIEEEAC2A : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcIEEEAC2A --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
          click UnderexcitationLimiterDynamics href "../UnderexcitationLimiterDynamics"
        
      ExcIEEEAC2A : ExcIEEEAC2A.vamax
        
          ExcIEEEAC2A --> PU : ExcIEEEAC2A.vamax
          click PU href "../PU"
        
      ExcIEEEAC2A : ExcIEEEAC2A.vamin
        
          ExcIEEEAC2A --> PU : ExcIEEEAC2A.vamin
          click PU href "../PU"
        
      ExcIEEEAC2A : ExcIEEEAC2A.ve1
        
          ExcIEEEAC2A --> PU : ExcIEEEAC2A.ve1
          click PU href "../PU"
        
      ExcIEEEAC2A : ExcIEEEAC2A.ve2
        
          ExcIEEEAC2A --> PU : ExcIEEEAC2A.ve2
          click PU href "../PU"
        
      ExcIEEEAC2A : ExcIEEEAC2A.vfemax
        
          ExcIEEEAC2A --> PU : ExcIEEEAC2A.vfemax
          click PU href "../PU"
        
      ExcIEEEAC2A : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcIEEEAC2A --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
          click VoltageCompensatorDynamics href "../VoltageCompensatorDynamics"
        
      ExcIEEEAC2A : ExcIEEEAC2A.vrmax
        
          ExcIEEEAC2A --> PU : ExcIEEEAC2A.vrmax
          click PU href "../PU"
        
      ExcIEEEAC2A : ExcIEEEAC2A.vrmin
        
          ExcIEEEAC2A --> PU : ExcIEEEAC2A.vrmin
          click PU href "../PU"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcIEEEAC2A**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| tb | [cim:ExcIEEEAC2A.tb](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.tb) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>T</i><i><sub>B</sub></i>) (&gt;= 0) | direct |
| tc | [cim:ExcIEEEAC2A.tc](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.tc) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>T</i><i><sub>C</sub></i>) (&gt;= 0) | direct |
| ka | [cim:ExcIEEEAC2A.ka](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.ka) | 1 <br />  [PU](PU.md)  | Voltage regulator gain (<i>K</i><i><sub>A</sub></i>) (&gt; 0) | direct |
| ta | [cim:ExcIEEEAC2A.ta](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.ta) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>T</i><i><sub>A</sub></i>) (&gt; 0) | direct |
| vamax | [cim:ExcIEEEAC2A.vamax](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.vamax) | 1 <br />  [PU](PU.md)  | Maximum voltage regulator output (<i>V</i><i><sub>AMAX</sub></i>) (&gt; 0) | direct |
| vamin | [cim:ExcIEEEAC2A.vamin](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.vamin) | 1 <br />  [PU](PU.md)  | Minimum voltage regulator output (<i>V</i><i><sub>AMIN</sub></i>) (&lt; 0) | direct |
| kb | [cim:ExcIEEEAC2A.kb](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.kb) | 1 <br />  [PU](PU.md)  | Second stage regulator gain (<i>K</i><i><sub>B</sub></i>) (&gt; 0) | direct |
| vrmax | [cim:ExcIEEEAC2A.vrmax](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.vrmax) | 1 <br />  [PU](PU.md)  | Maximum voltage regulator outputs (<i>V</i><i><sub>RMAX</sub></i>) (&gt; 0) | direct |
| vrmin | [cim:ExcIEEEAC2A.vrmin](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.vrmin) | 1 <br />  [PU](PU.md)  | Minimum voltage regulator outputs (<i>V</i><i><sub>RMIN</sub></i>) (&lt; 0) | direct |
| te | [cim:ExcIEEEAC2A.te](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.te) | 1 <br />  [Seconds](Seconds.md)  | Exciter time constant, integration rate associated with exciter control (<i>T... | direct |
| vfemax | [cim:ExcIEEEAC2A.vfemax](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.vfemax) | 1 <br />  [PU](PU.md)  | Exciter field current limit reference (<i>V</i><i><sub>FEMAX</sub></i>) (&gt;... | direct |
| kh | [cim:ExcIEEEAC2A.kh](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.kh) | 1 <br />  [PU](PU.md)  | Exciter field current feedback gain (<i>K</i><i><sub>H</sub></i>) (&gt;= 0) | direct |
| kf | [cim:ExcIEEEAC2A.kf](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.kf) | 1 <br />  [PU](PU.md)  | Excitation control system stabilizer gains (<i>K</i><i><sub>F</sub></i>) (&gt... | direct |
| tf | [cim:ExcIEEEAC2A.tf](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.tf) | 1 <br />  [Seconds](Seconds.md)  | Excitation control system stabilizer time constant (<i>T</i><i><sub>F</sub></... | direct |
| kc | [cim:ExcIEEEAC2A.kc](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.kc) | 1 <br />  [PU](PU.md)  | Rectifier loading factor proportional to commutating reactance (<i>K</i><i><s... | direct |
| kd | [cim:ExcIEEEAC2A.kd](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.kd) | 1 <br />  [PU](PU.md)  | Demagnetizing factor, a function of exciter alternator reactances (<i>K</i><i... | direct |
| ke | [cim:ExcIEEEAC2A.ke](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.ke) | 1 <br />  [PU](PU.md)  | Exciter constant related to self-excited field (<i>K</i><i><sub>E</sub></i>) ... | direct |
| ve1 | [cim:ExcIEEEAC2A.ve1](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.ve1) | 1 <br />  [PU](PU.md)  | Exciter alternator output voltages back of commutating reactance at which sat... | direct |
| seve1 | [cim:ExcIEEEAC2A.seve1](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.seve1) | 1 <br />  float  | Exciter saturation function value at the corresponding exciter voltage, <i>V<... | direct |
| ve2 | [cim:ExcIEEEAC2A.ve2](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.ve2) | 1 <br />  [PU](PU.md)  | Exciter alternator output voltages back of commutating reactance at which sat... | direct |
| seve2 | [cim:ExcIEEEAC2A.seve2](http://iec.ch/TC57/CIM100#ExcIEEEAC2A.seve2) | 1 <br />  float  | Exciter saturation function value at the corresponding exciter voltage, <i>V<... | direct |
| SynchronousMachineDynamics | [cim:ExcitationSystemDynamics.SynchronousMachineDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.SynchronousMachineDynamics) | 1 <br />  [SynchronousMachineDynamics](SynchronousMachineDynamics.md)  | Synchronous machine model with which this excitation system model is associat... | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| VoltageCompensatorDynamics | [cim:ExcitationSystemDynamics.VoltageCompensatorDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.VoltageCompensatorDynamics) | 1 <br />  [VoltageCompensatorDynamics](VoltageCompensatorDynamics.md)  | Voltage compensator model associated with this excitation system model | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| OverexcitationLimiterDynamics | [cim:ExcitationSystemDynamics.OverexcitationLimiterDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.OverexcitationLimiterDynamics) | 0..1 <br />  [OverexcitationLimiterDynamics](OverexcitationLimiterDynamics.md)  | Overexcitation limiter model associated with this excitation system model | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| PFVArControllerType2Dynamics | [cim:ExcitationSystemDynamics.PFVArControllerType2Dynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.PFVArControllerType2Dynamics) | 0..1 <br />  [PFVArControllerType2Dynamics](PFVArControllerType2Dynamics.md)  | Power factor or VAr controller type 2 model associated with this excitation s... | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| DiscontinuousExcitationControlDynamics | [cim:ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics) | 0..1 <br />  [DiscontinuousExcitationControlDynamics](DiscontinuousExcitationControlDynamics.md)  | Discontinuous excitation control model associated with this excitation system... | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| PowerSystemStabilizerDynamics | [cim:ExcitationSystemDynamics.PowerSystemStabilizerDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.PowerSystemStabilizerDynamics) | 0..1 <br />  [PowerSystemStabilizerDynamics](PowerSystemStabilizerDynamics.md)  | Power system stabilizer model associated with this excitation system model | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| UnderexcitationLimiterDynamics | [cim:ExcitationSystemDynamics.UnderexcitationLimiterDynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.UnderexcitationLimiterDynamics) | 0..1 <br />  [UnderexcitationLimiterDynamics](UnderexcitationLimiterDynamics.md)  | Undrexcitation limiter model associated with this excitation system model | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
| PFVArControllerType1Dynamics | [cim:ExcitationSystemDynamics.PFVArControllerType1Dynamics](http://iec.ch/TC57/CIM100#ExcitationSystemDynamics.PFVArControllerType1Dynamics) | 0..1 <br />  [PFVArControllerType1Dynamics](PFVArControllerType1Dynamics.md)  | Power factor or VAr controller type 1 model associated with this excitation s... | [ExcitationSystemDynamics](ExcitationSystemDynamics.md) |
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
| self | cim:ExcIEEEAC2A |
| native | this:ExcIEEEAC2A |




