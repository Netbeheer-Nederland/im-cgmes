# GovSteamFV2


_Steam turbine governor with reheat time constants and modelling of the effects of fast valve closing to reduce mechanical power._





**URI**: [cim:GovSteamFV2](http://iec.ch/TC57/CIM100#GovSteamFV2)<br />
**Type**: Class




```mermaid
 classDiagram
    class GovSteamFV2
      TurbineGovernorDynamics <|-- GovSteamFV2
      
      GovSteamFV2 : TurbineGovernorDynamics.AsynchronousMachineDynamics
        
          GovSteamFV2 --> AsynchronousMachineDynamics : TurbineGovernorDynamics.AsynchronousMachineDynamics
        
      GovSteamFV2 : IdentifiedObject.description
        
      GovSteamFV2 : GovSteamFV2.dt
        
          GovSteamFV2 --> PU : GovSteamFV2.dt
        
      GovSteamFV2 : DynamicsFunctionBlock.enabled
        
      GovSteamFV2 : GovSteamFV2.k
        
          GovSteamFV2 --> PU : GovSteamFV2.k
        
      GovSteamFV2 : IdentifiedObject.mRID
        
      GovSteamFV2 : GovSteamFV2.mwbase
        
          GovSteamFV2 --> ActivePower : GovSteamFV2.mwbase
        
      GovSteamFV2 : IdentifiedObject.name
        
      GovSteamFV2 : GovSteamFV2.r
        
          GovSteamFV2 --> PU : GovSteamFV2.r
        
      GovSteamFV2 : TurbineGovernorDynamics.SynchronousMachineDynamics
        
          GovSteamFV2 --> SynchronousMachineDynamics : TurbineGovernorDynamics.SynchronousMachineDynamics
        
      GovSteamFV2 : GovSteamFV2.t1
        
          GovSteamFV2 --> Seconds : GovSteamFV2.t1
        
      GovSteamFV2 : GovSteamFV2.t3
        
          GovSteamFV2 --> Seconds : GovSteamFV2.t3
        
      GovSteamFV2 : GovSteamFV2.ta
        
          GovSteamFV2 --> Seconds : GovSteamFV2.ta
        
      GovSteamFV2 : GovSteamFV2.tb
        
          GovSteamFV2 --> Seconds : GovSteamFV2.tb
        
      GovSteamFV2 : GovSteamFV2.tc
        
          GovSteamFV2 --> Seconds : GovSteamFV2.tc
        
      GovSteamFV2 : GovSteamFV2.tt
        
          GovSteamFV2 --> Seconds : GovSteamFV2.tt
        
      GovSteamFV2 : TurbineGovernorDynamics.TurbineLoadControllerDynamics
        
          GovSteamFV2 --> TurbineLoadControllerDynamics : TurbineGovernorDynamics.TurbineLoadControllerDynamics
        
      GovSteamFV2 : GovSteamFV2.vmax
        
          GovSteamFV2 --> PU : GovSteamFV2.vmax
        
      GovSteamFV2 : GovSteamFV2.vmin
        
          GovSteamFV2 --> PU : GovSteamFV2.vmin
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [TurbineGovernorDynamics](TurbineGovernorDynamics.md)
            * **GovSteamFV2**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| mwbase | [cim:GovSteamFV2.mwbase](http://iec.ch/TC57/CIM100#GovSteamFV2.mwbase) | 1..1 <br />  [ActivePower](ActivePower.md)  | Alternate base used instead of machine base in equipment model if necessary (... | direct |
| t1 | [cim:GovSteamFV2.t1](http://iec.ch/TC57/CIM100#GovSteamFV2.t1) | 1..1 <br />  [Seconds](Seconds.md)  | Governor time constant (<i>T1</i>) (&gt;= 0) | direct |
| vmax | [cim:GovSteamFV2.vmax](http://iec.ch/TC57/CIM100#GovSteamFV2.vmax) | 1..1 <br />  [PU](PU.md)  | (<i>Vmax</i>) (&gt; GovSteamFV2 | direct |
| vmin | [cim:GovSteamFV2.vmin](http://iec.ch/TC57/CIM100#GovSteamFV2.vmin) | 1..1 <br />  [PU](PU.md)  | (<i>Vmin</i>) (&lt; GovSteamFV2 | direct |
| k | [cim:GovSteamFV2.k](http://iec.ch/TC57/CIM100#GovSteamFV2.k) | 1..1 <br />  [PU](PU.md)  | Fraction of the turbine power developed by turbine sections not involved in f... | direct |
| t3 | [cim:GovSteamFV2.t3](http://iec.ch/TC57/CIM100#GovSteamFV2.t3) | 1..1 <br />  [Seconds](Seconds.md)  | Reheater time constant (<i>T3</i>) (&gt;= 0) | direct |
| dt | [cim:GovSteamFV2.dt](http://iec.ch/TC57/CIM100#GovSteamFV2.dt) | 1..1 <br />  [PU](PU.md)  | (<i>Dt</i>) | direct |
| tt | [cim:GovSteamFV2.tt](http://iec.ch/TC57/CIM100#GovSteamFV2.tt) | 1..1 <br />  [Seconds](Seconds.md)  | Time constant with which power falls off after intercept valve closure (<i>Tt... | direct |
| r | [cim:GovSteamFV2.r](http://iec.ch/TC57/CIM100#GovSteamFV2.r) | 1..1 <br />  [PU](PU.md)  | (<i>R</i>) | direct |
| ta | [cim:GovSteamFV2.ta](http://iec.ch/TC57/CIM100#GovSteamFV2.ta) | 1..1 <br />  [Seconds](Seconds.md)  | Time after initial time for valve to close (<i>Ta</i>) (&gt;= 0) | direct |
| tb | [cim:GovSteamFV2.tb](http://iec.ch/TC57/CIM100#GovSteamFV2.tb) | 1..1 <br />  [Seconds](Seconds.md)  | Time after initial time for valve to begin opening (<i>Tb</i>) (&gt;= 0) | direct |
| tc | [cim:GovSteamFV2.tc](http://iec.ch/TC57/CIM100#GovSteamFV2.tc) | 1..1 <br />  [Seconds](Seconds.md)  | Time after initial time for valve to become fully open (<i>Tc</i>) (&gt;= 0) | direct |
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
| self | cim:GovSteamFV2 |
| native | this:GovSteamFV2 |




