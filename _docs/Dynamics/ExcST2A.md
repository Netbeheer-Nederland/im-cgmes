# ExcST2A


_Modified IEEE ST2A static excitation system with another lead-lag block added to match the model defined by WECC._





**URI**: [cim:ExcST2A](http://iec.ch/TC57/CIM100#ExcST2A)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcST2A
      ExcitationSystemDynamics <|-- ExcST2A
      
      ExcST2A : IdentifiedObject.description
        
      ExcST2A : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcST2A --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
      ExcST2A : ExcST2A.efdmax
        
          ExcST2A --> PU : ExcST2A.efdmax
        
      ExcST2A : DynamicsFunctionBlock.enabled
        
      ExcST2A : ExcST2A.ka
        
          ExcST2A --> PU : ExcST2A.ka
        
      ExcST2A : ExcST2A.kc
        
          ExcST2A --> PU : ExcST2A.kc
        
      ExcST2A : ExcST2A.ke
        
          ExcST2A --> PU : ExcST2A.ke
        
      ExcST2A : ExcST2A.kf
        
          ExcST2A --> PU : ExcST2A.kf
        
      ExcST2A : ExcST2A.ki
        
          ExcST2A --> PU : ExcST2A.ki
        
      ExcST2A : ExcST2A.kp
        
          ExcST2A --> PU : ExcST2A.kp
        
      ExcST2A : IdentifiedObject.mRID
        
      ExcST2A : IdentifiedObject.name
        
      ExcST2A : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcST2A --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
      ExcST2A : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcST2A --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
      ExcST2A : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcST2A --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
      ExcST2A : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcST2A --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
      ExcST2A : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcST2A --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
        
      ExcST2A : ExcST2A.ta
        
          ExcST2A --> Seconds : ExcST2A.ta
        
      ExcST2A : ExcST2A.tb
        
          ExcST2A --> Seconds : ExcST2A.tb
        
      ExcST2A : ExcST2A.tc
        
          ExcST2A --> Seconds : ExcST2A.tc
        
      ExcST2A : ExcST2A.te
        
          ExcST2A --> Seconds : ExcST2A.te
        
      ExcST2A : ExcST2A.tf
        
          ExcST2A --> Seconds : ExcST2A.tf
        
      ExcST2A : ExcST2A.uelin
        
      ExcST2A : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcST2A --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
      ExcST2A : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcST2A --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
      ExcST2A : ExcST2A.vrmax
        
          ExcST2A --> PU : ExcST2A.vrmax
        
      ExcST2A : ExcST2A.vrmin
        
          ExcST2A --> PU : ExcST2A.vrmin
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcST2A**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ka | [cim:ExcST2A.ka](http://iec.ch/TC57/CIM100#ExcST2A.ka) | 1..1 <br />  [PU](PU.md)  | Voltage regulator gain (<i>Ka</i>) (&gt; 0) | direct |
| ta | [cim:ExcST2A.ta](http://iec.ch/TC57/CIM100#ExcST2A.ta) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Ta</i>) (&gt; 0) | direct |
| vrmax | [cim:ExcST2A.vrmax](http://iec.ch/TC57/CIM100#ExcST2A.vrmax) | 1..1 <br />  [PU](PU.md)  | Maximum voltage regulator outputs (<i>Vrmax</i>) (&gt; 0) | direct |
| vrmin | [cim:ExcST2A.vrmin](http://iec.ch/TC57/CIM100#ExcST2A.vrmin) | 1..1 <br />  [PU](PU.md)  | Minimum voltage regulator outputs (<i>Vrmin</i>) (&lt; 0) | direct |
| ke | [cim:ExcST2A.ke](http://iec.ch/TC57/CIM100#ExcST2A.ke) | 1..1 <br />  [PU](PU.md)  | Exciter constant related to self-excited field (<i>Ke</i>) | direct |
| te | [cim:ExcST2A.te](http://iec.ch/TC57/CIM100#ExcST2A.te) | 1..1 <br />  [Seconds](Seconds.md)  | Exciter time constant, integration rate associated with exciter control (<i>T... | direct |
| kf | [cim:ExcST2A.kf](http://iec.ch/TC57/CIM100#ExcST2A.kf) | 1..1 <br />  [PU](PU.md)  | Excitation control system stabilizer gains (<i>kf</i>) (&gt;= 0) | direct |
| tf | [cim:ExcST2A.tf](http://iec.ch/TC57/CIM100#ExcST2A.tf) | 1..1 <br />  [Seconds](Seconds.md)  | Excitation control system stabilizer time constant (<i>Tf</i>) (&gt;= 0) | direct |
| kp | [cim:ExcST2A.kp](http://iec.ch/TC57/CIM100#ExcST2A.kp) | 1..1 <br />  [PU](PU.md)  | Potential circuit gain coefficient (<i>K</i><i><sub>p</sub></i>) (&gt;= 0) | direct |
| ki | [cim:ExcST2A.ki](http://iec.ch/TC57/CIM100#ExcST2A.ki) | 1..1 <br />  [PU](PU.md)  | Potential circuit gain coefficient (<i>K</i><i><sub>i</sub></i>) (&gt;= 0) | direct |
| kc | [cim:ExcST2A.kc](http://iec.ch/TC57/CIM100#ExcST2A.kc) | 1..1 <br />  [PU](PU.md)  | Rectifier loading factor proportional to commutating reactance (<i>Kc</i>) (&... | direct |
| efdmax | [cim:ExcST2A.efdmax](http://iec.ch/TC57/CIM100#ExcST2A.efdmax) | 1..1 <br />  [PU](PU.md)  | Maximum field voltage (<i>Efdmax</i>) (&gt;= 0) | direct |
| uelin | [cim:ExcST2A.uelin](http://iec.ch/TC57/CIM100#ExcST2A.uelin) | 1..1 <br />  boolean  | UEL input (<i>UELin</i>) | direct |
| tb | [cim:ExcST2A.tb](http://iec.ch/TC57/CIM100#ExcST2A.tb) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tb</i>) (&gt;= 0) | direct |
| tc | [cim:ExcST2A.tc](http://iec.ch/TC57/CIM100#ExcST2A.tc) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tc</i>) (&gt;= 0) | direct |
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
| self | cim:ExcST2A |
| native | this:ExcST2A |




