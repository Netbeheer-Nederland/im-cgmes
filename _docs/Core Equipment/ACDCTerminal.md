# ACDCTerminal


_An electrical connection point (AC or DC) to a piece of conducting equipment. Terminals are connected at physical connection points called connectivity nodes._





**URI**: [cim:ACDCTerminal](http://iec.ch/TC57/CIM100#ACDCTerminal)<br />
**Type**: Class




```mermaid
 classDiagram
    class ACDCTerminal
    click ACDCTerminal href "../ACDCTerminal"
      IdentifiedObject <|-- ACDCTerminal
        click IdentifiedObject href "../IdentifiedObject"
      

      ACDCTerminal <|-- DCBaseTerminal
        click DCBaseTerminal href "../DCBaseTerminal"
      ACDCTerminal <|-- Terminal
        click Terminal href "../Terminal"
      
      
      ACDCTerminal : ACDCTerminal.BusNameMarker
        
          ACDCTerminal --> BusNameMarker : ACDCTerminal.BusNameMarker
          click BusNameMarker href "../BusNameMarker"
        
      ACDCTerminal : IdentifiedObject.description
        
      ACDCTerminal : IdentifiedObject.energyIdentCodeEic
        
      ACDCTerminal : IdentifiedObject.mRID
        
      ACDCTerminal : IdentifiedObject.name
        
      ACDCTerminal : ACDCTerminal.OperationalLimitSet
        
          ACDCTerminal --> OperationalLimitSet : ACDCTerminal.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      ACDCTerminal : ACDCTerminal.sequenceNumber
        
      ACDCTerminal : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * **ACDCTerminal**
        * [DCBaseTerminal](DCBaseTerminal.md)
        * [Terminal](Terminal.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| sequenceNumber | [cim:ACDCTerminal.sequenceNumber](http://iec.ch/TC57/CIM100#ACDCTerminal.sequenceNumber) | 1 <br />  integer  | The orientation of the terminal connections for a multiple terminal conductin... | direct |
| OperationalLimitSet | [cim:ACDCTerminal.OperationalLimitSet](http://iec.ch/TC57/CIM100#ACDCTerminal.OperationalLimitSet) | * <br />  [OperationalLimitSet](OperationalLimitSet.md)  | The operational limit sets at the terminal | direct |
| BusNameMarker | [cim:ACDCTerminal.BusNameMarker](http://iec.ch/TC57/CIM100#ACDCTerminal.BusNameMarker) | 0..1 <br />  [BusNameMarker](BusNameMarker.md)  | The bus name marker used to name the bus (topological node) | direct |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [BusNameMarker](BusNameMarker.md) | Terminal | range | [ACDCTerminal](ACDCTerminal.md) |
| [OperationalLimitSet](OperationalLimitSet.md) | Terminal | range | [ACDCTerminal](ACDCTerminal.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ACDCTerminal |
| native | this:ACDCTerminal |




