# WindContRotorRIEC


_Rotor resistance control model._

_Reference: IEC 61400-27-1:2015, 5.6.5.3._





**URI**: [cim:WindContRotorRIEC](http://iec.ch/TC57/CIM100#WindContRotorRIEC)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindContRotorRIEC
      IdentifiedObject <|-- WindContRotorRIEC
      
      WindContRotorRIEC : IdentifiedObject.description
        
      WindContRotorRIEC : WindContRotorRIEC.kirr
        
          WindContRotorRIEC --> PU : WindContRotorRIEC.kirr
        
      WindContRotorRIEC : WindContRotorRIEC.komegafilt
        
      WindContRotorRIEC : WindContRotorRIEC.kpfilt
        
      WindContRotorRIEC : WindContRotorRIEC.kprr
        
          WindContRotorRIEC --> PU : WindContRotorRIEC.kprr
        
      WindContRotorRIEC : IdentifiedObject.mRID
        
      WindContRotorRIEC : IdentifiedObject.name
        
      WindContRotorRIEC : WindContRotorRIEC.rmax
        
          WindContRotorRIEC --> PU : WindContRotorRIEC.rmax
        
      WindContRotorRIEC : WindContRotorRIEC.rmin
        
          WindContRotorRIEC --> PU : WindContRotorRIEC.rmin
        
      WindContRotorRIEC : WindContRotorRIEC.tomegafiltrr
        
          WindContRotorRIEC --> Seconds : WindContRotorRIEC.tomegafiltrr
        
      WindContRotorRIEC : WindContRotorRIEC.tpfiltrr
        
          WindContRotorRIEC --> Seconds : WindContRotorRIEC.tpfiltrr
        
      WindContRotorRIEC : WindContRotorRIEC.WindDynamicsLookupTable
        
          WindContRotorRIEC --> WindDynamicsLookupTable : WindContRotorRIEC.WindDynamicsLookupTable
        
      WindContRotorRIEC : WindContRotorRIEC.WindGenTurbineType2IEC
        
          WindContRotorRIEC --> WindGenTurbineType2IEC : WindContRotorRIEC.WindGenTurbineType2IEC
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **WindContRotorRIEC**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| kirr | [cim:WindContRotorRIEC.kirr](http://iec.ch/TC57/CIM100#WindContRotorRIEC.kirr) | 1..1 <br />  [PU](PU.md)  | Integral gain in rotor resistance PI controller (<i>K</i><i><sub>Irr</sub></i... | direct |
| komegafilt | [cim:WindContRotorRIEC.komegafilt](http://iec.ch/TC57/CIM100#WindContRotorRIEC.komegafilt) | 1..1 <br />  float  | Filter gain for generator speed measurement (<i>K</i><i><sub>omegafilt</sub><... | direct |
| kpfilt | [cim:WindContRotorRIEC.kpfilt](http://iec.ch/TC57/CIM100#WindContRotorRIEC.kpfilt) | 1..1 <br />  float  | Filter gain for power measurement (<i>K</i><i><sub>pfilt</sub></i>) | direct |
| kprr | [cim:WindContRotorRIEC.kprr](http://iec.ch/TC57/CIM100#WindContRotorRIEC.kprr) | 1..1 <br />  [PU](PU.md)  | Proportional gain in rotor resistance PI controller (<i>K</i><i><sub>Prr</sub... | direct |
| rmax | [cim:WindContRotorRIEC.rmax](http://iec.ch/TC57/CIM100#WindContRotorRIEC.rmax) | 1..1 <br />  [PU](PU.md)  | Maximum rotor resistance (<i>r</i><i><sub>max</sub></i>) (&gt; WindContRotorR... | direct |
| rmin | [cim:WindContRotorRIEC.rmin](http://iec.ch/TC57/CIM100#WindContRotorRIEC.rmin) | 1..1 <br />  [PU](PU.md)  | Minimum rotor resistance (<i>r</i><i><sub>min</sub></i>) (&lt; WindContRotorR... | direct |
| tomegafiltrr | [cim:WindContRotorRIEC.tomegafiltrr](http://iec.ch/TC57/CIM100#WindContRotorRIEC.tomegafiltrr) | 1..1 <br />  [Seconds](Seconds.md)  | Filter time constant for generator speed measurement (<i>T</i><i><sub>omegafi... | direct |
| tpfiltrr | [cim:WindContRotorRIEC.tpfiltrr](http://iec.ch/TC57/CIM100#WindContRotorRIEC.tpfiltrr) | 1..1 <br />  [Seconds](Seconds.md)  | Filter time constant for power measurement (<i>T</i><i><sub>pfiltrr</sub></i>... | direct |
| WindDynamicsLookupTable | [cim:WindContRotorRIEC.WindDynamicsLookupTable](http://iec.ch/TC57/CIM100#WindContRotorRIEC.WindDynamicsLookupTable) | 1..* <br />  [WindDynamicsLookupTable](WindDynamicsLookupTable.md)  | The wind dynamics lookup table associated with this rotor resistance control ... | direct |
| WindGenTurbineType2IEC | [cim:WindContRotorRIEC.WindGenTurbineType2IEC](http://iec.ch/TC57/CIM100#WindContRotorRIEC.WindGenTurbineType2IEC) | 1..1 <br />  [WindGenTurbineType2IEC](WindGenTurbineType2IEC.md)  | Wind turbine type 2 model with whitch this wind control rotor resistance mode... | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [WindDynamicsLookupTable](WindDynamicsLookupTable.md) | WindContRotorRIEC | range | [WindContRotorRIEC](WindContRotorRIEC.md) |
| [WindGenTurbineType2IEC](WindGenTurbineType2IEC.md) | WindContRotorRIEC | range | [WindContRotorRIEC](WindContRotorRIEC.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindContRotorRIEC |
| native | this:WindContRotorRIEC |




