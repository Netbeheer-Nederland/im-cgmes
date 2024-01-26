# ControlArea


_A control area is a grouping of generating units and/or loads and a cutset of tie lines (as terminals) which may be used for a variety of purposes including automatic generation control, power flow solution area interchange control specification, and input to load forecasting. All generation and load within the area defined by the terminals on the border are considered in the area interchange control. Note that any number of overlapping control area specifications can be superimposed on the physical model. The following general principles apply to ControlArea:_

_1.  The control area orientation for net interchange is positive for an import, negative for an export._

_2.  The control area net interchange is determined by summing flows in Terminals. The Terminals are identified by creating a set of TieFlow objects associated with a ControlArea object. Each TieFlow object identifies one Terminal._

_3.  In a single network model, a tie between two control areas must be modelled in both control area specifications, such that the two representations of the tie flow sum to zero._

_4.  The normal orientation of Terminal flow is positive for flow into the conducting equipment that owns the Terminal. (i.e. flow from a bus into a device is positive.) However, the orientation of each flow in the control area specification must align with the control area convention, i.e. import is positive. If the orientation of the Terminal flow referenced by a TieFlow is positive into the control area, then this is confirmed by setting TieFlow.positiveFlowIn flag TRUE. If not, the orientation must be reversed by setting the TieFlow.positiveFlowIn flag FALSE._





**URI**: [cim:ControlArea](http://iec.ch/TC57/CIM100#ControlArea)<br />
**Type**: Class




```mermaid
 classDiagram
    class ControlArea
      PowerSystemResource <|-- ControlArea
      
      ControlArea : ControlArea.ControlAreaGeneratingUnit
        
          ControlArea --> ControlAreaGeneratingUnit : ControlArea.ControlAreaGeneratingUnit
        
      ControlArea : IdentifiedObject.description
        
      ControlArea : ControlArea.EnergyArea
        
          ControlArea --> EnergyArea : ControlArea.EnergyArea
        
      ControlArea : IdentifiedObject.energyIdentCodeEic
        
      ControlArea : IdentifiedObject.mRID
        
      ControlArea : IdentifiedObject.name
        
      ControlArea : IdentifiedObject.shortName
        
      ControlArea : ControlArea.TieFlow
        
          ControlArea --> TieFlow : ControlArea.TieFlow
        
      ControlArea : ControlArea.type
        
          ControlArea --> ControlAreaTypeKind : ControlArea.type
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * **ControlArea**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| type | [cim:ControlArea.type](http://iec.ch/TC57/CIM100#ControlArea.type) | 1..1 <br />  [ControlAreaTypeKind](ControlAreaTypeKind.md)  | The primary type of control area definition used to determine if this is used... | direct |
| TieFlow | [cim:ControlArea.TieFlow](http://iec.ch/TC57/CIM100#ControlArea.TieFlow) | 0..* <br />  [TieFlow](TieFlow.md)  | The tie flows associated with the control area | direct |
| ControlAreaGeneratingUnit | [cim:ControlArea.ControlAreaGeneratingUnit](http://iec.ch/TC57/CIM100#ControlArea.ControlAreaGeneratingUnit) | 0..* <br />  [ControlAreaGeneratingUnit](ControlAreaGeneratingUnit.md)  | The generating unit specifications for the control area | direct |
| EnergyArea | [cim:ControlArea.EnergyArea](http://iec.ch/TC57/CIM100#ControlArea.EnergyArea) | 1..1 <br />  [EnergyArea](EnergyArea.md)  | The energy area that is forecast from this control area specification | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ControlAreaGeneratingUnit](ControlAreaGeneratingUnit.md) | ControlArea | range | [ControlArea](ControlArea.md) |
| [EnergyArea](EnergyArea.md) | ControlArea | range | [ControlArea](ControlArea.md) |
| [LoadArea](LoadArea.md) | ControlArea | range | [ControlArea](ControlArea.md) |
| [SubLoadArea](SubLoadArea.md) | ControlArea | range | [ControlArea](ControlArea.md) |
| [TieFlow](TieFlow.md) | ControlArea | range | [ControlArea](ControlArea.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ControlArea |
| native | this:ControlArea |




