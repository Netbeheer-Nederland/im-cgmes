# DCTopologicalNode


_DC bus._





**URI**: [cim:DCTopologicalNode](http://iec.ch/TC57/CIM100#DCTopologicalNode)<br />
**Type**: Class




```mermaid
 classDiagram
    class DCTopologicalNode
      IdentifiedObject <|-- DCTopologicalNode
      
      DCTopologicalNode : DCTopologicalNode.DCTopologicalIsland
        
          DCTopologicalNode --> DCTopologicalIsland : DCTopologicalNode.DCTopologicalIsland
        
      DCTopologicalNode : IdentifiedObject.mRID
        
      DCTopologicalNode : IdentifiedObject.name
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **DCTopologicalNode**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| DCTopologicalIsland | [cim:DCTopologicalNode.DCTopologicalIsland](http://iec.ch/TC57/CIM100#DCTopologicalNode.DCTopologicalIsland) | 0..1 <br />  [DCTopologicalIsland](DCTopologicalIsland.md)  | A DC topological node belongs to a DC topological island | direct |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [DCTopologicalIsland](DCTopologicalIsland.md) | DCTopologicalNodes | range | [DCTopologicalNode](DCTopologicalNode.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/StateVariables-EU#Package_StateVariablesProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:DCTopologicalNode |
| native | this:DCTopologicalNode |




