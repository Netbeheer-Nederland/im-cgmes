# DCBaseTerminal


_An electrical connection point at a piece of DC conducting equipment. DC terminals are connected at one physical DC node that may have multiple DC terminals connected. A DC node is similar to an AC connectivity node. The model requires that DC connections are distinct from AC connections._





**URI**: [cim:DCBaseTerminal](http://iec.ch/TC57/CIM100#DCBaseTerminal)<br />
**Type**: Class




```mermaid
 classDiagram
    class DCBaseTerminal
    click DCBaseTerminal href "../DCBaseTerminal"
      ACDCTerminal <|-- DCBaseTerminal
        click ACDCTerminal href "../ACDCTerminal"
      

      DCBaseTerminal <|-- ACDCConverterDCTerminal
        click ACDCConverterDCTerminal href "../ACDCConverterDCTerminal"
      DCBaseTerminal <|-- DCTerminal
        click DCTerminal href "../DCTerminal"
      
      
      DCBaseTerminal : ACDCTerminal.connected
        
      DCBaseTerminal : IdentifiedObject.mRID
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [ACDCTerminal](ACDCTerminal.md)
        * **DCBaseTerminal**
            * [ACDCConverterDCTerminal](ACDCConverterDCTerminal.md)
            * [DCTerminal](DCTerminal.md)



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
| self | cim:DCBaseTerminal |
| native | this:DCBaseTerminal |




