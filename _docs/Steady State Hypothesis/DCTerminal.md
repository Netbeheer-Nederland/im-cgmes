# DCTerminal


_An electrical connection point to generic DC conducting equipment._





**URI**: [cim:DCTerminal](http://iec.ch/TC57/CIM100#DCTerminal)<br />
**Type**: Class




```mermaid
 classDiagram
    class DCTerminal
    click DCTerminal href "../DCTerminal"
      DCBaseTerminal <|-- DCTerminal
        click DCBaseTerminal href "../DCBaseTerminal"
      
      DCTerminal : ACDCTerminal.connected
        
      DCTerminal : IdentifiedObject.mRID
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [ACDCTerminal](ACDCTerminal.md)
        * [DCBaseTerminal](DCBaseTerminal.md)
            * **DCTerminal**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| connected | [cim:ACDCTerminal.connected](http://iec.ch/TC57/CIM100#ACDCTerminal.connected) | 1 <br />  boolean  | The connected status is related to a bus-branch model and the topological nod... | [ACDCTerminal](ACDCTerminal.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/SteadyStateHypothesis-EU#Package_SteadyStateHypothesisProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:DCTerminal |
| native | this:DCTerminal |




