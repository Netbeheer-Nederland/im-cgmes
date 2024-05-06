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
      
      
      DCBaseTerminal : DCBaseTerminal.DCTopologicalNode
        
          DCBaseTerminal --> DCTopologicalNode : DCBaseTerminal.DCTopologicalNode
          click DCTopologicalNode href "../DCTopologicalNode"
        
      DCBaseTerminal : IdentifiedObject.description
        
      DCBaseTerminal : IdentifiedObject.energyIdentCodeEic
        
      DCBaseTerminal : IdentifiedObject.mRID
        
      DCBaseTerminal : IdentifiedObject.name
        
      DCBaseTerminal : IdentifiedObject.shortName
        
      
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
| DCTopologicalNode | [cim:DCBaseTerminal.DCTopologicalNode](http://iec.ch/TC57/CIM100#DCBaseTerminal.DCTopologicalNode) | 1 <br />  [DCTopologicalNode](DCTopologicalNode.md)  | See association end Terminal | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [DCTopologicalNode](DCTopologicalNode.md) | DCTerminals | range | [DCBaseTerminal](DCBaseTerminal.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Topology-EU#Package_TopologyProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:DCBaseTerminal |
| native | this:DCBaseTerminal |




