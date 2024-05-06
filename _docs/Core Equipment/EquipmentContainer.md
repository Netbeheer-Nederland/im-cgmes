# EquipmentContainer


_A modelling construct to provide a root class for containing equipment._





**URI**: [cim:EquipmentContainer](http://iec.ch/TC57/CIM100#EquipmentContainer)<br />
**Type**: Class




```mermaid
 classDiagram
    class EquipmentContainer
    click EquipmentContainer href "../EquipmentContainer"
      ConnectivityNodeContainer <|-- EquipmentContainer
        click ConnectivityNodeContainer href "../ConnectivityNodeContainer"
      

      EquipmentContainer <|-- Bay
        click Bay href "../Bay"
      EquipmentContainer <|-- DCEquipmentContainer
        click DCEquipmentContainer href "../DCEquipmentContainer"
      EquipmentContainer <|-- Line
        click Line href "../Line"
      EquipmentContainer <|-- Substation
        click Substation href "../Substation"
      EquipmentContainer <|-- VoltageLevel
        click VoltageLevel href "../VoltageLevel"
      
      
      EquipmentContainer : ConnectivityNodeContainer.ConnectivityNodes
        
          EquipmentContainer --> ConnectivityNode : ConnectivityNodeContainer.ConnectivityNodes
          click ConnectivityNode href "../ConnectivityNode"
        
      EquipmentContainer : IdentifiedObject.description
        
      EquipmentContainer : IdentifiedObject.energyIdentCodeEic
        
      EquipmentContainer : EquipmentContainer.Equipments
        
          EquipmentContainer --> Equipment : EquipmentContainer.Equipments
          click Equipment href "../Equipment"
        
      EquipmentContainer : IdentifiedObject.mRID
        
      EquipmentContainer : IdentifiedObject.name
        
      EquipmentContainer : IdentifiedObject.shortName
        
      
```





## Inheritance
* [IdentifiedObject](IdentifiedObject.md)
    * [PowerSystemResource](PowerSystemResource.md)
        * [ConnectivityNodeContainer](ConnectivityNodeContainer.md)
            * **EquipmentContainer**
                * [Bay](Bay.md)
                * [DCEquipmentContainer](DCEquipmentContainer.md)
                * [Line](Line.md)
                * [Substation](Substation.md)
                * [VoltageLevel](VoltageLevel.md)



## Attributes


| Name | URI | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- | --- |
| Equipments | [cim:EquipmentContainer.Equipments](http://iec.ch/TC57/CIM100#EquipmentContainer.Equipments) | * <br />  [Equipment](Equipment.md)  | Contained equipment | direct |
| ConnectivityNodes | [cim:ConnectivityNodeContainer.ConnectivityNodes](http://iec.ch/TC57/CIM100#ConnectivityNodeContainer.ConnectivityNodes) | * <br />  [ConnectivityNode](ConnectivityNode.md)  | Connectivity nodes which belong to this connectivity node container | [ConnectivityNodeContainer](ConnectivityNodeContainer.md) |
| description | [cim:IdentifiedObject.description](http://iec.ch/TC57/CIM100#IdentifiedObject.description) | 0..1 <br />  string  | The description is a free human readable text describing or naming the object | [IdentifiedObject](IdentifiedObject.md) |
| energyIdentCodeEic | [eu:IdentifiedObject.energyIdentCodeEic](http://iec.ch/TC57/CIM100-European#IdentifiedObject.energyIdentCodeEic) | 0..1 <br />  string  | The attribute is used for an exchange of the EIC code (Energy identification ... | [IdentifiedObject](IdentifiedObject.md) |
| mRID | [cim:IdentifiedObject.mRID](http://iec.ch/TC57/CIM100#IdentifiedObject.mRID) | 1 <br />  string  | Master resource identifier issued by a model authority | [IdentifiedObject](IdentifiedObject.md) |
| name | [cim:IdentifiedObject.name](http://iec.ch/TC57/CIM100#IdentifiedObject.name) | 1 <br />  string  | The name is any free human readable and possibly non unique text naming the o... | [IdentifiedObject](IdentifiedObject.md) |
| shortName | [eu:IdentifiedObject.shortName](http://iec.ch/TC57/CIM100-European#IdentifiedObject.shortName) | 0..1 <br />  string  | The attribute is used for an exchange of a human readable short name with len... | [IdentifiedObject](IdentifiedObject.md) |





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [ACDCConverter](ACDCConverter.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [ACLineSegment](ACLineSegment.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [AsynchronousMachine](AsynchronousMachine.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [AuxiliaryEquipment](AuxiliaryEquipment.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [BatteryUnit](BatteryUnit.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [Breaker](Breaker.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [BusbarSection](BusbarSection.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [Clamp](Clamp.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [ConductingEquipment](ConductingEquipment.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [Conductor](Conductor.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [ConformLoad](ConformLoad.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [Connector](Connector.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [CsConverter](CsConverter.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [CurrentTransformer](CurrentTransformer.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [Cut](Cut.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [DCBreaker](DCBreaker.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [DCBusbar](DCBusbar.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [DCChopper](DCChopper.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [DCConductingEquipment](DCConductingEquipment.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [DCDisconnector](DCDisconnector.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [DCGround](DCGround.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [DCLineSegment](DCLineSegment.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [DCSeriesDevice](DCSeriesDevice.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [DCShunt](DCShunt.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [DCSwitch](DCSwitch.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [Disconnector](Disconnector.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [DisconnectingCircuitBreaker](DisconnectingCircuitBreaker.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [EarthFaultCompensator](EarthFaultCompensator.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [EnergyConnection](EnergyConnection.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [EnergyConsumer](EnergyConsumer.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [EnergySource](EnergySource.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [Equipment](Equipment.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [EquivalentBranch](EquivalentBranch.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [EquivalentEquipment](EquivalentEquipment.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [EquivalentInjection](EquivalentInjection.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [EquivalentShunt](EquivalentShunt.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [ExternalNetworkInjection](ExternalNetworkInjection.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [FaultIndicator](FaultIndicator.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [Fuse](Fuse.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [GeneratingUnit](GeneratingUnit.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [Ground](Ground.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [GroundDisconnector](GroundDisconnector.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [GroundingImpedance](GroundingImpedance.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [HydroGeneratingUnit](HydroGeneratingUnit.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [HydroPump](HydroPump.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [Jumper](Jumper.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [Junction](Junction.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [LinearShuntCompensator](LinearShuntCompensator.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [LoadBreakSwitch](LoadBreakSwitch.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [NonConformLoad](NonConformLoad.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [NonlinearShuntCompensator](NonlinearShuntCompensator.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [NuclearGeneratingUnit](NuclearGeneratingUnit.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [PetersenCoil](PetersenCoil.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [PhotoVoltaicUnit](PhotoVoltaicUnit.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [PostLineSensor](PostLineSensor.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [PotentialTransformer](PotentialTransformer.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [PowerElectronicsConnection](PowerElectronicsConnection.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [PowerElectronicsUnit](PowerElectronicsUnit.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [PowerElectronicsWindUnit](PowerElectronicsWindUnit.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [PowerTransformer](PowerTransformer.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [ProtectedSwitch](ProtectedSwitch.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [RegulatingCondEq](RegulatingCondEq.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [RotatingMachine](RotatingMachine.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [Sensor](Sensor.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [SeriesCompensator](SeriesCompensator.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [ShuntCompensator](ShuntCompensator.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [SolarGeneratingUnit](SolarGeneratingUnit.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [StaticVarCompensator](StaticVarCompensator.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [StationSupply](StationSupply.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [SurgeArrester](SurgeArrester.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [Switch](Switch.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [SynchronousMachine](SynchronousMachine.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [ThermalGeneratingUnit](ThermalGeneratingUnit.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [VsConverter](VsConverter.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [WaveTrap](WaveTrap.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |
| [WindGeneratingUnit](WindGeneratingUnit.md) | EquipmentContainer | range | [EquipmentContainer](EquipmentContainer.md) |






## Identifier and Mapping Information







### Schema Source


* from schema: http://iec.ch/TC57/ns/CIM/CoreEquipment-EU#Package_CoreEquipmentProfile





## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | cim:EquipmentContainer |
| native | this:EquipmentContainer |




