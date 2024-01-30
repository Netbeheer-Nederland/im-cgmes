# ExcAC4A


_Modified IEEE AC4A alternator-supplied rectifier excitation system with different minimum controller output._





**URI**: [cim:ExcAC4A](http://iec.ch/TC57/CIM100#ExcAC4A)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcAC4A
      ExcitationSystemDynamics <|-- ExcAC4A
      
      ExcAC4A : IdentifiedObject.description
        
      ExcAC4A : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcAC4A --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
      ExcAC4A : DynamicsFunctionBlock.enabled
        
      ExcAC4A : ExcAC4A.ka
        
          ExcAC4A --> PU : ExcAC4A.ka
        
      ExcAC4A : ExcAC4A.kc
        
          ExcAC4A --> PU : ExcAC4A.kc
        
      ExcAC4A : IdentifiedObject.mRID
        
      ExcAC4A : IdentifiedObject.name
        
      ExcAC4A : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcAC4A --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
      ExcAC4A : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcAC4A --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
      ExcAC4A : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcAC4A --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
      ExcAC4A : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcAC4A --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
      ExcAC4A : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcAC4A --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
        
      ExcAC4A : ExcAC4A.ta
        
          ExcAC4A --> Seconds : ExcAC4A.ta
        
      ExcAC4A : ExcAC4A.tb
        
          ExcAC4A --> Seconds : ExcAC4A.tb
        
      ExcAC4A : ExcAC4A.tc
        
          ExcAC4A --> Seconds : ExcAC4A.tc
        
      ExcAC4A : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcAC4A --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
      ExcAC4A : ExcAC4A.vimax
        
          ExcAC4A --> PU : ExcAC4A.vimax
        
      ExcAC4A : ExcAC4A.vimin
        
          ExcAC4A --> PU : ExcAC4A.vimin
        
      ExcAC4A : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcAC4A --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
      ExcAC4A : ExcAC4A.vrmax
        
          ExcAC4A --> PU : ExcAC4A.vrmax
        
      ExcAC4A : ExcAC4A.vrmin
        
          ExcAC4A --> PU : ExcAC4A.vrmin
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcAC4A**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| vimax | [cim:ExcAC4A.vimax](http://iec.ch/TC57/CIM100#ExcAC4A.vimax) | 1..1 <br />  [PU](PU.md)  | Maximum voltage regulator input limit (<i>Vimax</i>)  (&gt; 0) | direct |
| vimin | [cim:ExcAC4A.vimin](http://iec.ch/TC57/CIM100#ExcAC4A.vimin) | 1..1 <br />  [PU](PU.md)  | Minimum voltage regulator input limit (<i>Vimin</i>) (&lt; 0) | direct |
| tc | [cim:ExcAC4A.tc](http://iec.ch/TC57/CIM100#ExcAC4A.tc) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tc</i>) (&gt;= 0) | direct |
| tb | [cim:ExcAC4A.tb](http://iec.ch/TC57/CIM100#ExcAC4A.tb) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tb</i>) (&gt;= 0) | direct |
| ka | [cim:ExcAC4A.ka](http://iec.ch/TC57/CIM100#ExcAC4A.ka) | 1..1 <br />  [PU](PU.md)  | Voltage regulator gain (<i>Ka</i>) (&gt; 0) | direct |
| ta | [cim:ExcAC4A.ta](http://iec.ch/TC57/CIM100#ExcAC4A.ta) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Ta</i>) (&gt; 0) | direct |
| vrmax | [cim:ExcAC4A.vrmax](http://iec.ch/TC57/CIM100#ExcAC4A.vrmax) | 1..1 <br />  [PU](PU.md)  | Maximum voltage regulator output (<i>Vrmax</i>) (&gt; 0) | direct |
| vrmin | [cim:ExcAC4A.vrmin](http://iec.ch/TC57/CIM100#ExcAC4A.vrmin) | 1..1 <br />  [PU](PU.md)  | Minimum voltage regulator output (<i>Vrmin</i>) (&lt; 0) | direct |
| kc | [cim:ExcAC4A.kc](http://iec.ch/TC57/CIM100#ExcAC4A.kc) | 1..1 <br />  [PU](PU.md)  | Rectifier loading factor proportional to commutating reactance (<i>Kc</i>) (&... | direct |
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
| self | cim:ExcAC4A |
| native | this:ExcAC4A |




