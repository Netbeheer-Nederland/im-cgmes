# ACDCConverterDCTerminal


_A DC electrical connection point at the AC/DC converter. The AC/DC converter is electrically connected also to the AC side. The AC connection is inherited from the AC conducting equipment in the same way as any other AC equipment. The AC/DC converter DC terminal is separate from generic DC terminal to restrict the connection with the AC side to AC/DC converter and so that no other DC conducting equipment can be connected to the AC side._





**URI**: [cim:ACDCConverterDCTerminal](http://iec.ch/TC57/CIM100#ACDCConverterDCTerminal)<br />
**Type**: Class




```mermaid
 classDiagram
    class ACDCConverterDCTerminal
      DCBaseTerminal <|-- ACDCConverterDCTerminal
      
      ACDCConverterDCTerminal : ACDCTerminal.BusNameMarker
        
          ACDCConverterDCTerminal --> BusNameMarker : ACDCTerminal.BusNameMarker
        
      ACDCConverterDCTerminal : ACDCConverterDCTerminal.DCConductingEquipment
        
          ACDCConverterDCTerminal --> ACDCConverter : ACDCConverterDCTerminal.DCConductingEquipment
        
      ACDCConverterDCTerminal : DCBaseTerminal.DCNode
        
          ACDCConverterDCTerminal --> DCNode : DCBaseTerminal.DCNode
        
      ACDCConverterDCTerminal : IdentifiedObject.description
        
      ACDCConverterDCTerminal : IdentifiedObject.energyIdentCodeEic
        
      ACDCConverterDCTerminal : IdentifiedObject.mRID
        
      ACDCConverterDCTerminal : IdentifiedObject.name
        
      ACDCConverterDCTerminal : ACDCTerminal.OperationalLimitSet
        
          ACDCConverterDCTerminal --> OperationalLimitSet : ACDCTerminal.OperationalLimitSet
        
      ACDCConverterDCTerminal : ACDCConverterDCTerminal.polarity
        
          ACDCConverterDCTerminal --> DCPolarityKind : ACDCConverterDCTerminal.polarity
        
      ACDCConverterDCTerminal : ACDCTerminal.sequenceNumber
        
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
| DCConductingEquipment | [cim:ACDCConverterDCTerminal.DCConductingEquipment](http://iec.ch/TC57/CIM100#ACDCConverterDCTerminal.DCConductingEquipment) | 1..1 <br />  [ACDCConverter](ACDCConverter.md)  | A DC converter terminal belong to an DC converter | direct |
| polarity | [cim:ACDCConverterDCTerminal.polarity](http://iec.ch/TC57/CIM100#ACDCConverterDCTerminal.polarity) | 1..1 <br />  [DCPolarityKind](DCPolarityKind.md)  | Represents the normal network polarity condition | direct |
| DCNode | [cim:DCBaseTerminal.DCNode](http://iec.ch/TC57/CIM100#DCBaseTerminal.DCNode) | 0..1 <br />  [DCNode](DCNode.md)  | The DC connectivity node to which this DC base terminal connects with zero im... | [DCBaseTerminal](DCBaseTerminal.md) |
| sequenceNumber | [cim:ACDCTerminal.sequenceNumber](http://iec.ch/TC57/CIM100#ACDCTerminal.sequenceNumber) | 1..1 <br />  integer  | The orientation of the terminal connections for a multiple terminal conductin... | [ACDCTerminal](ACDCTerminal.md) |
| OperationalLimitSet | [cim:ACDCTerminal.OperationalLimitSet](http://iec.ch/TC57/CIM100#ACDCTerminal.OperationalLimitSet) | 0..* <br />  [OperationalLimitSet](OperationalLimitSet.md)  | The operational limit sets at the terminal | [ACDCTerminal](ACDCTerminal.md) |
| BusNameMarker | [cim:ACDCTerminal.BusNameMarker](http://iec.ch/TC57/CIM100#ACDCTerminal.BusNameMarker) | 0..1 <br />  [BusNameMarker](BusNameMarker.md)  | The bus name marker used to name the bus (topological node) | [ACDCTerminal](ACDCTerminal.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1..1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1..1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ACDCConverter](ACDCConverter.md) | DCTerminals | range | [ACDCConverterDCTerminal](ACDCConverterDCTerminal.md) |
| [CsConverter](CsConverter.md) | DCTerminals | range | [ACDCConverterDCTerminal](ACDCConverterDCTerminal.md) |
| [VsConverter](VsConverter.md) | DCTerminals | range | [ACDCConverterDCTerminal](ACDCConverterDCTerminal.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:ACDCConverterDCTerminal |
| native | this:ACDCConverterDCTerminal |




