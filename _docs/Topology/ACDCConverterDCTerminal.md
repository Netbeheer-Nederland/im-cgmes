# ACDCConverterDCTerminal


_A DC electrical connection point at the AC/DC converter. The AC/DC converter is electrically connected also to the AC side. The AC connection is inherited from the AC conducting equipment in the same way as any other AC equipment. The AC/DC converter DC terminal is separate from generic DC terminal to restrict the connection with the AC side to AC/DC converter and so that no other DC conducting equipment can be connected to the AC side._





**URI**: [cim:ACDCConverterDCTerminal](http://iec.ch/TC57/CIM100#ACDCConverterDCTerminal)<br />
**Type**: Class




```mermaid
 classDiagram
    class ACDCConverterDCTerminal
    click ACDCConverterDCTerminal href "../ACDCConverterDCTerminal"
      DCBaseTerminal <|-- ACDCConverterDCTerminal
        click DCBaseTerminal href "../DCBaseTerminal"
      
      ACDCConverterDCTerminal : DCBaseTerminal.DCTopologicalNode
        
          ACDCConverterDCTerminal --> DCTopologicalNode : DCBaseTerminal.DCTopologicalNode
          click DCTopologicalNode href "../DCTopologicalNode"
        
      ACDCConverterDCTerminal : IdentifiedObject.description
        
      ACDCConverterDCTerminal : IdentifiedObject.energyIdentCodeEic
        
      ACDCConverterDCTerminal : IdentifiedObject.mRID
        
      ACDCConverterDCTerminal : IdentifiedObject.name
        
      ACDCConverterDCTerminal : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [ACDCTerminal](ACDCTerminal.md)
        * [DCBaseTerminal](DCBaseTerminal.md)
            * **ACDCConverterDCTerminal**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| DCTopologicalNode | [cim:DCBaseTerminal.DCTopologicalNode](http://iec.ch/TC57/CIM100#DCBaseTerminal.DCTopologicalNode) | 1 <br />  [DCTopologicalNode](DCTopologicalNode.md)  | See association end Terminal | [DCBaseTerminal](DCBaseTerminal.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 0..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/Topology-EU#Package_TopologyProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ACDCConverterDCTerminal |
| native | this:ACDCConverterDCTerminal |




