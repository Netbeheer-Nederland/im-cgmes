# ExcIEEEST1A


_IEEE 421.5-2005 type ST1A model. This model represents systems in which excitation power is supplied through a transformer from the generator terminals (or the unit’s auxiliary bus) and is regulated by a controlled rectifier.  The maximum exciter voltage available from such systems is directly related to the generator terminal voltage._

_Reference: IEEE 421.5-2005, 7.1._





**URI**: [cim:ExcIEEEST1A](http://iec.ch/TC57/CIM100#ExcIEEEST1A)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcIEEEST1A
      ExcitationSystemDynamics <|-- ExcIEEEST1A
      
      ExcIEEEST1A : IdentifiedObject.description
        
      ExcIEEEST1A : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcIEEEST1A --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
      ExcIEEEST1A : DynamicsFunctionBlock.enabled
        
      ExcIEEEST1A : ExcIEEEST1A.ilr
        
          ExcIEEEST1A --> PU : ExcIEEEST1A.ilr
        
      ExcIEEEST1A : ExcIEEEST1A.ka
        
          ExcIEEEST1A --> PU : ExcIEEEST1A.ka
        
      ExcIEEEST1A : ExcIEEEST1A.kc
        
          ExcIEEEST1A --> PU : ExcIEEEST1A.kc
        
      ExcIEEEST1A : ExcIEEEST1A.kf
        
          ExcIEEEST1A --> PU : ExcIEEEST1A.kf
        
      ExcIEEEST1A : ExcIEEEST1A.klr
        
          ExcIEEEST1A --> PU : ExcIEEEST1A.klr
        
      ExcIEEEST1A : IdentifiedObject.mRID
        
      ExcIEEEST1A : IdentifiedObject.name
        
      ExcIEEEST1A : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcIEEEST1A --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
      ExcIEEEST1A : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcIEEEST1A --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
      ExcIEEEST1A : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcIEEEST1A --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
      ExcIEEEST1A : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcIEEEST1A --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
      ExcIEEEST1A : ExcIEEEST1A.pssin
        
      ExcIEEEST1A : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcIEEEST1A --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
        
      ExcIEEEST1A : ExcIEEEST1A.ta
        
          ExcIEEEST1A --> Seconds : ExcIEEEST1A.ta
        
      ExcIEEEST1A : ExcIEEEST1A.tb
        
          ExcIEEEST1A --> Seconds : ExcIEEEST1A.tb
        
      ExcIEEEST1A : ExcIEEEST1A.tb1
        
          ExcIEEEST1A --> Seconds : ExcIEEEST1A.tb1
        
      ExcIEEEST1A : ExcIEEEST1A.tc
        
          ExcIEEEST1A --> Seconds : ExcIEEEST1A.tc
        
      ExcIEEEST1A : ExcIEEEST1A.tc1
        
          ExcIEEEST1A --> Seconds : ExcIEEEST1A.tc1
        
      ExcIEEEST1A : ExcIEEEST1A.tf
        
          ExcIEEEST1A --> Seconds : ExcIEEEST1A.tf
        
      ExcIEEEST1A : ExcIEEEST1A.uelin
        
          ExcIEEEST1A --> ExcIEEEST1AUELselectorKind : ExcIEEEST1A.uelin
        
      ExcIEEEST1A : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcIEEEST1A --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
      ExcIEEEST1A : ExcIEEEST1A.vamax
        
          ExcIEEEST1A --> PU : ExcIEEEST1A.vamax
        
      ExcIEEEST1A : ExcIEEEST1A.vamin
        
          ExcIEEEST1A --> PU : ExcIEEEST1A.vamin
        
      ExcIEEEST1A : ExcIEEEST1A.vimax
        
          ExcIEEEST1A --> PU : ExcIEEEST1A.vimax
        
      ExcIEEEST1A : ExcIEEEST1A.vimin
        
          ExcIEEEST1A --> PU : ExcIEEEST1A.vimin
        
      ExcIEEEST1A : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcIEEEST1A --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
      ExcIEEEST1A : ExcIEEEST1A.vrmax
        
          ExcIEEEST1A --> PU : ExcIEEEST1A.vrmax
        
      ExcIEEEST1A : ExcIEEEST1A.vrmin
        
          ExcIEEEST1A --> PU : ExcIEEEST1A.vrmin
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcIEEEST1A**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ilr | [cim:ExcIEEEST1A.ilr](http://iec.ch/TC57/CIM100#ExcIEEEST1A.ilr) | 1..1 <br />  [PU](PU.md)  | Exciter output current limit reference (<i>I</i><i><sub>LR</sub></i><i>)</i> | direct |
| ka | [cim:ExcIEEEST1A.ka](http://iec.ch/TC57/CIM100#ExcIEEEST1A.ka) | 1..1 <br />  [PU](PU.md)  | Voltage regulator gain (<i>K</i><i><sub>A</sub></i>) (&gt; 0) | direct |
| kc | [cim:ExcIEEEST1A.kc](http://iec.ch/TC57/CIM100#ExcIEEEST1A.kc) | 1..1 <br />  [PU](PU.md)  | Rectifier loading factor proportional to commutating reactance (<i>K</i><i><s... | direct |
| kf | [cim:ExcIEEEST1A.kf](http://iec.ch/TC57/CIM100#ExcIEEEST1A.kf) | 1..1 <br />  [PU](PU.md)  | Excitation control system stabilizer gains (<i>K</i><i><sub>F</sub></i>) (&gt... | direct |
| klr | [cim:ExcIEEEST1A.klr](http://iec.ch/TC57/CIM100#ExcIEEEST1A.klr) | 1..1 <br />  [PU](PU.md)  | Exciter output current limiter gain (<i>K</i><i><sub>LR</sub></i>) | direct |
| pssin | [cim:ExcIEEEST1A.pssin](http://iec.ch/TC57/CIM100#ExcIEEEST1A.pssin) | 1..1 <br />  boolean  | Selector of the Power System Stabilizer (PSS) input (<i>PSSin</i>) | direct |
| ta | [cim:ExcIEEEST1A.ta](http://iec.ch/TC57/CIM100#ExcIEEEST1A.ta) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>T</i><i><sub>A</sub></i>) (&gt;= 0) | direct |
| tb | [cim:ExcIEEEST1A.tb](http://iec.ch/TC57/CIM100#ExcIEEEST1A.tb) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>T</i><i><sub>B</sub></i>) (&gt;= 0) | direct |
| tb1 | [cim:ExcIEEEST1A.tb1](http://iec.ch/TC57/CIM100#ExcIEEEST1A.tb1) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>T</i><i><sub>B1</sub></i>) (&gt;= 0) | direct |
| tc | [cim:ExcIEEEST1A.tc](http://iec.ch/TC57/CIM100#ExcIEEEST1A.tc) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>T</i><i><sub>C</sub></i>) (&gt;= 0) | direct |
| tc1 | [cim:ExcIEEEST1A.tc1](http://iec.ch/TC57/CIM100#ExcIEEEST1A.tc1) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>T</i><i><sub>C1</sub></i>) (&gt;= 0) | direct |
| tf | [cim:ExcIEEEST1A.tf](http://iec.ch/TC57/CIM100#ExcIEEEST1A.tf) | 1..1 <br />  [Seconds](Seconds.md)  | Excitation control system stabilizer time constant (<i>T</i><i><sub>F</sub></... | direct |
| uelin | [cim:ExcIEEEST1A.uelin](http://iec.ch/TC57/CIM100#ExcIEEEST1A.uelin) | 1..1 <br />  [ExcIEEEST1AUELselectorKind](ExcIEEEST1AUELselectorKind.md)  | Selector of the connection of the UEL input (<i>UELin</i>) | direct |
| vamax | [cim:ExcIEEEST1A.vamax](http://iec.ch/TC57/CIM100#ExcIEEEST1A.vamax) | 1..1 <br />  [PU](PU.md)  | Maximum voltage regulator output (<i>V</i><i><sub>AMAX</sub></i>) (&gt; 0) | direct |
| vamin | [cim:ExcIEEEST1A.vamin](http://iec.ch/TC57/CIM100#ExcIEEEST1A.vamin) | 1..1 <br />  [PU](PU.md)  | Minimum voltage regulator output (<i>V</i><i><sub>AMIN</sub></i>) (&lt; 0) | direct |
| vimax | [cim:ExcIEEEST1A.vimax](http://iec.ch/TC57/CIM100#ExcIEEEST1A.vimax) | 1..1 <br />  [PU](PU.md)  | Maximum voltage regulator input limit (<i>V</i><i><sub>IMAX</sub></i>) (&gt; ... | direct |
| vimin | [cim:ExcIEEEST1A.vimin](http://iec.ch/TC57/CIM100#ExcIEEEST1A.vimin) | 1..1 <br />  [PU](PU.md)  | Minimum voltage regulator input limit (<i>V</i><i><sub>IMIN</sub></i>) (&lt; ... | direct |
| vrmax | [cim:ExcIEEEST1A.vrmax](http://iec.ch/TC57/CIM100#ExcIEEEST1A.vrmax) | 1..1 <br />  [PU](PU.md)  | Maximum voltage regulator outputs (<i>V</i><i><sub>RMAX</sub></i>) (&gt; 0) | direct |
| vrmin | [cim:ExcIEEEST1A.vrmin](http://iec.ch/TC57/CIM100#ExcIEEEST1A.vrmin) | 1..1 <br />  [PU](PU.md)  | Minimum voltage regulator outputs (<i>V</i><i><sub>RMIN</sub></i>) (&lt; 0) | direct |
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
| self | cim:ExcIEEEST1A |
| native | this:ExcIEEEST1A |




