# Terminal


_An AC electrical connection point to a piece of conducting equipment. Terminals are connected at physical connection points called connectivity nodes._





**URI**: [cim:Terminal](http://iec.ch/TC57/CIM100#Terminal)<br />
**Type**: Class




```mermaid
 classDiagram
    class Terminal
      ACDCTerminal <|-- Terminal
      
      Terminal : Terminal.ConductingEquipment
        
          Terminal --> ConductingEquipment : Terminal.ConductingEquipment
        
      Terminal : Terminal.ConnectivityNode
        
          Terminal --> ConnectivityNode : Terminal.ConnectivityNode
        
      Terminal : IdentifiedObject.description
        
      Terminal : IdentifiedObject.energyIdentCodeEic
        
      Terminal : IdentifiedObject.mRID
        
      Terminal : IdentifiedObject.name
        
      Terminal : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [ACDCTerminal](ACDCTerminal.md)
        * **Terminal**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| ConductingEquipment | [cim:Terminal.ConductingEquipment](http://iec.ch/TC57/CIM100#Terminal.ConductingEquipment) | 1..1 <br />  [ConductingEquipment](ConductingEquipment.md)  | The conducting equipment of the terminal | direct |
| ConnectivityNode | [cim:Terminal.ConnectivityNode](http://iec.ch/TC57/CIM100#Terminal.ConnectivityNode) | 0..1 <br />  [ConnectivityNode](ConnectivityNode.md)  | The connectivity node to which this terminal connects with zero impedance | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ConductingEquipment](ConductingEquipment.md) | Terminals | range | [Terminal](Terminal.md) |
| [ConnectivityNode](ConnectivityNode.md) | Terminals | range | [Terminal](Terminal.md) |
| [Connector](Connector.md) | Terminals | range | [Terminal](Terminal.md) |
| [Junction](Junction.md) | Terminals | range | [Terminal](Terminal.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/EquipmentBoundary-EU#Package_EquipmentBoundaryProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Terminal |
| native | this:Terminal |




