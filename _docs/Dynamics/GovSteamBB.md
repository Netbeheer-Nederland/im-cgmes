# GovSteamBB


_European governor model._





**URI**: [cim:GovSteamBB](http://iec.ch/TC57/CIM100#GovSteamBB)<br />
**Type**: Class




```mermaid
 classDiagram
    class GovSteamBB
      TurbineGovernorDynamics <|-- GovSteamBB
      
      GovSteamBB : TurbineGovernorDynamics.AsynchronousMachineDynamics
        
          GovSteamBB --> AsynchronousMachineDynamics : TurbineGovernorDynamics.AsynchronousMachineDynamics
        
      GovSteamBB : IdentifiedObject.description
        
      GovSteamBB : DynamicsFunctionBlock.enabled
        
      GovSteamBB : GovSteamBB.fcut
        
          GovSteamBB --> PU : GovSteamBB.fcut
        
      GovSteamBB : GovSteamBB.k2
        
          GovSteamBB --> PU : GovSteamBB.k2
        
      GovSteamBB : GovSteamBB.k3
        
          GovSteamBB --> PU : GovSteamBB.k3
        
      GovSteamBB : GovSteamBB.kd
        
          GovSteamBB --> PU : GovSteamBB.kd
        
      GovSteamBB : GovSteamBB.kg
        
          GovSteamBB --> PU : GovSteamBB.kg
        
      GovSteamBB : GovSteamBB.kls
        
          GovSteamBB --> PU : GovSteamBB.kls
        
      GovSteamBB : GovSteamBB.kp
        
          GovSteamBB --> PU : GovSteamBB.kp
        
      GovSteamBB : GovSteamBB.ks
        
          GovSteamBB --> PU : GovSteamBB.ks
        
      GovSteamBB : IdentifiedObject.mRID
        
      GovSteamBB : IdentifiedObject.name
        
      GovSteamBB : GovSteamBB.peflag
        
      GovSteamBB : GovSteamBB.pmax
        
          GovSteamBB --> PU : GovSteamBB.pmax
        
      GovSteamBB : GovSteamBB.pmin
        
          GovSteamBB --> PU : GovSteamBB.pmin
        
      GovSteamBB : TurbineGovernorDynamics.SynchronousMachineDynamics
        
          GovSteamBB --> SynchronousMachineDynamics : TurbineGovernorDynamics.SynchronousMachineDynamics
        
      GovSteamBB : GovSteamBB.t1
        
          GovSteamBB --> Seconds : GovSteamBB.t1
        
      GovSteamBB : GovSteamBB.t4
        
          GovSteamBB --> Seconds : GovSteamBB.t4
        
      GovSteamBB : GovSteamBB.t5
        
          GovSteamBB --> Seconds : GovSteamBB.t5
        
      GovSteamBB : GovSteamBB.t6
        
          GovSteamBB --> Seconds : GovSteamBB.t6
        
      GovSteamBB : GovSteamBB.td
        
          GovSteamBB --> Seconds : GovSteamBB.td
        
      GovSteamBB : GovSteamBB.tn
        
          GovSteamBB --> Seconds : GovSteamBB.tn
        
      GovSteamBB : TurbineGovernorDynamics.TurbineLoadControllerDynamics
        
          GovSteamBB --> TurbineLoadControllerDynamics : TurbineGovernorDynamics.TurbineLoadControllerDynamics
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [TurbineGovernorDynamics](TurbineGovernorDynamics.md)
            * **GovSteamBB**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| fcut | [cim:GovSteamBB.fcut](http://iec.ch/TC57/CIM100#GovSteamBB.fcut) | 1..1 <br />  [PU](PU.md)  | Frequency deadband (<i>f</i><i><sub>cut</sub></i>) (&gt;= 0) | direct |
| ks | [cim:GovSteamBB.ks](http://iec.ch/TC57/CIM100#GovSteamBB.ks) | 1..1 <br />  [PU](PU.md)  | Gain (<i>Ks</i>) | direct |
| kls | [cim:GovSteamBB.kls](http://iec.ch/TC57/CIM100#GovSteamBB.kls) | 1..1 <br />  [PU](PU.md)  | Gain (<i>Kls</i>) (&gt; 0) | direct |
| kg | [cim:GovSteamBB.kg](http://iec.ch/TC57/CIM100#GovSteamBB.kg) | 1..1 <br />  [PU](PU.md)  | Gain (<i>Kg</i>) | direct |
| t1 | [cim:GovSteamBB.t1](http://iec.ch/TC57/CIM100#GovSteamBB.t1) | 1..1 <br />  [Seconds](Seconds.md)  | Time constant (<i>T1</i>) | direct |
| kp | [cim:GovSteamBB.kp](http://iec.ch/TC57/CIM100#GovSteamBB.kp) | 1..1 <br />  [PU](PU.md)  | Gain (<i>Kp</i>) | direct |
| tn | [cim:GovSteamBB.tn](http://iec.ch/TC57/CIM100#GovSteamBB.tn) | 1..1 <br />  [Seconds](Seconds.md)  | Time constant (<i>Tn</i>) (&gt; 0) | direct |
| kd | [cim:GovSteamBB.kd](http://iec.ch/TC57/CIM100#GovSteamBB.kd) | 1..1 <br />  [PU](PU.md)  | Gain (<i>Kd</i>) | direct |
| td | [cim:GovSteamBB.td](http://iec.ch/TC57/CIM100#GovSteamBB.td) | 1..1 <br />  [Seconds](Seconds.md)  | Time constant (<i>Td</i>) (&gt; 0) | direct |
| pmax | [cim:GovSteamBB.pmax](http://iec.ch/TC57/CIM100#GovSteamBB.pmax) | 1..1 <br />  [PU](PU.md)  | High power limit (<i>Pmax</i>) (&gt; GovSteamBB | direct |
| pmin | [cim:GovSteamBB.pmin](http://iec.ch/TC57/CIM100#GovSteamBB.pmin) | 1..1 <br />  [PU](PU.md)  | Low power limit (<i>Pmin</i>) (&lt; GovSteamBB | direct |
| t4 | [cim:GovSteamBB.t4](http://iec.ch/TC57/CIM100#GovSteamBB.t4) | 1..1 <br />  [Seconds](Seconds.md)  | Time constant (<i>T4</i>) | direct |
| k2 | [cim:GovSteamBB.k2](http://iec.ch/TC57/CIM100#GovSteamBB.k2) | 1..1 <br />  [PU](PU.md)  | Gain (<i>K2</i>) | direct |
| t5 | [cim:GovSteamBB.t5](http://iec.ch/TC57/CIM100#GovSteamBB.t5) | 1..1 <br />  [Seconds](Seconds.md)  | Time constant (<i>T5</i>) | direct |
| k3 | [cim:GovSteamBB.k3](http://iec.ch/TC57/CIM100#GovSteamBB.k3) | 1..1 <br />  [PU](PU.md)  | Gain (<i>K3</i>) | direct |
| t6 | [cim:GovSteamBB.t6](http://iec.ch/TC57/CIM100#GovSteamBB.t6) | 1..1 <br />  [Seconds](Seconds.md)  | Time constant (<i>T6</i>) | direct |
| peflag | [cim:GovSteamBB.peflag](http://iec.ch/TC57/CIM100#GovSteamBB.peflag) | 1..1 <br />  boolean  | Electric power input selection (Peflag) | direct |
| SynchronousMachineDynamics | [cim:TurbineGovernorDynamics.SynchronousMachineDynamics](http://iec.ch/TC57/CIM100#TurbineGovernorDynamics.SynchronousMachineDynamics) | 0..1 <br />  [SynchronousMachineDynamics](SynchronousMachineDynamics.md)  | Synchronous machine model with which this turbine-governor model is associate... | [TurbineGovernorDynamics](TurbineGovernorDynamics.md) |
| AsynchronousMachineDynamics | [cim:TurbineGovernorDynamics.AsynchronousMachineDynamics](http://iec.ch/TC57/CIM100#TurbineGovernorDynamics.AsynchronousMachineDynamics) | 0..1 <br />  [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md)  | Asynchronous machine model with which this turbine-governor model is associat... | [TurbineGovernorDynamics](TurbineGovernorDynamics.md) |
| TurbineLoadControllerDynamics | [cim:TurbineGovernorDynamics.TurbineLoadControllerDynamics](http://iec.ch/TC57/CIM100#TurbineGovernorDynamics.TurbineLoadControllerDynamics) | 0..1 <br />  [TurbineLoadControllerDynamics](TurbineLoadControllerDynamics.md)  | Turbine load controller providing input to this turbine-governor | [TurbineGovernorDynamics](TurbineGovernorDynamics.md) |
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
| self | cim:GovSteamBB |
| native | this:GovSteamBB |




