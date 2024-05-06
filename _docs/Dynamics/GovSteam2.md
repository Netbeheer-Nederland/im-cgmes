# GovSteam2


_Simplified governor._





**URI**: [cim:GovSteam2](http://iec.ch/TC57/CIM100#GovSteam2)<br />
**Type**: Class




```mermaid
 classDiagram
    class GovSteam2
    click GovSteam2 href "../GovSteam2"
      TurbineGovernorDynamics <|-- GovSteam2
        click TurbineGovernorDynamics href "../TurbineGovernorDynamics"
      
      GovSteam2 : TurbineGovernorDynamics.AsynchronousMachineDynamics
        
          GovSteam2 --> AsynchronousMachineDynamics : TurbineGovernorDynamics.AsynchronousMachineDynamics
          click AsynchronousMachineDynamics href "../AsynchronousMachineDynamics"
        
      GovSteam2 : GovSteam2.dbf
        
          GovSteam2 --> PU : GovSteam2.dbf
          click PU href "../PU"
        
      GovSteam2 : IdentifiedObject.description
        
      GovSteam2 : DynamicsFunctionBlock.enabled
        
      GovSteam2 : GovSteam2.k
        
      GovSteam2 : GovSteam2.mnef
        
          GovSteam2 --> PU : GovSteam2.mnef
          click PU href "../PU"
        
      GovSteam2 : IdentifiedObject.mRID
        
      GovSteam2 : GovSteam2.mxef
        
          GovSteam2 --> PU : GovSteam2.mxef
          click PU href "../PU"
        
      GovSteam2 : IdentifiedObject.name
        
      GovSteam2 : GovSteam2.pmax
        
          GovSteam2 --> PU : GovSteam2.pmax
          click PU href "../PU"
        
      GovSteam2 : GovSteam2.pmin
        
          GovSteam2 --> PU : GovSteam2.pmin
          click PU href "../PU"
        
      GovSteam2 : TurbineGovernorDynamics.SynchronousMachineDynamics
        
          GovSteam2 --> SynchronousMachineDynamics : TurbineGovernorDynamics.SynchronousMachineDynamics
          click SynchronousMachineDynamics href "../SynchronousMachineDynamics"
        
      GovSteam2 : GovSteam2.t1
        
          GovSteam2 --> Seconds : GovSteam2.t1
          click Seconds href "../Seconds"
        
      GovSteam2 : GovSteam2.t2
        
          GovSteam2 --> Seconds : GovSteam2.t2
          click Seconds href "../Seconds"
        
      GovSteam2 : TurbineGovernorDynamics.TurbineLoadControllerDynamics
        
          GovSteam2 --> TurbineLoadControllerDynamics : TurbineGovernorDynamics.TurbineLoadControllerDynamics
          click TurbineLoadControllerDynamics href "../TurbineLoadControllerDynamics"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [DynamicsFunctionBlock](DynamicsFunctionBlock.md)
        * [TurbineGovernorDynamics](TurbineGovernorDynamics.md)
            * **GovSteam2**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| k | [cim:GovSteam2.k](http://iec.ch/TC57/CIM100#GovSteam2.k) | 1 <br />  float  | Governor gain (reciprocal of droop) (<i>K</i>) | direct |
| dbf | [cim:GovSteam2.dbf](http://iec.ch/TC57/CIM100#GovSteam2.dbf) | 1 <br />  [PU](PU.md)  | Frequency deadband (<i>DBF</i>) | direct |
| t1 | [cim:GovSteam2.t1](http://iec.ch/TC57/CIM100#GovSteam2.t1) | 1 <br />  [Seconds](Seconds.md)  | Governor lag time constant (<i>T</i><i><sub>1</sub></i>) (&gt; 0) | direct |
| t2 | [cim:GovSteam2.t2](http://iec.ch/TC57/CIM100#GovSteam2.t2) | 1 <br />  [Seconds](Seconds.md)  | Governor lead time constant (<i>T</i><i><sub>2</sub></i>) (&gt;= 0) | direct |
| pmax | [cim:GovSteam2.pmax](http://iec.ch/TC57/CIM100#GovSteam2.pmax) | 1 <br />  [PU](PU.md)  | Maximum fuel flow (<i>P</i><i><sub>MAX</sub></i>) (&gt; GovSteam2 | direct |
| pmin | [cim:GovSteam2.pmin](http://iec.ch/TC57/CIM100#GovSteam2.pmin) | 1 <br />  [PU](PU.md)  | Minimum fuel flow (<i>P</i><i><sub>MIN</sub></i>) (&lt; GovSteam2 | direct |
| mxef | [cim:GovSteam2.mxef](http://iec.ch/TC57/CIM100#GovSteam2.mxef) | 1 <br />  [PU](PU.md)  | Fuel flow maximum positive error value (<i>MX</i><i><sub>EF</sub></i>) | direct |
| mnef | [cim:GovSteam2.mnef](http://iec.ch/TC57/CIM100#GovSteam2.mnef) | 1 <br />  [PU](PU.md)  | Fuel flow maximum negative error value (<i>MN</i><i><sub>EF</sub></i>) | direct |
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
| self | cim:GovSteam2 |
| native | this:GovSteam2 |




