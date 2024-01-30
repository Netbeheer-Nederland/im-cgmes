# WindPitchContPowerIEC


_Pitch control power model._

_Reference: IEC 61400-27-1:2015, 5.6.5.1._





**URI**: [cim:WindPitchContPowerIEC](http://iec.ch/TC57/CIM100#WindPitchContPowerIEC)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindPitchContPowerIEC
      IdentifiedObject <|-- WindPitchContPowerIEC
      
      WindPitchContPowerIEC : IdentifiedObject.description
        
      WindPitchContPowerIEC : WindPitchContPowerIEC.dpmax
        
          WindPitchContPowerIEC --> PU : WindPitchContPowerIEC.dpmax
        
      WindPitchContPowerIEC : WindPitchContPowerIEC.dpmin
        
          WindPitchContPowerIEC --> PU : WindPitchContPowerIEC.dpmin
        
      WindPitchContPowerIEC : IdentifiedObject.mRID
        
      WindPitchContPowerIEC : IdentifiedObject.name
        
      WindPitchContPowerIEC : WindPitchContPowerIEC.pmin
        
          WindPitchContPowerIEC --> PU : WindPitchContPowerIEC.pmin
        
      WindPitchContPowerIEC : WindPitchContPowerIEC.pset
        
          WindPitchContPowerIEC --> PU : WindPitchContPowerIEC.pset
        
      WindPitchContPowerIEC : WindPitchContPowerIEC.t1
        
          WindPitchContPowerIEC --> Seconds : WindPitchContPowerIEC.t1
        
      WindPitchContPowerIEC : WindPitchContPowerIEC.tr
        
          WindPitchContPowerIEC --> Seconds : WindPitchContPowerIEC.tr
        
      WindPitchContPowerIEC : WindPitchContPowerIEC.uuvrt
        
          WindPitchContPowerIEC --> PU : WindPitchContPowerIEC.uuvrt
        
      WindPitchContPowerIEC : WindPitchContPowerIEC.WindDynamicsLookupTable
        
          WindPitchContPowerIEC --> WindDynamicsLookupTable : WindPitchContPowerIEC.WindDynamicsLookupTable
        
      WindPitchContPowerIEC : WindPitchContPowerIEC.WindGenTurbineType1bIEC
        
          WindPitchContPowerIEC --> WindGenTurbineType1bIEC : WindPitchContPowerIEC.WindGenTurbineType1bIEC
        
      WindPitchContPowerIEC : WindPitchContPowerIEC.WindGenTurbineType2IEC
        
          WindPitchContPowerIEC --> WindGenTurbineType2IEC : WindPitchContPowerIEC.WindGenTurbineType2IEC
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **WindPitchContPowerIEC**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| WindDynamicsLookupTable | [cim:WindPitchContPowerIEC.WindDynamicsLookupTable](http://iec.ch/TC57/CIM100#WindPitchContPowerIEC.WindDynamicsLookupTable) | 1..* <br />  [WindDynamicsLookupTable](WindDynamicsLookupTable.md)  | The wind dynamics lookup table associated with this pitch control power model | direct |
| WindGenTurbineType1bIEC | [cim:WindPitchContPowerIEC.WindGenTurbineType1bIEC](http://iec.ch/TC57/CIM100#WindPitchContPowerIEC.WindGenTurbineType1bIEC) | 0..1 <br />  [WindGenTurbineType1bIEC](WindGenTurbineType1bIEC.md)  | Wind turbine type 1B model with which this pitch control power model is assoc... | direct |
| WindGenTurbineType2IEC | [cim:WindPitchContPowerIEC.WindGenTurbineType2IEC](http://iec.ch/TC57/CIM100#WindPitchContPowerIEC.WindGenTurbineType2IEC) | 0..1 <br />  [WindGenTurbineType2IEC](WindGenTurbineType2IEC.md)  | Wind turbine type 2 model with which this pitch control power model is associ... | direct |
| dpmax | [cim:WindPitchContPowerIEC.dpmax](http://iec.ch/TC57/CIM100#WindPitchContPowerIEC.dpmax) | 1..1 <br />  [PU](PU.md)  | Rate limit for increasing power (<i>dp</i><i><sub>max</sub></i>) (&gt; WindPi... | direct |
| dpmin | [cim:WindPitchContPowerIEC.dpmin](http://iec.ch/TC57/CIM100#WindPitchContPowerIEC.dpmin) | 1..1 <br />  [PU](PU.md)  | Rate limit for decreasing power (<i>dp</i><i><sub>min</sub></i>) (&lt; WindPi... | direct |
| pmin | [cim:WindPitchContPowerIEC.pmin](http://iec.ch/TC57/CIM100#WindPitchContPowerIEC.pmin) | 1..1 <br />  [PU](PU.md)  | Minimum power setting (<i>p</i><i><sub>min</sub></i>) | direct |
| pset | [cim:WindPitchContPowerIEC.pset](http://iec.ch/TC57/CIM100#WindPitchContPowerIEC.pset) | 1..1 <br />  [PU](PU.md)  | If <i>p</i><i><sub>init</sub></i><sub> </sub>&lt; <i>p</i><i><sub>set</sub></... | direct |
| t1 | [cim:WindPitchContPowerIEC.t1](http://iec.ch/TC57/CIM100#WindPitchContPowerIEC.t1) | 1..1 <br />  [Seconds](Seconds.md)  | Lag time constant (<i>T</i><i><sub>1</sub></i>) (&gt;= 0) | direct |
| tr | [cim:WindPitchContPowerIEC.tr](http://iec.ch/TC57/CIM100#WindPitchContPowerIEC.tr) | 1..1 <br />  [Seconds](Seconds.md)  | Voltage measurement time constant (<i>T</i><i><sub>r</sub></i>) (&gt;= 0) | direct |
| uuvrt | [cim:WindPitchContPowerIEC.uuvrt](http://iec.ch/TC57/CIM100#WindPitchContPowerIEC.uuvrt) | 1..1 <br />  [PU](PU.md)  | Dip detection threshold (<i>u</i><i><sub>UVRT</sub></i>) | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [WindDynamicsLookupTable](WindDynamicsLookupTable.md) | WindPitchContPowerIEC | range | [WindPitchContPowerIEC](WindPitchContPowerIEC.md) |
| [WindGenTurbineType1bIEC](WindGenTurbineType1bIEC.md) | WindPitchContPowerIEC | range | [WindPitchContPowerIEC](WindPitchContPowerIEC.md) |
| [WindGenTurbineType2IEC](WindGenTurbineType2IEC.md) | WindPitchContPowerIEC | range | [WindPitchContPowerIEC](WindPitchContPowerIEC.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindPitchContPowerIEC |
| native | this:WindPitchContPowerIEC |




