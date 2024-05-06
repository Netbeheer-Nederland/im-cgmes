# GovGAST


_Single shaft gas turbine._





**URI**: [cim:GovGAST](http://iec.ch/TC57/CIM100#GovGAST)<br />
**Type**: Class




```mermaid
 classDiagram
    class GovGAST
    click GovGAST href "../GovGAST"
      TurbineGovernorDynamics <|-- GovGAST
        click TurbineGovernorDynamics href "../TurbineGovernorDynamics"
      
      GovGAST : TurbineGovernorDynamics.AsynchronousMachineDynamics
        
          GovGAST --> AsynchronousMachineDynamics : TurbineGovernorDynamics.AsynchronousMachineDynamics
          click AsynchronousMachineDynamics href "../AsynchronousMachineDynamics"
        
      GovGAST : GovGAST.at
        
          GovGAST --> PU : GovGAST.at
          click PU href "../PU"
        
      GovGAST : IdentifiedObject.description
        
      GovGAST : GovGAST.dturb
        
          GovGAST --> PU : GovGAST.dturb
          click PU href "../PU"
        
      GovGAST : DynamicsFunctionBlock.enabled
        
      GovGAST : GovGAST.kt
        
          GovGAST --> PU : GovGAST.kt
          click PU href "../PU"
        
      GovGAST : IdentifiedObject.mRID
        
      GovGAST : GovGAST.mwbase
        
          GovGAST --> ActivePower : GovGAST.mwbase
          click ActivePower href "../ActivePower"
        
      GovGAST : IdentifiedObject.name
        
      GovGAST : GovGAST.r
        
          GovGAST --> PU : GovGAST.r
          click PU href "../PU"
        
      GovGAST : TurbineGovernorDynamics.SynchronousMachineDynamics
        
          GovGAST --> SynchronousMachineDynamics : TurbineGovernorDynamics.SynchronousMachineDynamics
          click SynchronousMachineDynamics href "../SynchronousMachineDynamics"
        
      GovGAST : GovGAST.t1
        
          GovGAST --> Seconds : GovGAST.t1
          click Seconds href "../Seconds"
        
      GovGAST : GovGAST.t2
        
          GovGAST --> Seconds : GovGAST.t2
          click Seconds href "../Seconds"
        
      GovGAST : GovGAST.t3
        
          GovGAST --> Seconds : GovGAST.t3
          click Seconds href "../Seconds"
        
      GovGAST : TurbineGovernorDynamics.TurbineLoadControllerDynamics
        
          GovGAST --> TurbineLoadControllerDynamics : TurbineGovernorDynamics.TurbineLoadControllerDynamics
          click TurbineLoadControllerDynamics href "../TurbineLoadControllerDynamics"
        
      GovGAST : GovGAST.vmax
        
          GovGAST --> PU : GovGAST.vmax
          click PU href "../PU"
        
      GovGAST : GovGAST.vmin
        
          GovGAST --> PU : GovGAST.vmin
          click PU href "../PU"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [TurbineGovernorDynamics](TurbineGovernorDynamics.md)
            * **GovGAST**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| mwbase | [cim:GovGAST.mwbase](http://iec.ch/TC57/CIM100#GovGAST.mwbase) | 1 <br />  [ActivePower](ActivePower.md)  | Base for power values (<i>MWbase</i>) (&gt; 0) | direct |
| r | [cim:GovGAST.r](http://iec.ch/TC57/CIM100#GovGAST.r) | 1 <br />  [PU](PU.md)  | Permanent droop (<i>R</i>) (&gt;0) | direct |
| t1 | [cim:GovGAST.t1](http://iec.ch/TC57/CIM100#GovGAST.t1) | 1 <br />  [Seconds](Seconds.md)  | Governor mechanism time constant (<i>T1</i>) (&gt;= 0) | direct |
| t2 | [cim:GovGAST.t2](http://iec.ch/TC57/CIM100#GovGAST.t2) | 1 <br />  [Seconds](Seconds.md)  | Turbine power time constant (<i>T2</i>) (&gt;= 0) | direct |
| t3 | [cim:GovGAST.t3](http://iec.ch/TC57/CIM100#GovGAST.t3) | 1 <br />  [Seconds](Seconds.md)  | Turbine exhaust temperature time constant (<i>T3</i>) (&gt;= 0) | direct |
| at | [cim:GovGAST.at](http://iec.ch/TC57/CIM100#GovGAST.at) | 1 <br />  [PU](PU.md)  | Ambient temperature load limit (<i>Load Limit</i>) | direct |
| kt | [cim:GovGAST.kt](http://iec.ch/TC57/CIM100#GovGAST.kt) | 1 <br />  [PU](PU.md)  | Temperature limiter gain (<i>Kt</i>) | direct |
| vmax | [cim:GovGAST.vmax](http://iec.ch/TC57/CIM100#GovGAST.vmax) | 1 <br />  [PU](PU.md)  | Maximum turbine power, PU of MWbase (<i>Vmax</i>) (&gt; GovGAST | direct |
| vmin | [cim:GovGAST.vmin](http://iec.ch/TC57/CIM100#GovGAST.vmin) | 1 <br />  [PU](PU.md)  | Minimum turbine power, PU of MWbase (<i>Vmin</i>) (&lt; GovGAST | direct |
| dturb | [cim:GovGAST.dturb](http://iec.ch/TC57/CIM100#GovGAST.dturb) | 1 <br />  [PU](PU.md)  | Turbine damping factor (<i>Dturb</i>) | direct |
| SynchronousMachineDynamics | [cim:TurbineGovernorDynamics.SynchronousMachineDynamics](http://iec.ch/TC57/CIM100#TurbineGovernorDynamics.SynchronousMachineDynamics) | 0..1 <br />  [SynchronousMachineDynamics](SynchronousMachineDynamics.md)  | Synchronous machine model with which this turbine-governor model is associate... | [TurbineGovernorDynamics](TurbineGovernorDynamics.md) |
| AsynchronousMachineDynamics | [cim:TurbineGovernorDynamics.AsynchronousMachineDynamics](http://iec.ch/TC57/CIM100#TurbineGovernorDynamics.AsynchronousMachineDynamics) | 0..1 <br />  [AsynchronousMachineDynamics](AsynchronousMachineDynamics.md)  | Asynchronous machine model with which this turbine-governor model is associat... | [TurbineGovernorDynamics](TurbineGovernorDynamics.md) |
| TurbineLoadControllerDynamics | [cim:TurbineGovernorDynamics.TurbineLoadControllerDynamics](http://iec.ch/TC57/CIM100#TurbineGovernorDynamics.TurbineLoadControllerDynamics) | 0..1 <br />  [TurbineLoadControllerDynamics](TurbineLoadControllerDynamics.md)  | Turbine load controller providing input to this turbine-governor | [TurbineGovernorDynamics](TurbineGovernorDynamics.md) |
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
| self | cim:GovGAST |
| native | this:GovGAST |




