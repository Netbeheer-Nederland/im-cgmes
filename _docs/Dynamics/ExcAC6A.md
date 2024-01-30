# ExcAC6A


_Modified IEEE AC6A alternator-supplied rectifier excitation system with speed input._





**URI**: [cim:ExcAC6A](http://iec.ch/TC57/CIM100#ExcAC6A)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcAC6A
      ExcitationSystemDynamics <|-- ExcAC6A
      
      ExcAC6A : IdentifiedObject.description
        
      ExcAC6A : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcAC6A --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
      ExcAC6A : DynamicsFunctionBlock.enabled
        
      ExcAC6A : ExcAC6A.ka
        
          ExcAC6A --> PU : ExcAC6A.ka
        
      ExcAC6A : ExcAC6A.kc
        
          ExcAC6A --> PU : ExcAC6A.kc
        
      ExcAC6A : ExcAC6A.kd
        
          ExcAC6A --> PU : ExcAC6A.kd
        
      ExcAC6A : ExcAC6A.ke
        
          ExcAC6A --> PU : ExcAC6A.ke
        
      ExcAC6A : ExcAC6A.kh
        
          ExcAC6A --> PU : ExcAC6A.kh
        
      ExcAC6A : ExcAC6A.ks
        
          ExcAC6A --> PU : ExcAC6A.ks
        
      ExcAC6A : IdentifiedObject.mRID
        
      ExcAC6A : IdentifiedObject.name
        
      ExcAC6A : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcAC6A --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
      ExcAC6A : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcAC6A --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
      ExcAC6A : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcAC6A --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
      ExcAC6A : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcAC6A --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
      ExcAC6A : ExcAC6A.seve1
        
      ExcAC6A : ExcAC6A.seve2
        
      ExcAC6A : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcAC6A --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
        
      ExcAC6A : ExcAC6A.ta
        
          ExcAC6A --> Seconds : ExcAC6A.ta
        
      ExcAC6A : ExcAC6A.tb
        
          ExcAC6A --> Seconds : ExcAC6A.tb
        
      ExcAC6A : ExcAC6A.tc
        
          ExcAC6A --> Seconds : ExcAC6A.tc
        
      ExcAC6A : ExcAC6A.te
        
          ExcAC6A --> Seconds : ExcAC6A.te
        
      ExcAC6A : ExcAC6A.th
        
          ExcAC6A --> Seconds : ExcAC6A.th
        
      ExcAC6A : ExcAC6A.tj
        
          ExcAC6A --> Seconds : ExcAC6A.tj
        
      ExcAC6A : ExcAC6A.tk
        
          ExcAC6A --> Seconds : ExcAC6A.tk
        
      ExcAC6A : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcAC6A --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
      ExcAC6A : ExcAC6A.vamax
        
          ExcAC6A --> PU : ExcAC6A.vamax
        
      ExcAC6A : ExcAC6A.vamin
        
          ExcAC6A --> PU : ExcAC6A.vamin
        
      ExcAC6A : ExcAC6A.ve1
        
          ExcAC6A --> PU : ExcAC6A.ve1
        
      ExcAC6A : ExcAC6A.ve2
        
          ExcAC6A --> PU : ExcAC6A.ve2
        
      ExcAC6A : ExcAC6A.vfelim
        
          ExcAC6A --> PU : ExcAC6A.vfelim
        
      ExcAC6A : ExcAC6A.vhmax
        
          ExcAC6A --> PU : ExcAC6A.vhmax
        
      ExcAC6A : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcAC6A --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
      ExcAC6A : ExcAC6A.vrmax
        
          ExcAC6A --> PU : ExcAC6A.vrmax
        
      ExcAC6A : ExcAC6A.vrmin
        
          ExcAC6A --> PU : ExcAC6A.vrmin
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcAC6A**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ka | [cim:ExcAC6A.ka](http://iec.ch/TC57/CIM100#ExcAC6A.ka) | 1..1 <br />  [PU](PU.md)  | Voltage regulator gain (<i>Ka</i>) (&gt; 0) | direct |
| ks | [cim:ExcAC6A.ks](http://iec.ch/TC57/CIM100#ExcAC6A.ks) | 1..1 <br />  [PU](PU.md)  | Coefficient to allow different usage of the model-speed coefficient (<i>Ks</i... | direct |
| ta | [cim:ExcAC6A.ta](http://iec.ch/TC57/CIM100#ExcAC6A.ta) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Ta</i>) (&gt;= 0) | direct |
| tk | [cim:ExcAC6A.tk](http://iec.ch/TC57/CIM100#ExcAC6A.tk) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tk</i>) (&gt;= 0) | direct |
| tb | [cim:ExcAC6A.tb](http://iec.ch/TC57/CIM100#ExcAC6A.tb) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tb</i>) (&gt;= 0) | direct |
| tc | [cim:ExcAC6A.tc](http://iec.ch/TC57/CIM100#ExcAC6A.tc) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tc</i>) (&gt;= 0) | direct |
| vamax | [cim:ExcAC6A.vamax](http://iec.ch/TC57/CIM100#ExcAC6A.vamax) | 1..1 <br />  [PU](PU.md)  | Maximum voltage regulator output (<i>Vamax</i>) (&gt; 0) | direct |
| vamin | [cim:ExcAC6A.vamin](http://iec.ch/TC57/CIM100#ExcAC6A.vamin) | 1..1 <br />  [PU](PU.md)  | Minimum voltage regulator output (<i>Vamin</i>) (&lt; 0) | direct |
| vrmax | [cim:ExcAC6A.vrmax](http://iec.ch/TC57/CIM100#ExcAC6A.vrmax) | 1..1 <br />  [PU](PU.md)  | Maximum voltage regulator output (<i>Vrmax</i>) (&gt; 0) | direct |
| vrmin | [cim:ExcAC6A.vrmin](http://iec.ch/TC57/CIM100#ExcAC6A.vrmin) | 1..1 <br />  [PU](PU.md)  | Minimum voltage regulator output (<i>Vrmin</i>) (&lt; 0) | direct |
| te | [cim:ExcAC6A.te](http://iec.ch/TC57/CIM100#ExcAC6A.te) | 1..1 <br />  [Seconds](Seconds.md)  | Exciter time constant, integration rate associated with exciter control (<i>T... | direct |
| kh | [cim:ExcAC6A.kh](http://iec.ch/TC57/CIM100#ExcAC6A.kh) | 1..1 <br />  [PU](PU.md)  | Exciter field current limiter gain (<i>Kh</i>) (&gt;= 0) | direct |
| tj | [cim:ExcAC6A.tj](http://iec.ch/TC57/CIM100#ExcAC6A.tj) | 1..1 <br />  [Seconds](Seconds.md)  | Exciter field current limiter time constant (<i>Tj</i>) (&gt;= 0) | direct |
| th | [cim:ExcAC6A.th](http://iec.ch/TC57/CIM100#ExcAC6A.th) | 1..1 <br />  [Seconds](Seconds.md)  | Exciter field current limiter time constant (<i>Th</i>) (&gt; 0) | direct |
| vfelim | [cim:ExcAC6A.vfelim](http://iec.ch/TC57/CIM100#ExcAC6A.vfelim) | 1..1 <br />  [PU](PU.md)  | Exciter field current limit reference (<i>Vfelim</i>) (&gt; 0) | direct |
| vhmax | [cim:ExcAC6A.vhmax](http://iec.ch/TC57/CIM100#ExcAC6A.vhmax) | 1..1 <br />  [PU](PU.md)  | Maximum field current limiter signal reference (<i>Vhmax</i>) (&gt; 0) | direct |
| kc | [cim:ExcAC6A.kc](http://iec.ch/TC57/CIM100#ExcAC6A.kc) | 1..1 <br />  [PU](PU.md)  | Rectifier loading factor proportional to commutating reactance (<i>Kc</i>) (&... | direct |
| kd | [cim:ExcAC6A.kd](http://iec.ch/TC57/CIM100#ExcAC6A.kd) | 1..1 <br />  [PU](PU.md)  | Demagnetizing factor, a function of exciter alternator reactances (<i>Kd</i>)... | direct |
| ke | [cim:ExcAC6A.ke](http://iec.ch/TC57/CIM100#ExcAC6A.ke) | 1..1 <br />  [PU](PU.md)  | Exciter constant related to self-excited field (<i>Ke</i>) | direct |
| ve1 | [cim:ExcAC6A.ve1](http://iec.ch/TC57/CIM100#ExcAC6A.ve1) | 1..1 <br />  [PU](PU.md)  | Exciter alternator output voltages back of commutating reactance at which sat... | direct |
| seve1 | [cim:ExcAC6A.seve1](http://iec.ch/TC57/CIM100#ExcAC6A.seve1) | 1..1 <br />  float  | Exciter saturation function value at the corresponding exciter voltage, <i>Ve... | direct |
| ve2 | [cim:ExcAC6A.ve2](http://iec.ch/TC57/CIM100#ExcAC6A.ve2) | 1..1 <br />  [PU](PU.md)  | Exciter alternator output voltages back of commutating reactance at which sat... | direct |
| seve2 | [cim:ExcAC6A.seve2](http://iec.ch/TC57/CIM100#ExcAC6A.seve2) | 1..1 <br />  float  | Exciter saturation function value at the corresponding exciter voltage, <i>Ve... | direct |
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
| self | cim:ExcAC6A |
| native | this:ExcAC6A |




