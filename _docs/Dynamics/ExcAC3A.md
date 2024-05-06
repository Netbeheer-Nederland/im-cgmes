# ExcAC3A


_Modified IEEE AC3A alternator-supplied rectifier excitation system with different field current limit._





**URI**: [cim:ExcAC3A](http://iec.ch/TC57/CIM100#ExcAC3A)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcAC3A
    click ExcAC3A href "../ExcAC3A"
      ExcitationSystemDynamics <|-- ExcAC3A
        click ExcitationSystemDynamics href "../ExcitationSystemDynamics"
      
      ExcAC3A : IdentifiedObject.description
        
      ExcAC3A : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcAC3A --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
          click DiscontinuousExcitationControlDynamics href "../DiscontinuousExcitationControlDynamics"
        
      ExcAC3A : ExcAC3A.efdn
        
          ExcAC3A --> PU : ExcAC3A.efdn
          click PU href "../PU"
        
      ExcAC3A : DynamicsFunctionBlock.enabled
        
      ExcAC3A : ExcAC3A.ka
        
          ExcAC3A --> Seconds : ExcAC3A.ka
          click Seconds href "../Seconds"
        
      ExcAC3A : ExcAC3A.kc
        
          ExcAC3A --> PU : ExcAC3A.kc
          click PU href "../PU"
        
      ExcAC3A : ExcAC3A.kd
        
          ExcAC3A --> PU : ExcAC3A.kd
          click PU href "../PU"
        
      ExcAC3A : ExcAC3A.ke
        
          ExcAC3A --> PU : ExcAC3A.ke
          click PU href "../PU"
        
      ExcAC3A : ExcAC3A.kf
        
          ExcAC3A --> PU : ExcAC3A.kf
          click PU href "../PU"
        
      ExcAC3A : ExcAC3A.kf1
        
          ExcAC3A --> PU : ExcAC3A.kf1
          click PU href "../PU"
        
      ExcAC3A : ExcAC3A.kf2
        
          ExcAC3A --> PU : ExcAC3A.kf2
          click PU href "../PU"
        
      ExcAC3A : ExcAC3A.klv
        
          ExcAC3A --> PU : ExcAC3A.klv
          click PU href "../PU"
        
      ExcAC3A : ExcAC3A.kn
        
          ExcAC3A --> PU : ExcAC3A.kn
          click PU href "../PU"
        
      ExcAC3A : ExcAC3A.kr
        
          ExcAC3A --> PU : ExcAC3A.kr
          click PU href "../PU"
        
      ExcAC3A : ExcAC3A.ks
        
          ExcAC3A --> PU : ExcAC3A.ks
          click PU href "../PU"
        
      ExcAC3A : IdentifiedObject.mRID
        
      ExcAC3A : IdentifiedObject.name
        
      ExcAC3A : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcAC3A --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
          click OverexcitationLimiterDynamics href "../OverexcitationLimiterDynamics"
        
      ExcAC3A : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcAC3A --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
          click PFVArControllerType1Dynamics href "../PFVArControllerType1Dynamics"
        
      ExcAC3A : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcAC3A --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
          click PFVArControllerType2Dynamics href "../PFVArControllerType2Dynamics"
        
      ExcAC3A : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcAC3A --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
          click PowerSystemStabilizerDynamics href "../PowerSystemStabilizerDynamics"
        
      ExcAC3A : ExcAC3A.seve1
        
      ExcAC3A : ExcAC3A.seve2
        
      ExcAC3A : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcAC3A --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
          click SynchronousMachineDynamics href "../SynchronousMachineDynamics"
        
      ExcAC3A : ExcAC3A.ta
        
          ExcAC3A --> PU : ExcAC3A.ta
          click PU href "../PU"
        
      ExcAC3A : ExcAC3A.tb
        
          ExcAC3A --> Seconds : ExcAC3A.tb
          click Seconds href "../Seconds"
        
      ExcAC3A : ExcAC3A.tc
        
          ExcAC3A --> Seconds : ExcAC3A.tc
          click Seconds href "../Seconds"
        
      ExcAC3A : ExcAC3A.te
        
          ExcAC3A --> Seconds : ExcAC3A.te
          click Seconds href "../Seconds"
        
      ExcAC3A : ExcAC3A.tf
        
          ExcAC3A --> Seconds : ExcAC3A.tf
          click Seconds href "../Seconds"
        
      ExcAC3A : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcAC3A --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
          click UnderexcitationLimiterDynamics href "../UnderexcitationLimiterDynamics"
        
      ExcAC3A : ExcAC3A.vamax
        
          ExcAC3A --> PU : ExcAC3A.vamax
          click PU href "../PU"
        
      ExcAC3A : ExcAC3A.vamin
        
          ExcAC3A --> PU : ExcAC3A.vamin
          click PU href "../PU"
        
      ExcAC3A : ExcAC3A.ve1
        
          ExcAC3A --> PU : ExcAC3A.ve1
          click PU href "../PU"
        
      ExcAC3A : ExcAC3A.ve2
        
          ExcAC3A --> PU : ExcAC3A.ve2
          click PU href "../PU"
        
      ExcAC3A : ExcAC3A.vemin
        
          ExcAC3A --> PU : ExcAC3A.vemin
          click PU href "../PU"
        
      ExcAC3A : ExcAC3A.vfemax
        
          ExcAC3A --> PU : ExcAC3A.vfemax
          click PU href "../PU"
        
      ExcAC3A : ExcAC3A.vlv
        
          ExcAC3A --> PU : ExcAC3A.vlv
          click PU href "../PU"
        
      ExcAC3A : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcAC3A --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
          click VoltageCompensatorDynamics href "../VoltageCompensatorDynamics"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcAC3A**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| tb | [cim:ExcAC3A.tb](http://iec.ch/TC57/CIM100#ExcAC3A.tb) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tb</i>) (&gt;= 0) | direct |
| tc | [cim:ExcAC3A.tc](http://iec.ch/TC57/CIM100#ExcAC3A.tc) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tc</i>) (&gt;= 0) | direct |
| ka | [cim:ExcAC3A.ka](http://iec.ch/TC57/CIM100#ExcAC3A.ka) | 1 <br />  [Seconds](Seconds.md)  | Voltage regulator gain (<i>Ka</i>) (&gt; 0) | direct |
| ta | [cim:ExcAC3A.ta](http://iec.ch/TC57/CIM100#ExcAC3A.ta) | 1 <br />  [PU](PU.md)  | Voltage regulator time constant (<i>Ta</i>) (&gt; 0) | direct |
| vamax | [cim:ExcAC3A.vamax](http://iec.ch/TC57/CIM100#ExcAC3A.vamax) | 1 <br />  [PU](PU.md)  | Maximum voltage regulator output (<i>Vamax</i>) (&gt; 0) | direct |
| vamin | [cim:ExcAC3A.vamin](http://iec.ch/TC57/CIM100#ExcAC3A.vamin) | 1 <br />  [PU](PU.md)  | Minimum voltage regulator output (<i>Vamin</i>) (&lt; 0) | direct |
| te | [cim:ExcAC3A.te](http://iec.ch/TC57/CIM100#ExcAC3A.te) | 1 <br />  [Seconds](Seconds.md)  | Exciter time constant, integration rate associated with exciter control (<i>T... | direct |
| vemin | [cim:ExcAC3A.vemin](http://iec.ch/TC57/CIM100#ExcAC3A.vemin) | 1 <br />  [PU](PU.md)  | Minimum exciter voltage output (<i>Vemin</i>) (&lt;= 0) | direct |
| kr | [cim:ExcAC3A.kr](http://iec.ch/TC57/CIM100#ExcAC3A.kr) | 1 <br />  [PU](PU.md)  | Constant associated with regulator and alternator field power supply (<i>Kr</... | direct |
| kf | [cim:ExcAC3A.kf](http://iec.ch/TC57/CIM100#ExcAC3A.kf) | 1 <br />  [PU](PU.md)  | Excitation control system stabilizer gains (<i>Kf</i>) (&gt;= 0) | direct |
| tf | [cim:ExcAC3A.tf](http://iec.ch/TC57/CIM100#ExcAC3A.tf) | 1 <br />  [Seconds](Seconds.md)  | Excitation control system stabilizer time constant (<i>Tf</i>) (&gt; 0) | direct |
| kn | [cim:ExcAC3A.kn](http://iec.ch/TC57/CIM100#ExcAC3A.kn) | 1 <br />  [PU](PU.md)  | Excitation control system stabilizer gain (<i>Kn</i>) (&gt;= 0) | direct |
| efdn | [cim:ExcAC3A.efdn](http://iec.ch/TC57/CIM100#ExcAC3A.efdn) | 1 <br />  [PU](PU.md)  | Value of <i>Efd </i>at which feedback gain changes (<i>Efdn</i>) (&gt; 0) | direct |
| kc | [cim:ExcAC3A.kc](http://iec.ch/TC57/CIM100#ExcAC3A.kc) | 1 <br />  [PU](PU.md)  | Rectifier loading factor proportional to commutating reactance (<i>Kc</i>) (&... | direct |
| kd | [cim:ExcAC3A.kd](http://iec.ch/TC57/CIM100#ExcAC3A.kd) | 1 <br />  [PU](PU.md)  | Demagnetizing factor, a function of exciter alternator reactances (<i>Kd</i>)... | direct |
| ke | [cim:ExcAC3A.ke](http://iec.ch/TC57/CIM100#ExcAC3A.ke) | 1 <br />  [PU](PU.md)  | Exciter constant related to self-excited field (<i>Ke</i>) | direct |
| klv | [cim:ExcAC3A.klv](http://iec.ch/TC57/CIM100#ExcAC3A.klv) | 1 <br />  [PU](PU.md)  | Gain used in the minimum field voltage limiter loop (<i>Klv</i>) | direct |
| kf1 | [cim:ExcAC3A.kf1](http://iec.ch/TC57/CIM100#ExcAC3A.kf1) | 1 <br />  [PU](PU.md)  | Coefficient to allow different usage of the model (<i>Kf1</i>) | direct |
| kf2 | [cim:ExcAC3A.kf2](http://iec.ch/TC57/CIM100#ExcAC3A.kf2) | 1 <br />  [PU](PU.md)  | Coefficient to allow different usage of the model (<i>Kf2</i>) | direct |
| ks | [cim:ExcAC3A.ks](http://iec.ch/TC57/CIM100#ExcAC3A.ks) | 1 <br />  [PU](PU.md)  | Coefficient to allow different usage of the model-speed coefficient (<i>Ks</i... | direct |
| vfemax | [cim:ExcAC3A.vfemax](http://iec.ch/TC57/CIM100#ExcAC3A.vfemax) | 1 <br />  [PU](PU.md)  | Exciter field current limit reference (<i>Vfemax</i>) (&gt;= 0) | direct |
| ve1 | [cim:ExcAC3A.ve1](http://iec.ch/TC57/CIM100#ExcAC3A.ve1) | 1 <br />  [PU](PU.md)  | Exciter alternator output voltages back of commutating reactance at which sat... | direct |
| seve1 | [cim:ExcAC3A.seve1](http://iec.ch/TC57/CIM100#ExcAC3A.seve1) | 1 <br />  float  | Exciter saturation function value at the corresponding exciter voltage, <i>Ve... | direct |
| ve2 | [cim:ExcAC3A.ve2](http://iec.ch/TC57/CIM100#ExcAC3A.ve2) | 1 <br />  [PU](PU.md)  | Exciter alternator output voltages back of commutating reactance at which sat... | direct |
| seve2 | [cim:ExcAC3A.seve2](http://iec.ch/TC57/CIM100#ExcAC3A.seve2) | 1 <br />  float  | Exciter saturation function value at the corresponding exciter voltage, <i>Ve... | direct |
| vlv | [cim:ExcAC3A.vlv](http://iec.ch/TC57/CIM100#ExcAC3A.vlv) | 1 <br />  [PU](PU.md)  | Field voltage used in the minimum field voltage limiter loop (<i>Vlv</i>) | direct |
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
| self | cim:ExcAC3A |
| native | this:ExcAC3A |




