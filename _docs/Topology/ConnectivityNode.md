# ConnectivityNode


_Connectivity nodes are points where terminals of AC conducting equipment are connected together with zero impedance._





**URI**: [cim:ConnectivityNode](http://iec.ch/TC57/CIM100#ConnectivityNode)<br />
**Type**: Class




```mermaid
 classDiagram
    class ConnectivityNode
      ConnectivityNode : ConnectivityNode.TopologicalNode
        
          ConnectivityNode --> TopologicalNode : ConnectivityNode.TopologicalNode
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| TopologicalNode | [cim:ConnectivityNode.TopologicalNode](http://iec.ch/TC57/CIM100#ConnectivityNode.TopologicalNode) | 1..1 <br />  [TopologicalNode](TopologicalNode.md)  | The topological node to which this connectivity node is assigned | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [TopologicalNode](TopologicalNode.md) | ConnectivityNodes | range | [ConnectivityNode](ConnectivityNode.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Topology-EU#Package_TopologyProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ConnectivityNode |
| native | this:ConnectivityNode |




