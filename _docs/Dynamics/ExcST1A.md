# ExcST1A


_Modification of an old IEEE ST1A static excitation system without overexcitation limiter (OEL) and underexcitation limiter (UEL)._





**URI**: [cim:ExcST1A](http://iec.ch/TC57/CIM100#ExcST1A)<br />
**Type**: Class




```mermaid
 classDiagram
    class ExcST1A
      ExcitationSystemDynamics <|-- ExcST1A
      
      ExcST1A : IdentifiedObject.description
        
      ExcST1A : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
          ExcST1A --> DiscontinuousExcitationControlDynamics : ExcitationSystemDynamics.DiscontinuousExcitationControlDynamics
        
      ExcST1A : DynamicsFunctionBlock.enabled
        
      ExcST1A : ExcST1A.ilr
        
          ExcST1A --> PU : ExcST1A.ilr
        
      ExcST1A : ExcST1A.ka
        
          ExcST1A --> PU : ExcST1A.ka
        
      ExcST1A : ExcST1A.kc
        
          ExcST1A --> PU : ExcST1A.kc
        
      ExcST1A : ExcST1A.kf
        
          ExcST1A --> PU : ExcST1A.kf
        
      ExcST1A : ExcST1A.klr
        
          ExcST1A --> PU : ExcST1A.klr
        
      ExcST1A : IdentifiedObject.mRID
        
      ExcST1A : IdentifiedObject.name
        
      ExcST1A : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
          ExcST1A --> OverexcitationLimiterDynamics : ExcitationSystemDynamics.OverexcitationLimiterDynamics
        
      ExcST1A : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
          ExcST1A --> PFVArControllerType1Dynamics : ExcitationSystemDynamics.PFVArControllerType1Dynamics
        
      ExcST1A : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
          ExcST1A --> PFVArControllerType2Dynamics : ExcitationSystemDynamics.PFVArControllerType2Dynamics
        
      ExcST1A : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
          ExcST1A --> PowerSystemStabilizerDynamics : ExcitationSystemDynamics.PowerSystemStabilizerDynamics
        
      ExcST1A : ExcitationSystemDynamics.SynchronousMachineDynamics
        
          ExcST1A --> SynchronousMachineDynamics : ExcitationSystemDynamics.SynchronousMachineDynamics
        
      ExcST1A : ExcST1A.ta
        
          ExcST1A --> Seconds : ExcST1A.ta
        
      ExcST1A : ExcST1A.tb
        
          ExcST1A --> Seconds : ExcST1A.tb
        
      ExcST1A : ExcST1A.tb1
        
          ExcST1A --> Seconds : ExcST1A.tb1
        
      ExcST1A : ExcST1A.tc
        
          ExcST1A --> Seconds : ExcST1A.tc
        
      ExcST1A : ExcST1A.tc1
        
          ExcST1A --> Seconds : ExcST1A.tc1
        
      ExcST1A : ExcST1A.tf
        
          ExcST1A --> Seconds : ExcST1A.tf
        
      ExcST1A : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
          ExcST1A --> UnderexcitationLimiterDynamics : ExcitationSystemDynamics.UnderexcitationLimiterDynamics
        
      ExcST1A : ExcST1A.vamax
        
          ExcST1A --> PU : ExcST1A.vamax
        
      ExcST1A : ExcST1A.vamin
        
          ExcST1A --> PU : ExcST1A.vamin
        
      ExcST1A : ExcST1A.vimax
        
          ExcST1A --> PU : ExcST1A.vimax
        
      ExcST1A : ExcST1A.vimin
        
          ExcST1A --> PU : ExcST1A.vimin
        
      ExcST1A : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
          ExcST1A --> VoltageCompensatorDynamics : ExcitationSystemDynamics.VoltageCompensatorDynamics
        
      ExcST1A : ExcST1A.vrmax
        
          ExcST1A --> PU : ExcST1A.vrmax
        
      ExcST1A : ExcST1A.vrmin
        
          ExcST1A --> PU : ExcST1A.vrmin
        
      ExcST1A : ExcST1A.xe
        
          ExcST1A --> PU : ExcST1A.xe
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [ExcitationSystemDynamics](ExcitationSystemDynamics.md)
            * **ExcST1A**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| vimax | [cim:ExcST1A.vimax](http://iec.ch/TC57/CIM100#ExcST1A.vimax) | 1..1 <br />  [PU](PU.md)  | Maximum voltage regulator input limit (<i>Vimax</i>) (&gt; 0) | direct |
| vimin | [cim:ExcST1A.vimin](http://iec.ch/TC57/CIM100#ExcST1A.vimin) | 1..1 <br />  [PU](PU.md)  | Minimum voltage regulator input limit (<i>Vimin</i>) (&lt; 0) | direct |
| tc | [cim:ExcST1A.tc](http://iec.ch/TC57/CIM100#ExcST1A.tc) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tc</i>) (&gt;= 0) | direct |
| tb | [cim:ExcST1A.tb](http://iec.ch/TC57/CIM100#ExcST1A.tb) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tb</i>) (&gt;= 0) | direct |
| ka | [cim:ExcST1A.ka](http://iec.ch/TC57/CIM100#ExcST1A.ka) | 1..1 <br />  [PU](PU.md)  | Voltage regulator gain (<i>Ka</i>) (&gt; 0) | direct |
| ta | [cim:ExcST1A.ta](http://iec.ch/TC57/CIM100#ExcST1A.ta) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Ta</i>) (&gt;= 0) | direct |
| vrmax | [cim:ExcST1A.vrmax](http://iec.ch/TC57/CIM100#ExcST1A.vrmax) | 1..1 <br />  [PU](PU.md)  | Maximum voltage regulator outputs (<i>Vrmax</i>) (&gt; 0)  | direct |
| vrmin | [cim:ExcST1A.vrmin](http://iec.ch/TC57/CIM100#ExcST1A.vrmin) | 1..1 <br />  [PU](PU.md)  | Minimum voltage regulator outputs (<i>Vrmin</i>) (&lt; 0) | direct |
| kc | [cim:ExcST1A.kc](http://iec.ch/TC57/CIM100#ExcST1A.kc) | 1..1 <br />  [PU](PU.md)  | Rectifier loading factor proportional to commutating reactance (<i>Kc</i>) (&... | direct |
| kf | [cim:ExcST1A.kf](http://iec.ch/TC57/CIM100#ExcST1A.kf) | 1..1 <br />  [PU](PU.md)  | Excitation control system stabilizer gains (<i>Kf</i>) (&gt;= 0) | direct |
| tf | [cim:ExcST1A.tf](http://iec.ch/TC57/CIM100#ExcST1A.tf) | 1..1 <br />  [Seconds](Seconds.md)  | Excitation control system stabilizer time constant (<i>Tf</i>) (&gt;= 0) | direct |
| tc1 | [cim:ExcST1A.tc1](http://iec.ch/TC57/CIM100#ExcST1A.tc1) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tc1</i>) (&gt;= 0) | direct |
| tb1 | [cim:ExcST1A.tb1](http://iec.ch/TC57/CIM100#ExcST1A.tb1) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage regulator time constant (<i>Tb1</i>) (&gt;= 0) | direct |
| vamax | [cim:ExcST1A.vamax](http://iec.ch/TC57/CIM100#ExcST1A.vamax) | 1..1 <br />  [PU](PU.md)  | Maximum voltage regulator output (<i>Vamax</i>) (&gt; 0) | direct |
| vamin | [cim:ExcST1A.vamin](http://iec.ch/TC57/CIM100#ExcST1A.vamin) | 1..1 <br />  [PU](PU.md)  | Minimum voltage regulator output (<i>Vamin</i>) (&lt; 0) | direct |
| ilr | [cim:ExcST1A.ilr](http://iec.ch/TC57/CIM100#ExcST1A.ilr) | 1..1 <br />  [PU](PU.md)  | Exciter output current limit reference (<i>Ilr</i>) | direct |
| klr | [cim:ExcST1A.klr](http://iec.ch/TC57/CIM100#ExcST1A.klr) | 1..1 <br />  [PU](PU.md)  | Exciter output current limiter gain (<i>Klr</i>) | direct |
| xe | [cim:ExcST1A.xe](http://iec.ch/TC57/CIM100#ExcST1A.xe) | 1..1 <br />  [PU](PU.md)  | Excitation xfmr effective reactance (<i>Xe</i>) | direct |
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
| self | cim:ExcST1A |
| native | this:ExcST1A |




