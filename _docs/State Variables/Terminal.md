# Terminal


_An AC electrical connection point to a piece of conducting equipment. Terminals are connected at physical connection points called connectivity nodes._





**URI**: [cim:Terminal](http://iec.ch/TC57/CIM100#Terminal)<br />
**Type**: Class




```mermaid
 classDiagram
    class Terminal
    click Terminal href "../Terminal"
      ACDCTerminal <|-- Terminal
        click ACDCTerminal href "../ACDCTerminal"
      
      Terminal : IdentifiedObject.mRID
        
      Terminal : IdentifiedObject.name
        
      Terminal : Terminal.SvPowerFlow
        
          Terminal --> SvPowerFlow : Terminal.SvPowerFlow
          click SvPowerFlow href "../SvPowerFlow"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [ACDCTerminal](ACDCTerminal.md)
        * **Terminal**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| SvPowerFlow | [cim:Terminal.SvPowerFlow](http://iec.ch/TC57/CIM100#Terminal.SvPowerFlow) | 0..1 <br />  [SvPowerFlow](SvPowerFlow.md)  | The power flow state variable associated with the terminal | direct |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [SvPowerFlow](SvPowerFlow.md) | Terminal | range | [Terminal](Terminal.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/StateVariables-EU#Package_StateVariablesProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:Terminal |
| native | this:Terminal |




