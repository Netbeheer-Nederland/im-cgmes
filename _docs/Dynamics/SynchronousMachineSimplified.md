# SynchronousMachineSimplified


_The simplified model represents a synchronous generator as a constant internal voltage behind an impedance<i> </i>(<i>Rs + jXp</i>) as shown in the Simplified diagram._

_Since internal voltage is held constant, there is no <i>Efd</i> input and any excitation system model will be ignored.  There is also no <i>Ifd</i> output._

_This model should not be used for representing a real generator except, perhaps, small generators whose response is insignificant.  _

_The parameters used for the simplified model include:_

_- RotatingMachineDynamics.damping (<i>D</i>);_

_- RotatingMachineDynamics.inertia (<i>H</i>);_

_- RotatingMachineDynamics.statorLeakageReactance (used to exchange <i>jXp </i>for SynchronousMachineSimplified);_

_- RotatingMachineDynamics.statorResistance (<i>Rs</i>)._





**URI**: [cim:SynchronousMachineSimplified](http://iec.ch/TC57/CIM100#SynchronousMachineSimplified)<br />
**Type**: Class




```mermaid
 classDiagram
    class SynchronousMachineSimplified
      SynchronousMachineDynamics <|-- SynchronousMachineSimplified
      
      SynchronousMachineSimplified : SynchronousMachineDynamics.CrossCompoundTurbineGovernorDyanmics
        
          SynchronousMachineSimplified --> CrossCompoundTurbineGovernorDynamics : SynchronousMachineDynamics.CrossCompoundTurbineGovernorDyanmics
        
      SynchronousMachineSimplified : SynchronousMachineDynamics.CrossCompoundTurbineGovernorDynamics
        
          SynchronousMachineSimplified --> CrossCompoundTurbineGovernorDynamics : SynchronousMachineDynamics.CrossCompoundTurbineGovernorDynamics
        
      SynchronousMachineSimplified : RotatingMachineDynamics.damping
        
      SynchronousMachineSimplified : IdentifiedObject.description
        
      SynchronousMachineSimplified : DynamicsFunctionBlock.enabled
        
      SynchronousMachineSimplified : SynchronousMachineDynamics.ExcitationSystemDynamics
        
          SynchronousMachineSimplified --> ExcitationSystemDynamics : SynchronousMachineDynamics.ExcitationSystemDynamics
        
      SynchronousMachineSimplified : SynchronousMachineDynamics.GenICompensationForGenJ
        
          SynchronousMachineSimplified --> GenICompensationForGenJ : SynchronousMachineDynamics.GenICompensationForGenJ
        
      SynchronousMachineSimplified : RotatingMachineDynamics.inertia
        
          SynchronousMachineSimplified --> Seconds : RotatingMachineDynamics.inertia
        
      SynchronousMachineSimplified : SynchronousMachineDynamics.MechanicalLoadDynamics
        
          SynchronousMachineSimplified --> MechanicalLoadDynamics : SynchronousMachineDynamics.MechanicalLoadDynamics
        
      SynchronousMachineSimplified : IdentifiedObject.mRID
        
      SynchronousMachineSimplified : IdentifiedObject.name
        
      SynchronousMachineSimplified : RotatingMachineDynamics.saturationFactor
        
      SynchronousMachineSimplified : RotatingMachineDynamics.saturationFactor120
        
      SynchronousMachineSimplified : RotatingMachineDynamics.statorLeakageReactance
        
          SynchronousMachineSimplified --> PU : RotatingMachineDynamics.statorLeakageReactance
        
      SynchronousMachineSimplified : RotatingMachineDynamics.statorResistance
        
          SynchronousMachineSimplified --> PU : RotatingMachineDynamics.statorResistance
        
      SynchronousMachineSimplified : SynchronousMachineDynamics.SynchronousMachine
        
          SynchronousMachineSimplified --> SynchronousMachine : SynchronousMachineDynamics.SynchronousMachine
        
      SynchronousMachineSimplified : SynchronousMachineDynamics.TurbineGovernorDynamics
        
          SynchronousMachineSimplified --> TurbineGovernorDynamics : SynchronousMachineDynamics.TurbineGovernorDynamics
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [RotatingMachineDynamics](RotatingMachineDynamics.md)
            * [SynchronousMachineDynamics](SynchronousMachineDynamics.md)
                * **SynchronousMachineSimplified**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| SynchronousMachine | [cim:SynchronousMachineDynamics.SynchronousMachine](http://iec.ch/TC57/CIM100#SynchronousMachineDynamics.SynchronousMachine) | 1..1 <br />  [SynchronousMachine](SynchronousMachine.md)  | Synchronous machine to which synchronous machine dynamics model applies | [SynchronousMachineDynamics](SynchronousMachineDynamics.md) |
| CrossCompoundTurbineGovernorDyanmics | [cim:SynchronousMachineDynamics.CrossCompoundTurbineGovernorDyanmics](http://iec.ch/TC57/CIM100#SynchronousMachineDynamics.CrossCompoundTurbineGovernorDyanmics) | 0..1 <br />  [CrossCompoundTurbineGovernorDynamics](CrossCompoundTurbineGovernorDynamics.md)  | The cross-compound turbine governor with which this high-pressure synchronous... | [SynchronousMachineDynamics](SynchronousMachineDynamics.md) |
| CrossCompoundTurbineGovernorDynamics | [cim:SynchronousMachineDynamics.CrossCompoundTurbineGovernorDynamics](http://iec.ch/TC57/CIM100#SynchronousMachineDynamics.CrossCompoundTurbineGovernorDynamics) | 0..1 <br />  [CrossCompoundTurbineGovernorDynamics](CrossCompoundTurbineGovernorDynamics.md)  | The cross-compound turbine governor with which this low-pressure synchronous ... | [SynchronousMachineDynamics](SynchronousMachineDynamics.md) |
| MechanicalLoadDynamics | [cim:SynchronousMachineDynamics.MechanicalLoadDynamics](http://iec.ch/TC57/CIM100#SynchronousMachineDynamics.MechanicalLoadDynamics) | 0..1 <br />  [MechanicalLoadDynamics](MechanicalLoadDynamics.md)  | Mechanical load model associated with this synchronous machine model | [SynchronousMachineDynamics](SynchronousMachineDynamics.md) |
| ExcitationSystemDynamics | [cim:SynchronousMachineDynamics.ExcitationSystemDynamics](http://iec.ch/TC57/CIM100#SynchronousMachineDynamics.ExcitationSystemDynamics) | 0..1 <br />  [ExcitationSystemDynamics](ExcitationSystemDynamics.md)  | Excitation system model associated with this synchronous machine model | [SynchronousMachineDynamics](SynchronousMachineDynamics.md) |
| TurbineGovernorDynamics | [cim:SynchronousMachineDynamics.TurbineGovernorDynamics](http://iec.ch/TC57/CIM100#SynchronousMachineDynamics.TurbineGovernorDynamics) | 0..* <br />  [TurbineGovernorDynamics](TurbineGovernorDynamics.md)  | Turbine-governor model associated with this synchronous machine model | [SynchronousMachineDynamics](SynchronousMachineDynamics.md) |
| GenICompensationForGenJ | [cim:SynchronousMachineDynamics.GenICompensationForGenJ](http://iec.ch/TC57/CIM100#SynchronousMachineDynamics.GenICompensationForGenJ) | 0..* <br />  [GenICompensationForGenJ](GenICompensationForGenJ.md)  | Compensation of voltage compensator's generator for current flow out of this ... | [SynchronousMachineDynamics](SynchronousMachineDynamics.md) |
| damping | [cim:RotatingMachineDynamics.damping](http://iec.ch/TC57/CIM100#RotatingMachineDynamics.damping) | 1..1 <br />  float  | Damping torque coefficient (<i>D</i>) (&gt;= 0) | [RotatingMachineDynamics](RotatingMachineDynamics.md) |
| inertia | [cim:RotatingMachineDynamics.inertia](http://iec.ch/TC57/CIM100#RotatingMachineDynamics.inertia) | 1..1 <br />  [Seconds](Seconds.md)  | Inertia constant of generator or motor and mechanical load (<i>H</i>) (&gt; 0... | [RotatingMachineDynamics](RotatingMachineDynamics.md) |
| saturationFactor | [cim:RotatingMachineDynamics.saturationFactor](http://iec.ch/TC57/CIM100#RotatingMachineDynamics.saturationFactor) | 0..1 <br />  float  | Saturation factor at rated terminal voltage (<i>S1</i>) (&gt;= 0) | [RotatingMachineDynamics](RotatingMachineDynamics.md) |
| saturationFactor120 | [cim:RotatingMachineDynamics.saturationFactor120](http://iec.ch/TC57/CIM100#RotatingMachineDynamics.saturationFactor120) | 0..1 <br />  float  | Saturation factor at 120% of rated terminal voltage (<i>S12</i>) (&gt;= Rotat... | [RotatingMachineDynamics](RotatingMachineDynamics.md) |
| statorLeakageReactance | [cim:RotatingMachineDynamics.statorLeakageReactance](http://iec.ch/TC57/CIM100#RotatingMachineDynamics.statorLeakageReactance) | 1..1 <br />  [PU](PU.md)  | Stator leakage reactance (<i>Xl</i>) (&gt;= 0) | [RotatingMachineDynamics](RotatingMachineDynamics.md) |
| statorResistance | [cim:RotatingMachineDynamics.statorResistance](http://iec.ch/TC57/CIM100#RotatingMachineDynamics.statorResistance) | 1..1 <br />  [PU](PU.md)  | Stator (armature) resistance (<i>Rs</i>) (&gt;= 0) | [RotatingMachineDynamics](RotatingMachineDynamics.md) |
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
| self | cim:SynchronousMachineSimplified |
| native | this:SynchronousMachineSimplified |




