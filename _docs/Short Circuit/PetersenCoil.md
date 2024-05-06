# PetersenCoil


_A variable impedance device normally used to offset line charging during single line faults in an ungrounded section of network._





**URI**: [cim:PetersenCoil](http://iec.ch/TC57/CIM100#PetersenCoil)<br />
**Type**: Class




```mermaid
 classDiagram
    class PetersenCoil
    click PetersenCoil href "../PetersenCoil"
      EarthFaultCompensator <|-- PetersenCoil
        click EarthFaultCompensator href "../EarthFaultCompensator"
      
      PetersenCoil : PetersenCoil.mode
        
          PetersenCoil --> PetersenCoilModeKind : PetersenCoil.mode
          click PetersenCoilModeKind href "../PetersenCoilModeKind"
        
      PetersenCoil : IdentifiedObject.mRID
        
      PetersenCoil : PetersenCoil.nominalU
        
          PetersenCoil --> Voltage : PetersenCoil.nominalU
          click Voltage href "../Voltage"
        
      PetersenCoil : PetersenCoil.offsetCurrent
        
          PetersenCoil --> CurrentFlow : PetersenCoil.offsetCurrent
          click CurrentFlow href "../CurrentFlow"
        
      PetersenCoil : PetersenCoil.positionCurrent
        
          PetersenCoil --> CurrentFlow : PetersenCoil.positionCurrent
          click CurrentFlow href "../CurrentFlow"
        
      PetersenCoil : EarthFaultCompensator.r
        
          PetersenCoil --> Resistance : EarthFaultCompensator.r
          click Resistance href "../Resistance"
        
      PetersenCoil : PetersenCoil.xGroundMax
        
          PetersenCoil --> Reactance : PetersenCoil.xGroundMax
          click Reactance href "../Reactance"
        
      PetersenCoil : PetersenCoil.xGroundMin
        
          PetersenCoil --> Reactance : PetersenCoil.xGroundMin
          click Reactance href "../Reactance"
        
      PetersenCoil : PetersenCoil.xGroundNominal
        
          PetersenCoil --> Reactance : PetersenCoil.xGroundNominal
          click Reactance href "../Reactance"
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [Equipment](Equipment.md)
            * [ConductingEquipment](ConductingEquipment.md)
                * [EarthFaultCompensator](EarthFaultCompensator.md)
                    * **PetersenCoil**



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| mode | [cim:PetersenCoil.mode](http://iec.ch/TC57/CIM100#PetersenCoil.mode) | 1 <br />  [PetersenCoilModeKind](PetersenCoilModeKind.md)  | The mode of operation of the Petersen coil | direct |
| nominalU | [cim:PetersenCoil.nominalU](http://iec.ch/TC57/CIM100#PetersenCoil.nominalU) | 1 <br />  [Voltage](Voltage.md)  | The nominal voltage for which the coil is designed | direct |
| offsetCurrent | [cim:PetersenCoil.offsetCurrent](http://iec.ch/TC57/CIM100#PetersenCoil.offsetCurrent) | 0..1 <br />  [CurrentFlow](CurrentFlow.md)  | The offset current that the Petersen coil controller is operating from the re... | direct |
| positionCurrent | [cim:PetersenCoil.positionCurrent](http://iec.ch/TC57/CIM100#PetersenCoil.positionCurrent) | 0..1 <br />  [CurrentFlow](CurrentFlow.md)  | The control current used to control the Petersen coil also known as the posit... | direct |
| xGroundMax | [cim:PetersenCoil.xGroundMax](http://iec.ch/TC57/CIM100#PetersenCoil.xGroundMax) | 1 <br />  [Reactance](Reactance.md)  | The maximum reactance | direct |
| xGroundMin | [cim:PetersenCoil.xGroundMin](http://iec.ch/TC57/CIM100#PetersenCoil.xGroundMin) | 1 <br />  [Reactance](Reactance.md)  | The minimum reactance | direct |
| xGroundNominal | [cim:PetersenCoil.xGroundNominal](http://iec.ch/TC57/CIM100#PetersenCoil.xGroundNominal) | 1 <br />  [Reactance](Reactance.md)  | The nominal reactance | direct |
| r | [cim:EarthFaultCompensator.r](http://iec.ch/TC57/CIM100#EarthFaultCompensator.r) | 0..1 <br />  [Resistance](Resistance.md)  | Nominal resistance of device | [EarthFaultCompensator](EarthFaultCompensator.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |









## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/ShortCircuit-EU#Package_ShortCircuitProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:PetersenCoil |
| native | this:PetersenCoil |




