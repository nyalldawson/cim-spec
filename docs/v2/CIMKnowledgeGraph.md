


## CIMKnowledgeGraphDataConnection
#### Represents a Knowledge Graph data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string | The workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory) | The workspace factory. 
| customWorkspaceFactoryCLSID | string | The classID of the custom workspace factory. 
| dataset | string | The dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype) | The dataset type. 


### CIMKnowledgeGraphDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| definitionQuery | string | The OpenCypher definition query. 






## CIMKnowledgeGraphInvestigation
#### Represents a Knowledge Graph Investigation. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| URI | string | The URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the source was last modified, as of the last sync. Used to detect when another sync is needed. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 
| sourcePortalUrl | string | The source portal URI of the item. Set if sourced from an external item such as an item on a portal. 


### CIMKnowledgeGraphInvestigation 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection. 
| queries | [[CIMKnowledgeGraphQuery]](CIMKnowledgeGraph.md#cimknowledgegraphquery) | The collection of query definitions. 
| lists | [[CIMKnowledgeGraphList]](CIMKnowledgeGraph.md#cimknowledgegraphlist) | The collection of list definitions. 
| maps | [string] | An array of Map URIs referenced by this Investigation. 
| linkCharts | [string] | An array of Knowledge Graph Link Charts URIs referenced by this Investigation. 
| dataLoadingConfigurations | [[CIMKnowledgeGraphDataLoadingConfiguration]](CIMKnowledgeGraph.md#cimknowledgegraphdataloadingconfiguration) | The array of Data Loading Configurations referenced by this Investigation. All configurations are expected to have unique names. 
| defaultDataLoadingConfigurationName | string | The name of the default Data Loading Configuration referenced by this Investigation. 






## CIMKnowledgeGraphLayer
#### Provides access to properties of a Knowledge Graph layer. 


### CIMDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name. 
| URI | string | The URI of the definition. Typically set by the system and used as an identifier. 
| sourceURI | string | The source URI of the item. Set if sourced from an external item such as an item on a portal. 
| sourceModifiedTime | [TimeInstant](ExternalReferences.md#timeinstant) | The time the source was last modified, as of the last sync. Used to detect when another sync is needed. 
| metadataURI | string | The metadata URI. 
| useSourceMetadata | boolean | A value indicating whether the CIM definition accesses metadata from its data source (the default behavior), or if it has its own metadata stored in the project. 
| sourcePortalUrl | string | The source portal URI of the item. Set if sourced from an external item such as an item on a portal. 


### CIMLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| attribution | string | The attribution text that appears on a map that draws this layer. 
| description | string | The description. 
| layerElevation | [CIMLayerElevationSurface](CIMLayer.md#cimlayerelevationsurface) | The layer elevation. 
| expanded | boolean | A value indicating whether this layer is expanded in the contents pane. 
| layer3DProperties | [CIM3DLayerProperties](CIMLayer.md#cim3dlayerproperties) | The 3D layer properties. 
| layerMasks | [string] | The layer masks. 
| layerType | [enumeration MapLayerType](CIMEnumerations.md#enumeration-maplayertype) | The map layer type. 
| maxScale | double | The maximum scale for layer draw (set as the denominator of the scale's representative fraction). 
| minScale | double | The minimum scale for layer draw (set as the denominator of the scale's representative fraction). 
| showLegends | boolean | A value indicating whether or not to show legends. 
| transparency | double | The transparency of the layer. 
| visibility | boolean | A value indicating whether or not this layer is visible. 
| displayCacheType | [enumeration DisplayCacheType](CIMLayer.md#enumeration-displaycachetype) | The display cache type. 
| maxDisplayCacheAge | double | The maximum display cache age. 
| layerTemplate | [CIMLayerTemplate](CIMLayer.md#cimlayertemplate) | The layer template. 
| popupInfo | [CIMPopupInfo](CIMVectorLayers.md#cimpopupinfo) | The pop-up info. 
| showPopups | boolean | A value indicating whether or not to show pop-ups. 
| serviceLayerID | long | Identifier that will be used to identify the layer in server. 
| charts | [[CIMChart]](CIMCharts.md#cimchart) | Identifier the layer's charts. 
| searchable | boolean | A value indicating whether or not this layer should be included in the search. This property is honored only by layers that support search. 
| refreshRate | double | The amount of time to wait between refreshing the layer. 
| refreshRateUnit | [enumeration esriTimeUnits](ExternalReferences.md#enumeration-esritimeunits) | The units for the amount of time to wait between refreshing the layer. 
| showMapTips | boolean | A value indicating whether or not the display value is shown when hovering over a layer in the view. 
| customProperties | [[CIMStringMap]](CIMRenderers.md#cimstringmap) | The custom properties of the layer. Custom properties are limited to key / value pairs of strings and developers are fully responsible for stored content. 
| webMapLayerID | string | An identifier that will be used to identify the layer in a web map. This value is present if the layer originated in a web map and facilitates matching the layer back to its origin when updating the web map. 
| blendingMode | [enumeration BlendingMode](CIMSymbols.md#enumeration-blendingmode) | The blending mode for the layer. 
| allowDrapingOnIntegratedMesh | boolean | A value indicating whether layer can be draped on integrated mesh. 


### CIMStandaloneTableContainer 

|Property | Type | Description | 
|---------|--------|--------|
| standaloneTables | [string] | The standalone tables as an array of table repository paths. 


### CIMKnowledgeGraphLayerDefinition 

|Property | Type | Description | 
|---------|--------|--------|
| dataConnection | [DataConnection](Types.md#dataconnection) | The data connection. 
| layers | [string] | The layer URIs of the layers in the composite layer. 






## CIMKnowledgeGraphList
#### Represents a Knowledge Graph List. 


### CIMKnowledgeGraphList 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the List. 
| globalIdSetURI | string | The CIM path to the binary reference containing the collection of GlobalIDs that are part of this List. 






## CIMKnowledgeGraphQuery
#### Represents a Knowledge Graph Query. 


### CIMKnowledgeGraphQuery 

|Property | Type | Description | 
|---------|--------|--------|
| name | string | The name of the query. 
| query | string | The query text. 






## CIMKnowledgeGraphTableDataConnection
#### Represents a Knowledge Graph data connection. 


### CIMDataConnection 

|Property | Type | Description | 
|---------|--------|--------|


### CIMStandardDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| workspaceConnectionString | string | The workspace connection string. 
| workspaceFactory | [enumeration WorkspaceFactory](CIMVectorLayers.md#enumeration-workspacefactory) | The workspace factory. 
| customWorkspaceFactoryCLSID | string | The classID of the custom workspace factory. 
| dataset | string | The dataset name. 
| datasetType | [enumeration esriDatasetType](ExternalReferences.md#enumeration-esridatasettype) | The dataset type. 


### CIMKnowledgeGraphDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| definitionQuery | string | The OpenCypher definition query. 


### CIMKnowledgeGraphTableDataConnection 

|Property | Type | Description | 
|---------|--------|--------|
| inclusionSetURI | string | The InclusionSet for the table. 
| exclusionSetURI | string | The ExclusionSet for the table. 



