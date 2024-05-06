# DCTerminal


_An electrical connection point to generic DC conducting equipment._





**URI**: [cim:DCTerminal](http://iec.ch/TC57/CIM100#DCTerminal)<br />
**Type**: Class




```mermaid
 classDiagram
    class DCTerminal
    click DCTerminal href "../DCTerminal"
      DCBaseTerminal <|-- DCTerminal
        click DCBaseTerminal href "../DCBaseTerminal"
      
      DCTerminal : ACDCTerminal.BusNameMarker
        
          DCTerminal --> BusNameMarker : ACDCTerminal.BusNameMarker
          click BusNameMarker href "../BusNameMarker"
        
      DCTerminal : DCTerminal.DCConductingEquipment
        
          DCTerminal --> DCConductingEquipment : DCTerminal.DCConductingEquipment
          click DCConductingEquipment href "../DCConductingEquipment"
        
      DCTerminal : DCBaseTerminal.DCNode
        
          DCTerminal --> DCNode : DCBaseTerminal.DCNode
          click DCNode href "../DCNode"
        
      DCTerminal : IdentifiedObject.description
        
      DCTerminal : IdentifiedObject.energyIdentCodeEic
        
      DCTerminal : IdentifiedObject.mRID
        
      DCTerminal : IdentifiedObject.name
        
      DCTerminal : ACDCTerminal.OperationalLimitSet
        
          DCTerminal --> OperationalLimitSet : ACDCTerminal.OperationalLimitSet
          click OperationalLimitSet href "../OperationalLimitSet"
        
      DCTerminal : ACDCTerminal.sequenceNumber
        
      DCTerminal : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [ACDCTerminal](ACDCTerminal.md)
        * [DCBaseTerminal](DCBaseTerminal.md)
            * **DCTerminal**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| DCConductingEquipment | [cim:DCTerminal.DCConductingEquipment](http://iec.ch/TC57/CIM100#DCTerminal.DCConductingEquipment) | 1 <br />  [DCConductingEquipment](DCConductingEquipment.md)  | An DC  terminal belong to a DC conducting equipment | direct |
| DCNode | [cim:DCBaseTerminal.DCNode](http://iec.ch/TC57/CIM100#DCBaseTerminal.DCNode) | 0..1 <br />  [DCNode](DCNode.md)  | The DC connectivity node to which this DC base terminal connects with zero im... | [DCBaseTerminal](DCBaseTerminal.md) |
| sequenceNumber | [cim:ACDCTerminal.sequenceNumber](http://iec.ch/TC57/CIM100#ACDCTerminal.sequenceNumber) | 1 <br />  integer  | The orientation of the terminal connections for a multiple terminal conductin... | [ACDCTerminal](ACDCTerminal.md) |
| OperationalLimitSet | [cim:ACDCTerminal.OperationalLimitSet](http://iec.ch/TC57/CIM100#ACDCTerminal.OperationalLimitSet) | * <br />  [OperationalLimitSet](OperationalLimitSet.md)  | The operational limit sets at the terminal | [ACDCTerminal](ACDCTerminal.md) |
| BusNameMarker | [cim:ACDCTerminal.BusNameMarker](http://iec.ch/TC57/CIM100#ACDCTerminal.BusNameMarker) | 0..1 <br />  [BusNameMarker](BusNameMarker.md)  | The bus name marker used to name the bus (topological node) | [ACDCTerminal](ACDCTerminal.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [DCBreaker](DCBreaker.md) | DCTerminals | range | [DCTerminal](DCTerminal.md) |
| [DCBusbar](DCBusbar.md) | DCTerminals | range | [DCTerminal](DCTerminal.md) |
| [DCChopper](DCChopper.md) | DCTerminals | range | [DCTerminal](DCTerminal.md) |
| [DCConductingEquipment](DCConductingEquipment.md) | DCTerminals | range | [DCTerminal](DCTerminal.md) |
| [DCDisconnector](DCDisconnector.md) | DCTerminals | range | [DCTerminal](DCTerminal.md) |
| [DCGround](DCGround.md) | DCTerminals | range | [DCTerminal](DCTerminal.md) |
| [DCLineSegment](DCLineSegment.md) | DCTerminals | range | [DCTerminal](DCTerminal.md) |
| [DCSeriesDevice](DCSeriesDevice.md) | DCTerminals | range | [DCTerminal](DCTerminal.md) |
| [DCShunt](DCShunt.md) | DCTerminals | range | [DCTerminal](DCTerminal.md) |
| [DCSwitch](DCSwitch.md) | DCTerminals | range | [DCTerminal](DCTerminal.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:DCTerminal |
| native | this:DCTerminal |




