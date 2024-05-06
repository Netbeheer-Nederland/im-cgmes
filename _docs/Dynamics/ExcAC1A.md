# ExcAC1A


_Modified IEEE AC1A alternator-supplied rectifier excitation system with different rate feedback source._





**URI**: [cim:ExcAC1A](http://iec.ch/TC57/CIM100#ExcAC1A)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcAC1A
    click ExcAC1A href "../ExcAC1A"
      ExcitationSystemDynamics <|-- ExcAC1A
        click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
      
      ExcAC1A : IdentifiedObject.description
        
      ExcAC1A : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcAC1A --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
          click DiscontinuousExcitationControlDynamics href "../DiscontinuousExcitationControlDynamics"
        
      ExcAC1A : DynamicsFunctionBlock.enabled
        
      ExcAC1A : ExcAC1A.hvlvgates
        
      ExcAC1A : ExcAC1A.ka
        
          ExcAC1A --> PU : ExcAC1A.ka
          click PU href "../PU"
        
      ExcAC1A : ExcAC1A.kc
        
          ExcAC1A --> PU : ExcAC1A.kc
          click PU href "../PU"
        
      ExcAC1A : ExcAC1A.kd
        
          ExcAC1A --> PU : ExcAC1A.kd
          click PU href "../PU"
        
      ExcAC1A : ExcAC1A.ke
        
          ExcAC1A --> PU : ExcAC1A.ke
          click PU href "../PU"
        
      ExcAC1A : ExcAC1A.kf
        
          ExcAC1A --> PU : ExcAC1A.kf
          click PU href "../PU"
        
      ExcAC1A : ExcAC1A.kf1
        
          ExcAC1A --> PU : ExcAC1A.kf1
          click PU href "../PU"
        
      ExcAC1A : ExcAC1A.kf2
        
          ExcAC1A --> PU : ExcAC1A.kf2
          click PU href "../PU"
        
      ExcAC1A : ExcAC1A.ks
        
          ExcAC1A --> PU : ExcAC1A.ks
          click PU href "../PU"
        
      ExcAC1A : IdentifiedObject.mRID
        
      ExcAC1A : IdentifiedObject.name
        
      ExcAC1A : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcAC1A --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
          click OverexcitationLimiterDynamics href "../OverexcitationLimiterDynamics"
        
      ExcAC1A : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcAC1A --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
          click PFVArControllerType1Dynamics href "../PFVArControllerType1Dynamics"
        
      ExcAC1A : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcAC1A --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
          click PFVArControllerType2Dynamics href "../PFVArControllerType2Dynamics"
        
      ExcAC1A : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcAC1A --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
          click PowerSystemStabilizerDynamics href "../PowerSystemStabilizerDynamics"
        
      ExcAC1A : ExcAC1A.seve1
        
      ExcAC1A : ExcAC1A.seve2
        
      ExcAC1A : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcAC1A --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
          click SynchronousMachineDynamics href "../SynchronousMachineDynamics"
        
      ExcAC1A : ExcAC1A.ta
        
          ExcAC1A --> Seconds : ExcAC1A.ta
          click Seconds href "../Seconds"
        
      ExcAC1A : ExcAC1A.tb
        
          ExcAC1A --> Seconds : ExcAC1A.tb
          click Seconds href "../Seconds"
        
      ExcAC1A : ExcAC1A.tc
        
          ExcAC1A --> Seconds : ExcAC1A.tc
          click Seconds href "../Seconds"
        
      ExcAC1A : ExcAC1A.te
        
          ExcAC1A --> Seconds : ExcAC1A.te
          click Seconds href "../Seconds"
        
      ExcAC1A : ExcAC1A.tf
        
          ExcAC1A --> Seconds : ExcAC1A.tf
          click Seconds href "../Seconds"
        
      ExcAC1A : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcAC1A --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
          click UnderexcitationLimiterDynamics href "../UnderexcitationLimiterDynamics"
        
      ExcAC1A : ExcAC1A.vamax
        
          ExcAC1A --> PU : ExcAC1A.vamax
          click PU href "../PU"
        
      ExcAC1A : ExcAC1A.vamin
        
          ExcAC1A --> PU : ExcAC1A.vamin
          click PU href "../PU"
        
      ExcAC1A : ExcAC1A.ve1
        
          ExcAC1A --> PU : ExcAC1A.ve1
          click PU href "../PU"
        
      ExcAC1A : ExcAC1A.ve2
        
          ExcAC1A --> PU : ExcAC1A.ve2
          click PU href "../PU"
        
      ExcAC1A : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcAC1A --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
          click VoltageCompensatorDynamics href "../VoltageCompensatorDynamics"
        
      ExcAC1A : ExcAC1A.vrmax
        
          ExcAC1A --> PU : ExcAC1A.vrmax
          click PU href "../PU"
        
      ExcAC1A : ExcAC1A.vrmin
        
          ExcAC1A --> PU : ExcAC1A.vrmin
          click PU href "../PU"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcAC1A**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| tb | [cim:ExcAC1A.tb](http://iec.ch/TC57/CIM100#ExcAC1A.tb) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tb</i>) (&gt;= 0) | direct |
| tc | [cim:ExcAC1A.tc](http://iec.ch/TC57/CIM100#ExcAC1A.tc) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>T</i><i><sub>c</sub></i>) (&gt;= 0) | direct |
| ka | [cim:ExcAC1A.ka](http://iec.ch/TC57/CIM100#ExcAC1A.ka) | 1 <br />  [PU](PU.md)  | Voltage regulator gain (<i>Ka</i>) (&gt; 0) | direct |
| ta | [cim:ExcAC1A.ta](http://iec.ch/TC57/CIM100#ExcAC1A.ta) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Ta</i>) (&gt; 0) | direct |
| vamax | [cim:ExcAC1A.vamax](http://iec.ch/TC57/CIM100#ExcAC1A.vamax) | 1 <br />  [PU](PU.md)  | Maximum voltage regulator output (<i>V</i><i><sub>amax</sub></i>) (&gt; 0) | direct |
| vamin | [cim:ExcAC1A.vamin](http://iec.ch/TC57/CIM100#ExcAC1A.vamin) | 1 <br />  [PU](PU.md)  | Minimum voltage regulator output (<i>V</i><i><sub>amin</sub></i>) (&lt; 0) | direct |
| te | [cim:ExcAC1A.te](http://iec.ch/TC57/CIM100#ExcAC1A.te) | 1 <br />  [Seconds](Seconds.md)  | Exciter time constant, integration rate associated with exciter control (<i>T... | direct |
| kf | [cim:ExcAC1A.kf](http://iec.ch/TC57/CIM100#ExcAC1A.kf) | 1 <br />  [PU](PU.md)  | Excitation control system stabilizer gains (<i>Kf</i>) (&gt;= 0) | direct |
| kf1 | [cim:ExcAC1A.kf1](http://iec.ch/TC57/CIM100#ExcAC1A.kf1) | 1 <br />  [PU](PU.md)  | Coefficient to allow different usage of the model (<i>Kf1</i>) (&gt;= 0) | direct |
| kf2 | [cim:ExcAC1A.kf2](http://iec.ch/TC57/CIM100#ExcAC1A.kf2) | 1 <br />  [PU](PU.md)  | Coefficient to allow different usage of the model (<i>Kf2</i>) (&gt;= 0) | direct |
| ks | [cim:ExcAC1A.ks](http://iec.ch/TC57/CIM100#ExcAC1A.ks) | 1 <br />  [PU](PU.md)  | Coefficient to allow different usage of the model-speed coefficient (<i>Ks</i... | direct |
| tf | [cim:ExcAC1A.tf](http://iec.ch/TC57/CIM100#ExcAC1A.tf) | 1 <br />  [Seconds](Seconds.md)  | Excitation control system stabilizer time constant (<i>Tf</i>) (&gt; 0) | direct |
| kc | [cim:ExcAC1A.kc](http://iec.ch/TC57/CIM100#ExcAC1A.kc) | 1 <br />  [PU](PU.md)  | Rectifier loading factor proportional to commutating reactance (<i>Kc</i>) (&... | direct |
| kd | [cim:ExcAC1A.kd](http://iec.ch/TC57/CIM100#ExcAC1A.kd) | 1 <br />  [PU](PU.md)  | Demagnetizing factor, a function of exciter alternator reactances (<i>Kd</i>)... | direct |
| ke | [cim:ExcAC1A.ke](http://iec.ch/TC57/CIM100#ExcAC1A.ke) | 1 <br />  [PU](PU.md)  | Exciter constant related to self-excited field (<i>Ke</i>) | direct |
| ve1 | [cim:ExcAC1A.ve1](http://iec.ch/TC57/CIM100#ExcAC1A.ve1) | 1 <br />  [PU](PU.md)  | Exciter alternator output voltages back of commutating reactance at which sat... | direct |
| seve1 | [cim:ExcAC1A.seve1](http://iec.ch/TC57/CIM100#ExcAC1A.seve1) | 1 <br />  float  | Exciter saturation function value at the corresponding exciter voltage, <i>Ve... | direct |
| ve2 | [cim:ExcAC1A.ve2](http://iec.ch/TC57/CIM100#ExcAC1A.ve2) | 1 <br />  [PU](PU.md)  | Exciter alternator output voltages back of commutating reactance at which sat... | direct |
| seve2 | [cim:ExcAC1A.seve2](http://iec.ch/TC57/CIM100#ExcAC1A.seve2) | 1 <br />  float  | Exciter saturation function value at the corresponding exciter voltage, <i>Ve... | direct |
| vrmax | [cim:ExcAC1A.vrmax](http://iec.ch/TC57/CIM100#ExcAC1A.vrmax) | 1 <br />  [PU](PU.md)  | Maximum voltage regulator outputs (<i>Vrmax</i>) (&gt; 0) | direct |
| vrmin | [cim:ExcAC1A.vrmin](http://iec.ch/TC57/CIM100#ExcAC1A.vrmin) | 1 <br />  [PU](PU.md)  | Minimum voltage regulator outputs (<i>Vrmin</i>) (&lt; 0) | direct |
| hvlvgates | [cim:ExcAC1A.hvlvgates](http://iec.ch/TC57/CIM100#ExcAC1A.hvlvgates) | 1 <br />  boolean  | Indicates if both HV gate and LV gate are active (<i>HVLVgates</i>) | direct |
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
| self | cim:ExcAC1A |
| native | this:ExcAC1A |




