# IdentifiedObject


_This is a root class to provide common identification for all classes needing identification and naming attributes._





**URI**: [cim:IdentifiedObject](http://iec.ch/TC57/CIM100#IdentifiedObject)<br />
**Type**: Class




```mermaid
 classDiagram
    class IdentifiedObject
    click IdentifiedObject href "../IdentifiedObject"
      IdentifiedObject <|-- Diagram
        click Diagram href "../Diagram"
      IdentifiedObject <|-- DiagramObject
        click DiagramObject href "../DiagramObject"
      IdentifiedObject <|-- DiagramObjectStyle
        click DiagramObjectStyle href "../DiagramObjectStyle"
      IdentifiedObject <|-- DiagramStyle
        click DiagramStyle href "../DiagramStyle"
      IdentifiedObject <|-- VisibilityLayer
        click VisibilityLayer href "../VisibilityLayer"
      
      IdentifiedObject : IdentifiedObject.description
        
      IdentifiedObject : IdentifiedObject.DiagramObjects
        
          IdentifiedObject --> DiagramObject : IdentifiedObject.DiagramObjects
          click DiagramObject href "../DiagramObject"
        
      IdentifiedObject : IdentifiedObject.mRID
        
      IdentifiedObject : IdentifiedObject.name
        
      
```





## Inheritance
* **IdentifiedObject**
    * [Diagram](Diagram.md)
    * [DiagramObject](DiagramObject.md)
    * [DiagramObjectStyle](DiagramObjectStyle.md)
    * [DiagramStyle](DiagramStyle.md)
    * [VisibilityLayer](VisibilityLayer.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| DiagramObjects | [cim:IdentifiedObject.DiagramObjects](http://iec.ch/TC57/CIM100#IdentifiedObject.DiagramObjects) | * <br />  [DiagramObject](DiagramObject.md)  | The diagram objects that are associated with the domain object | direct |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | direct |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | direct |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [DiagramObject](DiagramObject.md) | IdentifiedObject | range | [IdentifiedObject](IdentifiedObject.md) |
| [TextDiagramObject](TextDiagramObject.md) | IdentifiedObject | range | [IdentifiedObject](IdentifiedObject.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/DiagramLayout-EU#Package_DiagramLayoutProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:IdentifiedObject |
| native | this:IdentifiedObject |




