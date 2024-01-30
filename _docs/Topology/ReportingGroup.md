# ReportingGroup


_A reporting group is used for various ad-hoc groupings used for reporting._





**URI**: [cim:ReportingGroup](http://iec.ch/TC57/CIM100#ReportingGroup)<br />
**Type**: Class




```mermaid
 classDiagram
    class ReportingGroup
      IdentifiedObject <|-- ReportingGroup
      
      ReportingGroup : IdentifiedObject.description
        
      ReportingGroup : IdentifiedObject.energyIdentCodeEic
        
      ReportingGroup : IdentifiedObject.mRID
        
      ReportingGroup : IdentifiedObject.name
        
      ReportingGroup : IdentifiedObject.shortName
        
      ReportingGroup : ReportingGroup.TopologicalNode
        
          ReportingGroup --> TopologicalNode : ReportingGroup.TopologicalNode
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **ReportingGroup**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| TopologicalNode | [cim:ReportingGroup.TopologicalNode](http://iec.ch/TC57/CIM100#ReportingGroup.TopologicalNode) | 0..* <br />  [TopologicalNode](TopologicalNode.md)  | The topological nodes that belong to the reporting group | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [TopologicalNode](TopologicalNode.md) | ReportingGroup | range | [ReportingGroup](ReportingGroup.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Topology-EU#Package_TopologyProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ReportingGroup |
| native | this:ReportingGroup |




