# ExcANS


_Italian excitation system. It represents static field voltage or excitation current feedback excitation system._





**URI**: [cim:ExcANS](http://iec.ch/TC57/CIM100#ExcANS)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcANS
      ExcitationSystemDynamics <|-- ExcANS
      
      ExcANS : ExcANS.blint
        
      ExcANS : IdentifiedObject.description
        
      ExcANS : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcANS --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
      ExcANS : DynamicsFunctionBlock.enabled
        
      ExcANS : ExcANS.ifmn
        
          ExcANS --> PU : ExcANS.ifmn
        
      ExcANS : ExcANS.ifmx
        
          ExcANS --> PU : ExcANS.ifmx
        
      ExcANS : ExcANS.k2
        
      ExcANS : ExcANS.k3
        
      ExcANS : ExcANS.kce
        
      ExcANS : ExcANS.krvecc
        
      ExcANS : ExcANS.kvfif
        
      ExcANS : IdentifiedObject.mRID
        
      ExcANS : IdentifiedObject.name
        
      ExcANS : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcANS --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
      ExcANS : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcANS --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
      ExcANS : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcANS --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
      ExcANS : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcANS --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
      ExcANS : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcANS --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
        
      ExcANS : ExcANS.t1
        
          ExcANS --> Seconds : ExcANS.t1
        
      ExcANS : ExcANS.t2
        
          ExcANS --> Seconds : ExcANS.t2
        
      ExcANS : ExcANS.t3
        
          ExcANS --> Seconds : ExcANS.t3
        
      ExcANS : ExcANS.tb
        
          ExcANS --> Seconds : ExcANS.tb
        
      ExcANS : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcANS --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
      ExcANS : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcANS --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
      ExcANS : ExcANS.vrmn
        
          ExcANS --> PU : ExcANS.vrmn
        
      ExcANS : ExcANS.vrmx
        
          ExcANS --> PU : ExcANS.vrmx
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcANS**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| k3 | [cim:ExcANS.k3](http://iec.ch/TC57/CIM100#ExcANS.k3) | 1..1 <br />  float  | AVR gain (<i>K</i><i><sub>3</sub></i>) | direct |
| k2 | [cim:ExcANS.k2](http://iec.ch/TC57/CIM100#ExcANS.k2) | 1..1 <br />  float  | Exciter gain (<i>K</i><i><sub>2</sub></i>) | direct |
| kce | [cim:ExcANS.kce](http://iec.ch/TC57/CIM100#ExcANS.kce) | 1..1 <br />  float  | Ceiling factor (<i>K</i><i><sub>CE</sub></i>) | direct |
| t3 | [cim:ExcANS.t3](http://iec.ch/TC57/CIM100#ExcANS.t3) | 1..1 <br />  [Seconds](Seconds.md)  | Time constant (<i>T</i><i><sub>3</sub></i>) (&gt;= 0) | direct |
| t2 | [cim:ExcANS.t2](http://iec.ch/TC57/CIM100#ExcANS.t2) | 1..1 <br />  [Seconds](Seconds.md)  | Time constant (<i>T</i><i><sub>2</sub></i>) (&gt;= 0) | direct |
| t1 | [cim:ExcANS.t1](http://iec.ch/TC57/CIM100#ExcANS.t1) | 1..1 <br />  [Seconds](Seconds.md)  | Time constant (<i>T</i><i><sub>1</sub></i>) (&gt;= 0) | direct |
| blint | [cim:ExcANS.blint](http://iec.ch/TC57/CIM100#ExcANS.blint) | 1..1 <br />  integer  | Governor control flag (<i>BLINT</i>) | direct |
| kvfif | [cim:ExcANS.kvfif](http://iec.ch/TC57/CIM100#ExcANS.kvfif) | 1..1 <br />  integer  | Rate feedback signal flag (<i>K</i><i><sub>VFIF</sub></i>) | direct |
| ifmn | [cim:ExcANS.ifmn](http://iec.ch/TC57/CIM100#ExcANS.ifmn) | 1..1 <br />  [PU](PU.md)  | Minimum exciter current (<i>I</i><i><sub>FMN</sub></i>) | direct |
| ifmx | [cim:ExcANS.ifmx](http://iec.ch/TC57/CIM100#ExcANS.ifmx) | 1..1 <br />  [PU](PU.md)  | Maximum exciter current (<i>I</i><i><sub>FMX</sub></i>) | direct |
| vrmn | [cim:ExcANS.vrmn](http://iec.ch/TC57/CIM100#ExcANS.vrmn) | 1..1 <br />  [PU](PU.md)  | Minimum AVR output (<i>V</i><i><sub>RMN</sub></i>) | direct |
| vrmx | [cim:ExcANS.vrmx](http://iec.ch/TC57/CIM100#ExcANS.vrmx) | 1..1 <br />  [PU](PU.md)  | Maximum AVR output (<i>V</i><i><sub>RMX</sub></i>) | direct |
| krvecc | [cim:ExcANS.krvecc](http://iec.ch/TC57/CIM100#ExcANS.krvecc) | 1..1 <br />  integer  | Feedback enabling (<i>K</i><i><sub>RVECC</sub></i>) | direct |
| tb | [cim:ExcANS.tb](http://iec.ch/TC57/CIM100#ExcANS.tb) | 1..1 <br />  [Seconds](Seconds.md)  | Exciter time constant (<i>T</i><i><sub>B</sub></i>) (&gt;= 0) | direct |
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
| self | cim:ExcANS |
| native | this:ExcANS |




