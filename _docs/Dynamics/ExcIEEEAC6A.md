# ExcIEEEAC6A


_IEEE 421.5-2005 type AC6A model. The model represents field-controlled alternator-rectifier excitation systems with system-supplied electronic voltage regulators.  The maximum output of the regulator, <i>V</i><i><sub>R</sub></i>, is a function of terminal voltage, <i>V</i><i><sub>T</sub></i>. The field current limiter included in the original model AC6A remains in the 2005 update._

_Reference: IEEE 421.5-2005, 6.6._





**URI**: [cim:ExcIEEEAC6A](http://iec.ch/TC57/CIM100#ExcIEEEAC6A)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcIEEEAC6A
    click ExcIEEEAC6A href "../ExcIEEEAC6A"
      ExcitationSystemDynamics <|-- ExcIEEEAC6A
        click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
      
      ExcIEEEAC6A : IdentifiedObject.description
        
      ExcIEEEAC6A : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcIEEEAC6A --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
          click DiscontinuousExcitationControlDynamics href "../DiscontinuousExcitationControlDynamics"
        
      ExcIEEEAC6A : DynamicsFunctionBlock.enabled
        
      ExcIEEEAC6A : ExcIEEEAC6A.ka
        
          ExcIEEEAC6A --> PU : ExcIEEEAC6A.ka
          click PU href "../PU"
        
      ExcIEEEAC6A : ExcIEEEAC6A.kc
        
          ExcIEEEAC6A --> PU : ExcIEEEAC6A.kc
          click PU href "../PU"
        
      ExcIEEEAC6A : ExcIEEEAC6A.kd
        
          ExcIEEEAC6A --> PU : ExcIEEEAC6A.kd
          click PU href "../PU"
        
      ExcIEEEAC6A : ExcIEEEAC6A.ke
        
          ExcIEEEAC6A --> PU : ExcIEEEAC6A.ke
          click PU href "../PU"
        
      ExcIEEEAC6A : ExcIEEEAC6A.kh
        
          ExcIEEEAC6A --> PU : ExcIEEEAC6A.kh
          click PU href "../PU"
        
      ExcIEEEAC6A : IdentifiedObject.mRID
        
      ExcIEEEAC6A : IdentifiedObject.name
        
      ExcIEEEAC6A : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcIEEEAC6A --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
          click OverexcitationLimiterDynamics href "../OverexcitationLimiterDynamics"
        
      ExcIEEEAC6A : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcIEEEAC6A --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
          click PFVArControllerType1Dynamics href "../PFVArControllerType1Dynamics"
        
      ExcIEEEAC6A : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcIEEEAC6A --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
          click PFVArControllerType2Dynamics href "../PFVArControllerType2Dynamics"
        
      ExcIEEEAC6A : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcIEEEAC6A --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
          click PowerSystemStabilizerDynamics href "../PowerSystemStabilizerDynamics"
        
      ExcIEEEAC6A : ExcIEEEAC6A.seve1
        
      ExcIEEEAC6A : ExcIEEEAC6A.seve2
        
      ExcIEEEAC6A : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcIEEEAC6A --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
          click SynchronousMachineDynamics href "../SynchronousMachineDynamics"
        
      ExcIEEEAC6A : ExcIEEEAC6A.ta
        
          ExcIEEEAC6A --> Seconds : ExcIEEEAC6A.ta
          click Seconds href "../Seconds"
        
      ExcIEEEAC6A : ExcIEEEAC6A.tb
        
          ExcIEEEAC6A --> Seconds : ExcIEEEAC6A.tb
          click Seconds href "../Seconds"
        
      ExcIEEEAC6A : ExcIEEEAC6A.tc
        
          ExcIEEEAC6A --> Seconds : ExcIEEEAC6A.tc
          click Seconds href "../Seconds"
        
      ExcIEEEAC6A : ExcIEEEAC6A.te
        
          ExcIEEEAC6A --> Seconds : ExcIEEEAC6A.te
          click Seconds href "../Seconds"
        
      ExcIEEEAC6A : ExcIEEEAC6A.th
        
          ExcIEEEAC6A --> Seconds : ExcIEEEAC6A.th
          click Seconds href "../Seconds"
        
      ExcIEEEAC6A : ExcIEEEAC6A.tj
        
          ExcIEEEAC6A --> Seconds : ExcIEEEAC6A.tj
          click Seconds href "../Seconds"
        
      ExcIEEEAC6A : ExcIEEEAC6A.tk
        
          ExcIEEEAC6A --> Seconds : ExcIEEEAC6A.tk
          click Seconds href "../Seconds"
        
      ExcIEEEAC6A : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcIEEEAC6A --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
          click UnderexcitationLimiterDynamics href "../UnderexcitationLimiterDynamics"
        
      ExcIEEEAC6A : ExcIEEEAC6A.vamax
        
          ExcIEEEAC6A --> PU : ExcIEEEAC6A.vamax
          click PU href "../PU"
        
      ExcIEEEAC6A : ExcIEEEAC6A.vamin
        
          ExcIEEEAC6A --> PU : ExcIEEEAC6A.vamin
          click PU href "../PU"
        
      ExcIEEEAC6A : ExcIEEEAC6A.ve1
        
          ExcIEEEAC6A --> PU : ExcIEEEAC6A.ve1
          click PU href "../PU"
        
      ExcIEEEAC6A : ExcIEEEAC6A.ve2
        
          ExcIEEEAC6A --> PU : ExcIEEEAC6A.ve2
          click PU href "../PU"
        
      ExcIEEEAC6A : ExcIEEEAC6A.vfelim
        
          ExcIEEEAC6A --> PU : ExcIEEEAC6A.vfelim
          click PU href "../PU"
        
      ExcIEEEAC6A : ExcIEEEAC6A.vhmax
        
          ExcIEEEAC6A --> PU : ExcIEEEAC6A.vhmax
          click PU href "../PU"
        
      ExcIEEEAC6A : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcIEEEAC6A --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
          click VoltageCompensatorDynamics href "../VoltageCompensatorDynamics"
        
      ExcIEEEAC6A : ExcIEEEAC6A.vrmax
        
          ExcIEEEAC6A --> PU : ExcIEEEAC6A.vrmax
          click PU href "../PU"
        
      ExcIEEEAC6A : ExcIEEEAC6A.vrmin
        
          ExcIEEEAC6A --> PU : ExcIEEEAC6A.vrmin
          click PU href "../PU"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcIEEEAC6A**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ka | [cim:ExcIEEEAC6A.ka](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.ka) | 1 <br />  [PU](PU.md)  | Voltage regulator gain (<i>K</i><i><sub>A</sub></i>) (&gt; 0) | direct |
| ta | [cim:ExcIEEEAC6A.ta](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.ta) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>T</i><i><sub>A</sub></i>) (&gt;= 0) | direct |
| tk | [cim:ExcIEEEAC6A.tk](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.tk) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>T</i><i><sub>K</sub></i>) (&gt;= 0) | direct |
| tb | [cim:ExcIEEEAC6A.tb](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.tb) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>T</i><i><sub>B</sub></i>) (&gt;= 0) | direct |
| tc | [cim:ExcIEEEAC6A.tc](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.tc) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>T</i><i><sub>C</sub></i>) (&gt;= 0) | direct |
| vamax | [cim:ExcIEEEAC6A.vamax](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.vamax) | 1 <br />  [PU](PU.md)  | Maximum voltage regulator output (<i>V</i><i><sub>AMAX</sub></i>) (&gt; 0) | direct |
| vamin | [cim:ExcIEEEAC6A.vamin](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.vamin) | 1 <br />  [PU](PU.md)  | Minimum voltage regulator output (V<sub>AMIN</sub>) (&lt; 0) | direct |
| vrmax | [cim:ExcIEEEAC6A.vrmax](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.vrmax) | 1 <br />  [PU](PU.md)  | Maximum voltage regulator output (<i>V</i><i><sub>RMAX</sub></i>) (&gt; 0) | direct |
| vrmin | [cim:ExcIEEEAC6A.vrmin](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.vrmin) | 1 <br />  [PU](PU.md)  | Minimum voltage regulator output (<i>V</i><i><sub>RMIN</sub></i>) (&lt; 0) | direct |
| te | [cim:ExcIEEEAC6A.te](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.te) | 1 <br />  [Seconds](Seconds.md)  | Exciter time constant, integration rate associated with exciter control (<i>T... | direct |
| kh | [cim:ExcIEEEAC6A.kh](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.kh) | 1 <br />  [PU](PU.md)  | Exciter field current limiter gain (<i>K</i><i><sub>H</sub></i>) (&gt;= 0) | direct |
| tj | [cim:ExcIEEEAC6A.tj](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.tj) | 1 <br />  [Seconds](Seconds.md)  | Exciter field current limiter time constant (<i>T</i><i><sub>J</sub></i>) (&g... | direct |
| th | [cim:ExcIEEEAC6A.th](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.th) | 1 <br />  [Seconds](Seconds.md)  | Exciter field current limiter time constant (<i>T</i><i><sub>H</sub></i>) (&g... | direct |
| vfelim | [cim:ExcIEEEAC6A.vfelim](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.vfelim) | 1 <br />  [PU](PU.md)  | Exciter field current limit reference (<i>V</i><i><sub>FELIM</sub></i>) (&gt;... | direct |
| vhmax | [cim:ExcIEEEAC6A.vhmax](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.vhmax) | 1 <br />  [PU](PU.md)  | Maximum field current limiter signal reference (<i>V</i><i><sub>HMAX</sub></i... | direct |
| kc | [cim:ExcIEEEAC6A.kc](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.kc) | 1 <br />  [PU](PU.md)  | Rectifier loading factor proportional to commutating reactance (<i>K</i><i><s... | direct |
| kd | [cim:ExcIEEEAC6A.kd](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.kd) | 1 <br />  [PU](PU.md)  | Demagnetizing factor, a function of exciter alternator reactances (<i>K</i><i... | direct |
| ke | [cim:ExcIEEEAC6A.ke](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.ke) | 1 <br />  [PU](PU.md)  | Exciter constant related to self-excited field (<i>K</i><i><sub>E</sub></i>) | direct |
| ve1 | [cim:ExcIEEEAC6A.ve1](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.ve1) | 1 <br />  [PU](PU.md)  | Exciter alternator output voltages back of commutating reactance at which sat... | direct |
| seve1 | [cim:ExcIEEEAC6A.seve1](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.seve1) | 1 <br />  float  | Exciter saturation function value at the corresponding exciter voltage, <i>V<... | direct |
| ve2 | [cim:ExcIEEEAC6A.ve2](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.ve2) | 1 <br />  [PU](PU.md)  | Exciter alternator output voltages back of commutating reactance at which sat... | direct |
| seve2 | [cim:ExcIEEEAC6A.seve2](http://iec.ch/TC57/CIM100#ExcIEEEAC6A.seve2) | 1 <br />  float  | Exciter saturation function value at the corresponding exciter voltage, <i>V<... | direct |
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
| self | cim:ExcIEEEAC6A |
| native | this:ExcIEEEAC6A |




