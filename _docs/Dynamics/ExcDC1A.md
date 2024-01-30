# ExcDC1A


_Modified IEEE DC1A direct current commutator exciter with speed input and without underexcitation limiters (UEL) inputs._





**URI**: [cim:ExcDC1A](http://iec.ch/TC57/CIM100#ExcDC1A)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcDC1A
      ExcitationSystemDynamics <|-- ExcDC1A
      
      ExcDC1A : IdentifiedObject.description
        
      ExcDC1A : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcDC1A --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
      ExcDC1A : ExcDC1A.efd1
        
          ExcDC1A --> PU : ExcDC1A.efd1
        
      ExcDC1A : ExcDC1A.efd2
        
          ExcDC1A --> PU : ExcDC1A.efd2
        
      ExcDC1A : ExcDC1A.efdmax
        
          ExcDC1A --> PU : ExcDC1A.efdmax
        
      ExcDC1A : ExcDC1A.efdmin
        
          ExcDC1A --> PU : ExcDC1A.efdmin
        
      ExcDC1A : DynamicsFunctionBlock.enabled
        
      ExcDC1A : ExcDC1A.exclim
        
      ExcDC1A : ExcDC1A.ka
        
          ExcDC1A --> PU : ExcDC1A.ka
        
      ExcDC1A : ExcDC1A.ke
        
          ExcDC1A --> PU : ExcDC1A.ke
        
      ExcDC1A : ExcDC1A.kf
        
          ExcDC1A --> PU : ExcDC1A.kf
        
      ExcDC1A : ExcDC1A.ks
        
          ExcDC1A --> PU : ExcDC1A.ks
        
      ExcDC1A : IdentifiedObject.mRID
        
      ExcDC1A : IdentifiedObject.name
        
      ExcDC1A : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcDC1A --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
      ExcDC1A : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcDC1A --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
      ExcDC1A : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcDC1A --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
      ExcDC1A : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcDC1A --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
      ExcDC1A : ExcDC1A.seefd1
        
      ExcDC1A : ExcDC1A.seefd2
        
      ExcDC1A : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcDC1A --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
        
      ExcDC1A : ExcDC1A.ta
        
          ExcDC1A --> Seconds : ExcDC1A.ta
        
      ExcDC1A : ExcDC1A.tb
        
          ExcDC1A --> Seconds : ExcDC1A.tb
        
      ExcDC1A : ExcDC1A.tc
        
          ExcDC1A --> Seconds : ExcDC1A.tc
        
      ExcDC1A : ExcDC1A.te
        
          ExcDC1A --> Seconds : ExcDC1A.te
        
      ExcDC1A : ExcDC1A.tf
        
          ExcDC1A --> Seconds : ExcDC1A.tf
        
      ExcDC1A : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcDC1A --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
      ExcDC1A : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcDC1A --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
      ExcDC1A : ExcDC1A.vrmax
        
          ExcDC1A --> PU : ExcDC1A.vrmax
        
      ExcDC1A : ExcDC1A.vrmin
        
          ExcDC1A --> PU : ExcDC1A.vrmin
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcDC1A**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ka | [cim:ExcDC1A.ka](http://iec.ch/TC57/CIM100#ExcDC1A.ka) | 1..1 <br />  [PU](PU.md)  | Voltage regulator gain (<i>Ka</i>) (&gt; 0) | direct |
| ks | [cim:ExcDC1A.ks](http://iec.ch/TC57/CIM100#ExcDC1A.ks) | 1..1 <br />  [PU](PU.md)  | Coefficient to allow different usage of the model-speed coefficient (<i>Ks</i... | direct |
| ta | [cim:ExcDC1A.ta](http://iec.ch/TC57/CIM100#ExcDC1A.ta) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Ta</i>) (&gt; 0) | direct |
| tb | [cim:ExcDC1A.tb](http://iec.ch/TC57/CIM100#ExcDC1A.tb) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tb</i>) (&gt;= 0) | direct |
| tc | [cim:ExcDC1A.tc](http://iec.ch/TC57/CIM100#ExcDC1A.tc) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tc</i>) (&gt;= 0) | direct |
| vrmax | [cim:ExcDC1A.vrmax](http://iec.ch/TC57/CIM100#ExcDC1A.vrmax) | 1..1 <br />  [PU](PU.md)  | Maximum voltage regulator output (<i>Vrmax</i>) (&gt; ExcDC1A | direct |
| vrmin | [cim:ExcDC1A.vrmin](http://iec.ch/TC57/CIM100#ExcDC1A.vrmin) | 1..1 <br />  [PU](PU.md)  | Minimum voltage regulator output (<i>Vrmin</i>) (&lt; 0 and &lt; ExcDC1A | direct |
| ke | [cim:ExcDC1A.ke](http://iec.ch/TC57/CIM100#ExcDC1A.ke) | 1..1 <br />  [PU](PU.md)  | Exciter constant related to self-excited field (<i>Ke</i>) | direct |
| te | [cim:ExcDC1A.te](http://iec.ch/TC57/CIM100#ExcDC1A.te) | 1..1 <br />  [Seconds](Seconds.md)  | Exciter time constant, integration rate associated with exciter control (<i>T... | direct |
| kf | [cim:ExcDC1A.kf](http://iec.ch/TC57/CIM100#ExcDC1A.kf) | 1..1 <br />  [PU](PU.md)  | Excitation control system stabilizer gain (<i>Kf</i>) (&gt;= 0) | direct |
| tf | [cim:ExcDC1A.tf](http://iec.ch/TC57/CIM100#ExcDC1A.tf) | 1..1 <br />  [Seconds](Seconds.md)  | Excitation control system stabilizer time constant (<i>Tf</i>) (&gt; 0) | direct |
| efd1 | [cim:ExcDC1A.efd1](http://iec.ch/TC57/CIM100#ExcDC1A.efd1) | 1..1 <br />  [PU](PU.md)  | Exciter voltage at which exciter saturation is defined (<i>Efd</i><i><sub>1</... | direct |
| seefd1 | [cim:ExcDC1A.seefd1](http://iec.ch/TC57/CIM100#ExcDC1A.seefd1) | 1..1 <br />  float  | Exciter saturation function value at the corresponding exciter voltage, <i>Ef... | direct |
| efd2 | [cim:ExcDC1A.efd2](http://iec.ch/TC57/CIM100#ExcDC1A.efd2) | 1..1 <br />  [PU](PU.md)  | Exciter voltage at which exciter saturation is defined (<i>Efd</i><i><sub>2</... | direct |
| seefd2 | [cim:ExcDC1A.seefd2](http://iec.ch/TC57/CIM100#ExcDC1A.seefd2) | 1..1 <br />  float  | Exciter saturation function value at the corresponding exciter voltage, <i>Ef... | direct |
| exclim | [cim:ExcDC1A.exclim](http://iec.ch/TC57/CIM100#ExcDC1A.exclim) | 1..1 <br />  boolean  | (<i>exclim</i>) | direct |
| efdmin | [cim:ExcDC1A.efdmin](http://iec.ch/TC57/CIM100#ExcDC1A.efdmin) | 1..1 <br />  [PU](PU.md)  | Minimum voltage exciter output limiter (<i>Efdmin</i>) (&lt; ExcDC1A | direct |
| efdmax | [cim:ExcDC1A.efdmax](http://iec.ch/TC57/CIM100#ExcDC1A.efdmax) | 1..1 <br />  [PU](PU.md)  | Maximum voltage exciter output limiter (<i>Efdmax</i>) (&gt; ExcDC1A | direct |
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
| self | cim:ExcDC1A |
| native | this:ExcDC1A |




