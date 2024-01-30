# DCTopologicalIsland


_An electrically connected subset of the network. DC topological islands can change as the current network state changes, e.g. due to: _

_- disconnect switches or breakers changing state in a SCADA/EMS._

_- manual creation, change or deletion of topological nodes in a planning tool._

_Only energised TopologicalNode-s shall be part of the topological island._





**URI**: [cim:DCTopologicalIsland](http://iec.ch/TC57/CIM100#DCTopologicalIsland)<br />
**Type**: Class




```mermaid
 classDiagram
    class DCTopologicalIsland
      IdentifiedObject <|-- DCTopologicalIsland
      
      DCTopologicalIsland : DCTopologicalIsland.DCTopologicalNodes
        
          DCTopologicalIsland --> DCTopologicalNode : DCTopologicalIsland.DCTopologicalNodes
        
      DCTopologicalIsland : IdentifiedObject.mRID
        
      DCTopologicalIsland : IdentifiedObject.name
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **DCTopologicalIsland**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| DCTopologicalNodes | [cim:DCTopologicalIsland.DCTopologicalNodes](http://iec.ch/TC57/CIM100#DCTopologicalIsland.DCTopologicalNodes) | 1..* <br />  [DCTopologicalNode](DCTopologicalNode.md)  | The DC topological nodes in a DC topological island | direct |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [DCTopologicalNode](DCTopologicalNode.md) | DCTopologicalIsland | range | [DCTopologicalIsland](DCTopologicalIsland.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/StateVariables-EU#Package_StateVariablesProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:DCTopologicalIsland |
| native | this:DCTopologicalIsland |




