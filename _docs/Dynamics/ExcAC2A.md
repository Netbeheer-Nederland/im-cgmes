# ExcAC2A


_Modified IEEE AC2A alternator-supplied rectifier excitation system with different field current limit._





**URI**: [cim:ExcAC2A](http://iec.ch/TC57/CIM100#ExcAC2A)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcAC2A
    click ExcAC2A href "../ExcAC2A"
      ExcitationSystemDynamics <|-- ExcAC2A
        click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
      
      ExcAC2A : IdentifiedObject.description
        
      ExcAC2A : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcAC2A --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
          click DiscontinuousExcitationControlDynamics href "../DiscontinuousExcitationControlDynamics"
        
      ExcAC2A : DynamicsFunctionBlock.enabled
        
      ExcAC2A : ExcAC2A.hvgate
        
      ExcAC2A : ExcAC2A.ka
        
          ExcAC2A --> PU : ExcAC2A.ka
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.kb
        
          ExcAC2A --> PU : ExcAC2A.kb
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.kb1
        
          ExcAC2A --> PU : ExcAC2A.kb1
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.kc
        
          ExcAC2A --> PU : ExcAC2A.kc
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.kd
        
          ExcAC2A --> PU : ExcAC2A.kd
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.ke
        
          ExcAC2A --> PU : ExcAC2A.ke
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.kf
        
          ExcAC2A --> PU : ExcAC2A.kf
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.kh
        
          ExcAC2A --> PU : ExcAC2A.kh
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.kl
        
          ExcAC2A --> PU : ExcAC2A.kl
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.kl1
        
          ExcAC2A --> PU : ExcAC2A.kl1
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.ks
        
          ExcAC2A --> PU : ExcAC2A.ks
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.lvgate
        
      ExcAC2A : IdentifiedObject.mRID
        
      ExcAC2A : IdentifiedObject.name
        
      ExcAC2A : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcAC2A --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
          click OverexcitationLimiterDynamics href "../OverexcitationLimiterDynamics"
        
      ExcAC2A : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcAC2A --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
          click PFVArControllerType1Dynamics href "../PFVArControllerType1Dynamics"
        
      ExcAC2A : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcAC2A --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
          click PFVArControllerType2Dynamics href "../PFVArControllerType2Dynamics"
        
      ExcAC2A : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcAC2A --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
          click PowerSystemStabilizerDynamics href "../PowerSystemStabilizerDynamics"
        
      ExcAC2A : ExcAC2A.seve1
        
      ExcAC2A : ExcAC2A.seve2
        
      ExcAC2A : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcAC2A --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
          click SynchronousMachineDynamics href "../SynchronousMachineDynamics"
        
      ExcAC2A : ExcAC2A.ta
        
          ExcAC2A --> Seconds : ExcAC2A.ta
          click Seconds href "../Seconds"
        
      ExcAC2A : ExcAC2A.tb
        
          ExcAC2A --> Seconds : ExcAC2A.tb
          click Seconds href "../Seconds"
        
      ExcAC2A : ExcAC2A.tc
        
          ExcAC2A --> Seconds : ExcAC2A.tc
          click Seconds href "../Seconds"
        
      ExcAC2A : ExcAC2A.te
        
          ExcAC2A --> Seconds : ExcAC2A.te
          click Seconds href "../Seconds"
        
      ExcAC2A : ExcAC2A.tf
        
          ExcAC2A --> Seconds : ExcAC2A.tf
          click Seconds href "../Seconds"
        
      ExcAC2A : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcAC2A --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
          click UnderexcitationLimiterDynamics href "../UnderexcitationLimiterDynamics"
        
      ExcAC2A : ExcAC2A.vamax
        
          ExcAC2A --> PU : ExcAC2A.vamax
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.vamin
        
          ExcAC2A --> PU : ExcAC2A.vamin
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.ve1
        
          ExcAC2A --> PU : ExcAC2A.ve1
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.ve2
        
          ExcAC2A --> PU : ExcAC2A.ve2
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.vfemax
        
          ExcAC2A --> PU : ExcAC2A.vfemax
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.vlr
        
          ExcAC2A --> PU : ExcAC2A.vlr
          click PU href "../PU"
        
      ExcAC2A : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcAC2A --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
          click VoltageCompensatorDynamics href "../VoltageCompensatorDynamics"
        
      ExcAC2A : ExcAC2A.vrmax
        
          ExcAC2A --> PU : ExcAC2A.vrmax
          click PU href "../PU"
        
      ExcAC2A : ExcAC2A.vrmin
        
          ExcAC2A --> PU : ExcAC2A.vrmin
          click PU href "../PU"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcAC2A**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| tb | [cim:ExcAC2A.tb](http://iec.ch/TC57/CIM100#ExcAC2A.tb) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tb</i>) (&gt;= 0) | direct |
| tc | [cim:ExcAC2A.tc](http://iec.ch/TC57/CIM100#ExcAC2A.tc) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tc</i>) (&gt;= 0) | direct |
| ka | [cim:ExcAC2A.ka](http://iec.ch/TC57/CIM100#ExcAC2A.ka) | 1 <br />  [PU](PU.md)  | Voltage regulator gain (<i>Ka</i>) (&gt; 0) | direct |
| ta | [cim:ExcAC2A.ta](http://iec.ch/TC57/CIM100#ExcAC2A.ta) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Ta</i>) (&gt; 0) | direct |
| vamax | [cim:ExcAC2A.vamax](http://iec.ch/TC57/CIM100#ExcAC2A.vamax) | 1 <br />  [PU](PU.md)  | Maximum voltage regulator output (<i>Vamax</i>) (&gt; 0) | direct |
| vamin | [cim:ExcAC2A.vamin](http://iec.ch/TC57/CIM100#ExcAC2A.vamin) | 1 <br />  [PU](PU.md)  | Minimum voltage regulator output (<i>Vamin</i>) (&lt; 0) | direct |
| kb | [cim:ExcAC2A.kb](http://iec.ch/TC57/CIM100#ExcAC2A.kb) | 1 <br />  [PU](PU.md)  | Second stage regulator gain (<i>Kb</i>) (&gt; 0) | direct |
| kb1 | [cim:ExcAC2A.kb1](http://iec.ch/TC57/CIM100#ExcAC2A.kb1) | 1 <br />  [PU](PU.md)  | Second stage regulator gain (<i>Kb1</i>) | direct |
| vrmax | [cim:ExcAC2A.vrmax](http://iec.ch/TC57/CIM100#ExcAC2A.vrmax) | 1 <br />  [PU](PU.md)  | Maximum voltage regulator outputs (<i>Vrmax</i>) (&gt; 0) | direct |
| vrmin | [cim:ExcAC2A.vrmin](http://iec.ch/TC57/CIM100#ExcAC2A.vrmin) | 1 <br />  [PU](PU.md)  | Minimum voltage regulator outputs (<i>Vrmin</i>) (&lt; 0) | direct |
| te | [cim:ExcAC2A.te](http://iec.ch/TC57/CIM100#ExcAC2A.te) | 1 <br />  [Seconds](Seconds.md)  | Exciter time constant, integration rate associated with exciter control (<i>T... | direct |
| vfemax | [cim:ExcAC2A.vfemax](http://iec.ch/TC57/CIM100#ExcAC2A.vfemax) | 1 <br />  [PU](PU.md)  | Exciter field current limit reference (<i>Vfemax</i>) (&gt;= 0) | direct |
| kh | [cim:ExcAC2A.kh](http://iec.ch/TC57/CIM100#ExcAC2A.kh) | 1 <br />  [PU](PU.md)  | Exciter field current feedback gain (<i>Kh</i>) (&gt;= 0) | direct |
| kf | [cim:ExcAC2A.kf](http://iec.ch/TC57/CIM100#ExcAC2A.kf) | 1 <br />  [PU](PU.md)  | Excitation control system stabilizer gains (<i>Kf</i>) (&gt;= 0) | direct |
| kl | [cim:ExcAC2A.kl](http://iec.ch/TC57/CIM100#ExcAC2A.kl) | 1 <br />  [PU](PU.md)  | Exciter field current limiter gain (<i>Kl</i>) | direct |
| vlr | [cim:ExcAC2A.vlr](http://iec.ch/TC57/CIM100#ExcAC2A.vlr) | 1 <br />  [PU](PU.md)  | Maximum exciter field current (<i>Vlr</i>) (&gt; 0) | direct |
| kl1 | [cim:ExcAC2A.kl1](http://iec.ch/TC57/CIM100#ExcAC2A.kl1) | 1 <br />  [PU](PU.md)  | Coefficient to allow different usage of the model (<i>Kl1</i>) | direct |
| ks | [cim:ExcAC2A.ks](http://iec.ch/TC57/CIM100#ExcAC2A.ks) | 1 <br />  [PU](PU.md)  | Coefficient to allow different usage of the model-speed coefficient (<i>Ks</i... | direct |
| tf | [cim:ExcAC2A.tf](http://iec.ch/TC57/CIM100#ExcAC2A.tf) | 1 <br />  [Seconds](Seconds.md)  | Excitation control system stabilizer time constant (<i>Tf</i>) (&gt; 0) | direct |
| kc | [cim:ExcAC2A.kc](http://iec.ch/TC57/CIM100#ExcAC2A.kc) | 1 <br />  [PU](PU.md)  | Rectifier loading factor proportional to commutating reactance (<i>Kc</i>) (&... | direct |
| kd | [cim:ExcAC2A.kd](http://iec.ch/TC57/CIM100#ExcAC2A.kd) | 1 <br />  [PU](PU.md)  | Demagnetizing factor, a function of exciter alternator reactances (<i>Kd</i>)... | direct |
| ke | [cim:ExcAC2A.ke](http://iec.ch/TC57/CIM100#ExcAC2A.ke) | 1 <br />  [PU](PU.md)  | Exciter constant related to self-excited field (<i>Ke</i>) | direct |
| ve1 | [cim:ExcAC2A.ve1](http://iec.ch/TC57/CIM100#ExcAC2A.ve1) | 1 <br />  [PU](PU.md)  | Exciter alternator output voltages back of commutating reactance at which sat... | direct |
| seve1 | [cim:ExcAC2A.seve1](http://iec.ch/TC57/CIM100#ExcAC2A.seve1) | 1 <br />  float  | Exciter saturation function value at the corresponding exciter voltage, <i>Ve... | direct |
| ve2 | [cim:ExcAC2A.ve2](http://iec.ch/TC57/CIM100#ExcAC2A.ve2) | 1 <br />  [PU](PU.md)  | Exciter alternator output voltages back of commutating reactance at which sat... | direct |
| seve2 | [cim:ExcAC2A.seve2](http://iec.ch/TC57/CIM100#ExcAC2A.seve2) | 1 <br />  float  | Exciter saturation function value at the corresponding exciter voltage, <i>Ve... | direct |
| hvgate | [cim:ExcAC2A.hvgate](http://iec.ch/TC57/CIM100#ExcAC2A.hvgate) | 1 <br />  boolean  | Indicates if HV gate is active (<i>HVgate</i>) | direct |
| lvgate | [cim:ExcAC2A.lvgate](http://iec.ch/TC57/CIM100#ExcAC2A.lvgate) | 1 <br />  boolean  | Indicates if LV gate is active (<i>LVgate</i>) | direct |
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
| self | cim:ExcAC2A |
| native | this:ExcAC2A |




