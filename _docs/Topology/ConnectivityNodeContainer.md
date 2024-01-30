# ConnectivityNodeContainer


_A base class for all objects that may contain connectivity nodes or topological nodes._





**URI**: [cim:ConnectivityNodeContainer](http://iec.ch/TC57/CIM100#ConnectivityNodeContainer)<br />
**Type**: Class




```mermaid
 classDiagram
    class ConnectivityNodeContainer
      ConnectivityNodeContainer : ConnectivityNodeContainer.TopologicalNode
        
          ConnectivityNodeContainer --> TopologicalNode : ConnectivityNodeContainer.TopologicalNode
        
      
```




<!-- no inheritance hierarchy -->


## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| TopologicalNode | [cim:ConnectivityNodeContainer.TopologicalNode](http://iec.ch/TC57/CIM100#ConnectivityNodeContainer.TopologicalNode) | 0..* <br />  [TopologicalNode](TopologicalNode.md)  | The topological nodes which belong to this connectivity node container | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [TopologicalNode](TopologicalNode.md) | ConnectivityNodeContainer | range | [ConnectivityNodeContainer](ConnectivityNodeContainer.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Topology-EU#Package_TopologyProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ConnectivityNodeContainer |
| native | this:ConnectivityNodeContainer |




