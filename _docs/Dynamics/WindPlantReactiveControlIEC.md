# WindPlantReactiveControlIEC


_Simplified plant voltage and reactive power control model for use with type 3 and type 4 wind turbine models._

_Reference: IEC 61400-27-1:2015, Annex D._





**URI**: [cim:WindPlantReactiveControlIEC](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC)<br />
**Type**: Class




```mermaid
 classDiagram
    class WindPlantReactiveControlIEC
    click WindPlantReactiveControlIEC href "../WindPlantReactiveControlIEC"
      IdentifiedObject <|-- WindPlantReactiveControlIEC
        click IdentifiedObject href "../IdentifiedObject"
      
      WindPlantReactiveControlIEC : IdentifiedObject.description
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.dxrefmax
        
          WindPlantReactiveControlIEC --> PU : WindPlantReactiveControlIEC.dxrefmax
          click PU href "../PU"
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.dxrefmin
        
          WindPlantReactiveControlIEC --> PU : WindPlantReactiveControlIEC.dxrefmin
          click PU href "../PU"
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.kiwpx
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.kiwpxmax
        
          WindPlantReactiveControlIEC --> PU : WindPlantReactiveControlIEC.kiwpxmax
          click PU href "../PU"
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.kiwpxmin
        
          WindPlantReactiveControlIEC --> PU : WindPlantReactiveControlIEC.kiwpxmin
          click PU href "../PU"
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.kpwpx
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.kwpqref
        
          WindPlantReactiveControlIEC --> PU : WindPlantReactiveControlIEC.kwpqref
          click PU href "../PU"
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.kwpqu
        
          WindPlantReactiveControlIEC --> PU : WindPlantReactiveControlIEC.kwpqu
          click PU href "../PU"
        
      WindPlantReactiveControlIEC : IdentifiedObject.mRID
        
      WindPlantReactiveControlIEC : IdentifiedObject.name
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.tuqfilt
        
          WindPlantReactiveControlIEC --> Seconds : WindPlantReactiveControlIEC.tuqfilt
          click Seconds href "../Seconds"
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.twppfiltq
        
          WindPlantReactiveControlIEC --> Seconds : WindPlantReactiveControlIEC.twppfiltq
          click Seconds href "../Seconds"
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.twpqfiltq
        
          WindPlantReactiveControlIEC --> Seconds : WindPlantReactiveControlIEC.twpqfiltq
          click Seconds href "../Seconds"
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.twpufiltq
        
          WindPlantReactiveControlIEC --> Seconds : WindPlantReactiveControlIEC.twpufiltq
          click Seconds href "../Seconds"
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.txft
        
          WindPlantReactiveControlIEC --> Seconds : WindPlantReactiveControlIEC.txft
          click Seconds href "../Seconds"
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.txfv
        
          WindPlantReactiveControlIEC --> Seconds : WindPlantReactiveControlIEC.txfv
          click Seconds href "../Seconds"
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.uwpqdip
        
          WindPlantReactiveControlIEC --> PU : WindPlantReactiveControlIEC.uwpqdip
          click PU href "../PU"
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.WindDynamicsLookupTable
        
          WindPlantReactiveControlIEC --> WindDynamicsLookupTable : WindPlantReactiveControlIEC.WindDynamicsLookupTable
          click WindDynamicsLookupTable href "../WindDynamicsLookupTable"
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.WindPlantIEC
        
          WindPlantReactiveControlIEC --> WindPlantIEC : WindPlantReactiveControlIEC.WindPlantIEC
          click WindPlantIEC href "../WindPlantIEC"
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.windPlantQcontrolModesType
        
          WindPlantReactiveControlIEC --> WindPlantQcontrolModeKind : WindPlantReactiveControlIEC.windPlantQcontrolModesType
          click WindPlantQcontrolModeKind href "../WindPlantQcontrolModeKind"
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.xrefmax
        
          WindPlantReactiveControlIEC --> PU : WindPlantReactiveControlIEC.xrefmax
          click PU href "../PU"
        
      WindPlantReactiveControlIEC : WindPlantReactiveControlIEC.xrefmin
        
          WindPlantReactiveControlIEC --> PU : WindPlantReactiveControlIEC.xrefmin
          click PU href "../PU"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **WindPlantReactiveControlIEC**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| WindDynamicsLookupTable | [cim:WindPlantReactiveControlIEC.WindDynamicsLookupTable](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.WindDynamicsLookupTable) | 1..* <br />  [WindDynamicsLookupTable](WindDynamicsLookupTable.md)  | The wind dynamics lookup table associated with this voltage and reactive powe... | direct |
| WindPlantIEC | [cim:WindPlantReactiveControlIEC.WindPlantIEC](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.WindPlantIEC) | 1 <br />  [WindPlantIEC](WindPlantIEC.md)  | Wind plant reactive control model associated with this wind plant | direct |
| dxrefmax | [cim:WindPlantReactiveControlIEC.dxrefmax](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.dxrefmax) | 1 <br />  [PU](PU.md)  | Maximum positive ramp rate for wind turbine reactive power/voltage reference ... | direct |
| dxrefmin | [cim:WindPlantReactiveControlIEC.dxrefmin](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.dxrefmin) | 1 <br />  [PU](PU.md)  | Maximum negative ramp rate for wind turbine reactive power/voltage reference ... | direct |
| kiwpx | [cim:WindPlantReactiveControlIEC.kiwpx](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.kiwpx) | 1 <br />  float  | Plant Q controller integral gain (<i>K</i><i><sub>IWPx</sub></i>) | direct |
| kiwpxmax | [cim:WindPlantReactiveControlIEC.kiwpxmax](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.kiwpxmax) | 1 <br />  [PU](PU.md)  | Maximum reactive power/voltage reference from integration (<i>K</i><i><sub>IW... | direct |
| kiwpxmin | [cim:WindPlantReactiveControlIEC.kiwpxmin](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.kiwpxmin) | 1 <br />  [PU](PU.md)  | Minimum reactive power/voltage reference from integration (<i>K</i><i><sub>IW... | direct |
| kpwpx | [cim:WindPlantReactiveControlIEC.kpwpx](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.kpwpx) | 1 <br />  float  | Plant Q controller proportional gain (<i>K</i><i><sub>PWPx</sub></i>) | direct |
| kwpqref | [cim:WindPlantReactiveControlIEC.kwpqref](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.kwpqref) | 1 <br />  [PU](PU.md)  | Reactive power reference gain (<i>K</i><i><sub>WPqref</sub></i>) | direct |
| kwpqu | [cim:WindPlantReactiveControlIEC.kwpqu](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.kwpqu) | 1 <br />  [PU](PU.md)  | Plant voltage control droop (<i>K</i><i><sub>WPqu</sub></i>) | direct |
| tuqfilt | [cim:WindPlantReactiveControlIEC.tuqfilt](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.tuqfilt) | 1 <br />  [Seconds](Seconds.md)  | Filter time constant for voltage-dependent reactive power (<i>T</i><i><sub>uq... | direct |
| twppfiltq | [cim:WindPlantReactiveControlIEC.twppfiltq](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.twppfiltq) | 1 <br />  [Seconds](Seconds.md)  | Filter time constant for active power measurement (<i>T</i><i><sub>WPpfiltq</... | direct |
| twpqfiltq | [cim:WindPlantReactiveControlIEC.twpqfiltq](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.twpqfiltq) | 1 <br />  [Seconds](Seconds.md)  | Filter time constant for reactive power measurement (<i>T</i><i><sub>WPqfiltq... | direct |
| twpufiltq | [cim:WindPlantReactiveControlIEC.twpufiltq](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.twpufiltq) | 1 <br />  [Seconds](Seconds.md)  | Filter time constant for voltage measurement (<i>T</i><i><sub>WPufiltq</sub><... | direct |
| txft | [cim:WindPlantReactiveControlIEC.txft](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.txft) | 1 <br />  [Seconds](Seconds.md)  | Lead time constant in reference value transfer function (<i>T</i><i><sub>xft<... | direct |
| txfv | [cim:WindPlantReactiveControlIEC.txfv](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.txfv) | 1 <br />  [Seconds](Seconds.md)  | Lag time constant in reference value transfer function (<i>T</i><i><sub>xfv</... | direct |
| uwpqdip | [cim:WindPlantReactiveControlIEC.uwpqdip](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.uwpqdip) | 1 <br />  [PU](PU.md)  | Voltage threshold for UVRT detection in Q control (<i>u</i><i><sub>WPqdip</su... | direct |
| windPlantQcontrolModesType | [cim:WindPlantReactiveControlIEC.windPlantQcontrolModesType](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.windPlantQcontrolModesType) | 1 <br />  [WindPlantQcontrolModeKind](WindPlantQcontrolModeKind.md)  | Reactive power/voltage controller mode (<i>M</i><i><sub>WPqmode</sub></i>) | direct |
| xrefmax | [cim:WindPlantReactiveControlIEC.xrefmax](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.xrefmax) | 1 <br />  [PU](PU.md)  | Maximum <i>x</i><sub>WTref</sub> (<i>q</i><i><sub>WTref</sub></i> or delta<i>... | direct |
| xrefmin | [cim:WindPlantReactiveControlIEC.xrefmin](http://iec.ch/TC57/CIM100#WindPlantReactiveControlIEC.xrefmin) | 1 <br />  [PU](PU.md)  | Minimum <i>x</i><i><sub>WTref</sub></i> (<i>q</i><i><sub>WTref</sub></i> or d... | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [WindDynamicsLookupTable](WindDynamicsLookupTable.md) | WindPlantReactiveControlIEC | range | [WindPlantReactiveControlIEC](WindPlantReactiveControlIEC.md) |
| [WindPlantIEC](WindPlantIEC.md) | WindPlantReactiveControlIEC | range | [WindPlantReactiveControlIEC](WindPlantReactiveControlIEC.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Dynamics-EU#Package_DynamicsProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:WindPlantReactiveControlIEC |
| native | this:WindPlantReactiveControlIEC |




