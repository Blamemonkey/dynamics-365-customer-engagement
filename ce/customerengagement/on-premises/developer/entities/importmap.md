---
title: "ImportMap Entity Reference (Dynamics 365 Customer Engagement)| MicrosoftDocs"
description: "Includes schema information and supported messages for the ImportMap entity."
ms.date: 04/02/2019

ms.topic: "reference"
ms.assetid: 3948cc48-07c8-7f60-0608-71c37158ad7c
author: "KumarVivek"
ms.author: "kvivek"
manager: "annbe"
search.audienceType: 
  - developer

---
# ImportMap Entity Reference

Data map used in import.


## Messages

|Message|Web API Operation|SDK Assembly|
|-|-|-|
|Assign|PATCH [*org URI*]/api/data/v9.0/importmaps(*importmapid*)<br />[Update](/powerapps/developer/common-data-service/webapi/update-delete-entities-using-web-api#basic-update) `ownerid` property.|<xref:Microsoft.Crm.Sdk.Messages.AssignRequest>|
|Create|POST [*org URI*]/api/data/v9.0/importmaps<br />See [Create](/powerapps/developer/common-data-service/webapi/create-entity-web-api)|<xref:Microsoft.Xrm.Sdk.Messages.CreateRequest> or <br /><xref:Microsoft.Xrm.Sdk.IOrganizationService.Create*>|
|Delete|DELETE [*org URI*]/api/data/v9.0/importmaps(*importmapid*)<br />See [Delete](/powerapps/developer/common-data-service/webapi/update-delete-entities-using-web-api#basic-delete)|<xref:Microsoft.Xrm.Sdk.Messages.DeleteRequest> or <br /><xref:Microsoft.Xrm.Sdk.IOrganizationService.Delete*>|
|ExportMappingsImportMap|<xref href="Microsoft.Dynamics.CRM.ExportMappingsImportMap?text=ExportMappingsImportMap Action" />|<xref:Microsoft.Crm.Sdk.Messages.ExportMappingsImportMapRequest>|
|GrantAccess|<xref href="Microsoft.Dynamics.CRM.GrantAccess?text=GrantAccess Action" />|<xref:Microsoft.Crm.Sdk.Messages.GrantAccessRequest>|
|ImportMappingsImportMap|<xref href="Microsoft.Dynamics.CRM.ImportMappingsImportMap?text=ImportMappingsImportMap Action" />|<xref:Microsoft.Crm.Sdk.Messages.ImportMappingsImportMapRequest>|
|ModifyAccess|<xref href="Microsoft.Dynamics.CRM.ModifyAccess?text=ModifyAccess Action" />|<xref:Microsoft.Crm.Sdk.Messages.ModifyAccessRequest>|
|Retrieve|GET [*org URI*]/api/data/v9.0/importmaps(*importmapid*)<br />See [Retrieve](/powerapps/developer/common-data-service/webapi/retrieve-entity-using-web-api)|<xref:Microsoft.Xrm.Sdk.Messages.RetrieveRequest> or <br /><xref:Microsoft.Xrm.Sdk.IOrganizationService.Retrieve*>|
|RetrieveMultiple|GET [*org URI*]/api/data/v9.0/importmaps<br />See [Query Data](/powerapps/developer/common-data-service/webapi/query-data-web-api)|<xref:Microsoft.Xrm.Sdk.Messages.RetrieveMultipleRequest> or <br /><xref:Microsoft.Xrm.Sdk.IOrganizationService.RetrieveMultiple*>|
|RetrievePrincipalAccess|<xref href="Microsoft.Dynamics.CRM.RetrievePrincipalAccess?text=RetrievePrincipalAccess Function" />|<xref:Microsoft.Crm.Sdk.Messages.RetrievePrincipalAccessRequest>|
|RetrieveSharedPrincipalsAndAccess|<xref href="Microsoft.Dynamics.CRM.RetrieveSharedPrincipalsAndAccess?text=RetrieveSharedPrincipalsAndAccess Function" />|<xref:Microsoft.Crm.Sdk.Messages.RetrieveSharedPrincipalsAndAccessRequest>|
|RevokeAccess|<xref href="Microsoft.Dynamics.CRM.RevokeAccess?text=RevokeAccess Action" />|<xref:Microsoft.Crm.Sdk.Messages.RevokeAccessRequest>|
|SetState|PATCH [*org URI*]/api/data/v9.0/importmaps(*importmapid*)<br />[Update](/powerapps/developer/common-data-service/webapi/update-delete-entities-using-web-api#basic-update) `statecode` and `statuscode` properties.|<xref:Microsoft.Crm.Sdk.Messages.SetStateRequest>|
|Update|PATCH [*org URI*]/api/data/v9.0/importmaps(*importmapid*)<br />See [Update](/powerapps/developer/common-data-service/webapi/update-delete-entities-using-web-api#basic-update)|<xref:Microsoft.Xrm.Sdk.Messages.UpdateRequest> or <br /><xref:Microsoft.Xrm.Sdk.IOrganizationService.Update*>|

## Entity Properties

|Property|Value|
|--------|-----|
|CollectionSchemaName|ImportMaps|
|DisplayCollectionName|Data Maps|
|DisplayName|Data Map|
|EntitySetName|importmaps|
|IsBPFEntity|False|
|LogicalCollectionName|importmaps|
|LogicalName|importmap|
|OwnershipType|UserOwned|
|PrimaryIdAttribute|importmapid|
|PrimaryNameAttribute|name|
|SchemaName|ImportMap|

<a name="writable-attributes"></a>

## Writable attributes

These attributes return true for either **IsValidForCreate** or **IsValidForUpdate** (usually both). Listed by **SchemaName**.

- [Description](#BKMK_Description)
- [EntitiesPerFile](#BKMK_EntitiesPerFile)
- [ImportMapId](#BKMK_ImportMapId)
- [ImportMapType](#BKMK_ImportMapType)
- [IntroducedVersion](#BKMK_IntroducedVersion)
- [IsWizardCreated](#BKMK_IsWizardCreated)
- [MapCustomizations](#BKMK_MapCustomizations)
- [Name](#BKMK_Name)
- [OwnerId](#BKMK_OwnerId)
- [OwnerIdType](#BKMK_OwnerIdType)
- [Source](#BKMK_Source)
- [SourceType](#BKMK_SourceType)
- [SourceUserIdentifierForSourceCRMUserLink](#BKMK_SourceUserIdentifierForSourceCRMUserLink)
- [SourceUserIdentifierForSourceDataSourceUserLink](#BKMK_SourceUserIdentifierForSourceDataSourceUserLink)
- [StateCode](#BKMK_StateCode)
- [StatusCode](#BKMK_StatusCode)
- [TargetUserIdentifierForSourceCRMUserLink](#BKMK_TargetUserIdentifierForSourceCRMUserLink)


### <a name="BKMK_Description"></a> Description

|Property|Value|
|--------|-----|
|Description|Type additional information to describe the data map, such as the intended use or data source.|
|DisplayName|Description|
|FormatName|TextArea|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|description|
|MaxLength|2000|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_EntitiesPerFile"></a> EntitiesPerFile

|Property|Value|
|--------|-----|
|Description|Choose whether a data file can contain data for one or more record types.|
|DisplayName|Entities Per File|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|entitiesperfile|
|RequiredLevel|SystemRequired|
|Type|Picklist|

#### EntitiesPerFile Options

|Value|Label|
|-----|-----|
|1|Single Entity Per File|
|2|Multiple Entities Per File|



### <a name="BKMK_ImportMapId"></a> ImportMapId

|Property|Value|
|--------|-----|
|Description|Unique identifier of the data map.|
|DisplayName|Data Map|
|IsValidForForm|False|
|IsValidForRead|True|
|IsValidForUpdate|False|
|LogicalName|importmapid|
|RequiredLevel|SystemRequired|
|Type|Uniqueidentifier|


### <a name="BKMK_ImportMapType"></a> ImportMapType

|Property|Value|
|--------|-----|
|Description|Select the type of data map to distinguish out-of-the-box data maps from custom maps.|
|DisplayName|Map Type|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|importmaptype|
|RequiredLevel|None|
|Type|Picklist|

#### ImportMapType Options

|Value|Label|
|-----|-----|
|1|Standard|
|2|Out of Box|
|3|In Process|



### <a name="BKMK_IntroducedVersion"></a> IntroducedVersion

|Property|Value|
|--------|-----|
|Description|Version in which the component is introduced.|
|DisplayName|Introduced Version|
|FormatName|VersionNumber|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|IsValidForUpdate|False|
|LogicalName|introducedversion|
|MaxLength|48|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_IsWizardCreated"></a> IsWizardCreated

|Property|Value|
|--------|-----|
|Description|Information about whether this data map was created by the Data Migration Manager.|
|DisplayName|Is Wizard-Created|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|iswizardcreated|
|RequiredLevel|None|
|Type|Boolean|

#### IsWizardCreated Options

|Value|Label|
|-----|-----|
|1|True|
|0|False|

**DefaultValue**: False



### <a name="BKMK_MapCustomizations"></a> MapCustomizations

|Property|Value|
|--------|-----|
|Description|Customizations XML|
|DisplayName|Map Customizations|
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|mapcustomizations|
|MaxLength|1073741823|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_Name"></a> Name

|Property|Value|
|--------|-----|
|Description|Type a descriptive name for the data map.|
|DisplayName|Map Name|
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|name|
|MaxLength|320|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_OwnerId"></a> OwnerId

|Property|Value|
|--------|-----|
|Description|Enter the user or team who is assigned to manage the record. This field is updated every time the record is assigned to a different user.|
|DisplayName|Owner|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|ownerid|
|RequiredLevel|SystemRequired|
|Targets|systemuser,team|
|Type|Owner|


### <a name="BKMK_OwnerIdType"></a> OwnerIdType

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|owneridtype|
|RequiredLevel|SystemRequired|
|Type|EntityName|


### <a name="BKMK_Source"></a> Source

|Property|Value|
|--------|-----|
|Description|Type the name of the migration source that this data map is used for.|
|DisplayName|Source|
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|source|
|MaxLength|160|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_SourceType"></a> SourceType

|Property|Value|
|--------|-----|
|Description|Select the migration source type that this data map is used for.|
|DisplayName|Source System Type|
|IsValidForForm|True|
|IsValidForRead|True|
|IsValidForUpdate|False|
|LogicalName|sourcetype|
|RequiredLevel|None|
|Type|Picklist|

#### SourceType Options

|Value|Label|
|-----|-----|
|1|Map For SalesForce.com Full Data Export|
|2|Map For SalesForce.com Report Export|
|3|Map For SalesForce.com Contact and Account Report Export|
|4|Microsoft Office Outlook 2010 with Business Contact Manager|
|5|Generic Map for Contact and Account|



### <a name="BKMK_SourceUserIdentifierForSourceCRMUserLink"></a> SourceUserIdentifierForSourceCRMUserLink

|Property|Value|
|--------|-----|
|Description|Source user value for source Microsoft Dynamics 365 user link.|
|DisplayName|Source User Value|
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|sourceuseridentifierforsourcecrmuserlink|
|MaxLength|160|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_SourceUserIdentifierForSourceDataSourceUserLink"></a> SourceUserIdentifierForSourceDataSourceUserLink

|Property|Value|
|--------|-----|
|Description|Column in the source file that uniquely identifies a user.|
|DisplayName|Source User Identifier|
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|sourceuseridentifierforsourcedatasourceuserlink|
|MaxLength|160|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_StateCode"></a> StateCode

|Property|Value|
|--------|-----|
|Description|Shows whether the data map is active or inactive. Inactive data maps are read-only and can't be edited.|
|DisplayName|Status|
|IsValidForCreate|False|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|statecode|
|RequiredLevel|SystemRequired|
|Type|State|

#### StateCode Options

|Value|Label|DefaultStatus|InvariantName|
|-----|-----|-------------|-------------|
|0|Active|1|Active|
|1|Inactive|2|Inactive|



### <a name="BKMK_StatusCode"></a> StatusCode

|Property|Value|
|--------|-----|
|Description|Select the data map's status.|
|DisplayName|Status Reason|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|statuscode|
|RequiredLevel|SystemRequired|
|Type|Status|

#### StatusCode Options

|Value|Label|State|
|-----|-----|-----|
|1|Active|0|
|2|Inactive|1|



### <a name="BKMK_TargetUserIdentifierForSourceCRMUserLink"></a> TargetUserIdentifierForSourceCRMUserLink

|Property|Value|
|--------|-----|
|Description|Microsoft Dynamics 365 user.|
|DisplayName|Target User Value|
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|targetuseridentifierforsourcecrmuserlink|
|MaxLength|160|
|RequiredLevel|None|
|Type|String|

<a name="read-only-attributes"></a>

## Read-only attributes

These attributes return false for both **IsValidForCreate** or **IsValidForUpdate**. Listed by **SchemaName**.

- [ComponentState](#BKMK_ComponentState)
- [CreatedBy](#BKMK_CreatedBy)
- [CreatedByName](#BKMK_CreatedByName)
- [CreatedByYomiName](#BKMK_CreatedByYomiName)
- [CreatedOn](#BKMK_CreatedOn)
- [CreatedOnBehalfBy](#BKMK_CreatedOnBehalfBy)
- [CreatedOnBehalfByName](#BKMK_CreatedOnBehalfByName)
- [CreatedOnBehalfByYomiName](#BKMK_CreatedOnBehalfByYomiName)
- [ImportMapIdUnique](#BKMK_ImportMapIdUnique)
- [IsManaged](#BKMK_IsManaged)
- [IsValidForImport](#BKMK_IsValidForImport)
- [ModifiedBy](#BKMK_ModifiedBy)
- [ModifiedByName](#BKMK_ModifiedByName)
- [ModifiedByYomiName](#BKMK_ModifiedByYomiName)
- [ModifiedOn](#BKMK_ModifiedOn)
- [ModifiedOnBehalfBy](#BKMK_ModifiedOnBehalfBy)
- [ModifiedOnBehalfByName](#BKMK_ModifiedOnBehalfByName)
- [ModifiedOnBehalfByYomiName](#BKMK_ModifiedOnBehalfByYomiName)
- [OverwriteTime](#BKMK_OverwriteTime)
- [OwnerIdName](#BKMK_OwnerIdName)
- [OwnerIdYomiName](#BKMK_OwnerIdYomiName)
- [OwningBusinessUnit](#BKMK_OwningBusinessUnit)
- [OwningTeam](#BKMK_OwningTeam)
- [OwningUser](#BKMK_OwningUser)
- [SolutionId](#BKMK_SolutionId)
- [SupportingSolutionId](#BKMK_SupportingSolutionId)
- [TargetEntity](#BKMK_TargetEntity)


### <a name="BKMK_ComponentState"></a> ComponentState

|Property|Value|
|--------|-----|
|Description|For internal use only.|
|DisplayName|Component State|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|componentstate|
|RequiredLevel|SystemRequired|
|Type|Picklist|

#### ComponentState Options

|Value|Label|
|-----|-----|
|0|Published|
|1|Unpublished|
|2|Deleted|
|3|Deleted Unpublished|



### <a name="BKMK_CreatedBy"></a> CreatedBy

|Property|Value|
|--------|-----|
|Description|Shows who created the record.|
|DisplayName|Created By|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|createdby|
|RequiredLevel|None|
|Targets|systemuser|
|Type|Lookup|


### <a name="BKMK_CreatedByName"></a> CreatedByName

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|createdbyname|
|MaxLength|100|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_CreatedByYomiName"></a> CreatedByYomiName

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|createdbyyominame|
|MaxLength|100|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_CreatedOn"></a> CreatedOn

|Property|Value|
|--------|-----|
|DateTimeBehavior|UserLocal|
|Description|Shows the date and time when the record was created. The date and time are displayed in the time zone selected in Microsoft Dynamics 365 options.|
|DisplayName|Created On|
|Format|DateAndTime|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|createdon|
|RequiredLevel|SystemRequired|
|Type|DateTime|


### <a name="BKMK_CreatedOnBehalfBy"></a> CreatedOnBehalfBy

|Property|Value|
|--------|-----|
|Description|Shows who created the record on behalf of another user.|
|DisplayName|Created By (Delegate)|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|createdonbehalfby|
|RequiredLevel|None|
|Targets|systemuser|
|Type|Lookup|


### <a name="BKMK_CreatedOnBehalfByName"></a> CreatedOnBehalfByName

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|createdonbehalfbyname|
|MaxLength|100|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_CreatedOnBehalfByYomiName"></a> CreatedOnBehalfByYomiName

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|createdonbehalfbyyominame|
|MaxLength|100|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_ImportMapIdUnique"></a> ImportMapIdUnique

|Property|Value|
|--------|-----|
|Description|Unique identifier of the ImortMap.|
|DisplayName||
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|importmapidunique|
|RequiredLevel|SystemRequired|
|Type|Uniqueidentifier|


### <a name="BKMK_IsManaged"></a> IsManaged

|Property|Value|
|--------|-----|
|Description|Information that specifies whether this component is managed.|
|DisplayName|State|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|ismanaged|
|RequiredLevel|SystemRequired|
|Type|Boolean|

#### IsManaged Options

|Value|Label|
|-----|-----|
|1|Managed|
|0|Unmanaged|

**DefaultValue**: False



### <a name="BKMK_IsValidForImport"></a> IsValidForImport

|Property|Value|
|--------|-----|
|Description|Information about whether the data map is valid for use with data import.|
|DisplayName|Is Valid For Import|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|isvalidforimport|
|RequiredLevel|None|
|Type|Boolean|

#### IsValidForImport Options

|Value|Label|
|-----|-----|
|1|Yes|
|0|No|

**DefaultValue**: False



### <a name="BKMK_ModifiedBy"></a> ModifiedBy

|Property|Value|
|--------|-----|
|Description|Shows who last updated the record.|
|DisplayName|Modified By|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|modifiedby|
|RequiredLevel|None|
|Targets|systemuser|
|Type|Lookup|


### <a name="BKMK_ModifiedByName"></a> ModifiedByName

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|modifiedbyname|
|MaxLength|100|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_ModifiedByYomiName"></a> ModifiedByYomiName

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|modifiedbyyominame|
|MaxLength|100|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_ModifiedOn"></a> ModifiedOn

|Property|Value|
|--------|-----|
|DateTimeBehavior|UserLocal|
|Description|Shows the date and time when the record was last updated. The date and time are displayed in the time zone selected in Microsoft Dynamics 365 options.|
|DisplayName|Modified On|
|Format|DateAndTime|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|modifiedon|
|RequiredLevel|SystemRequired|
|Type|DateTime|


### <a name="BKMK_ModifiedOnBehalfBy"></a> ModifiedOnBehalfBy

|Property|Value|
|--------|-----|
|Description|Shows who last updated the record on behalf of another user.|
|DisplayName|Modified By (Delegate)|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|modifiedonbehalfby|
|RequiredLevel|None|
|Targets|systemuser|
|Type|Lookup|


### <a name="BKMK_ModifiedOnBehalfByName"></a> ModifiedOnBehalfByName

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|modifiedonbehalfbyname|
|MaxLength|100|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_ModifiedOnBehalfByYomiName"></a> ModifiedOnBehalfByYomiName

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|modifiedonbehalfbyyominame|
|MaxLength|100|
|RequiredLevel|None|
|Type|String|


### <a name="BKMK_OverwriteTime"></a> OverwriteTime

|Property|Value|
|--------|-----|
|DateTimeBehavior|UserLocal|
|Description|For internal use only.|
|DisplayName|Record Overwrite Time|
|Format|DateOnly|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|overwritetime|
|RequiredLevel|SystemRequired|
|Type|DateTime|


### <a name="BKMK_OwnerIdName"></a> OwnerIdName

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|owneridname|
|MaxLength|100|
|RequiredLevel|SystemRequired|
|Type|String|


### <a name="BKMK_OwnerIdYomiName"></a> OwnerIdYomiName

|Property|Value|
|--------|-----|
|Description||
|DisplayName||
|FormatName|Text|
|IsLocalizable|False|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|owneridyominame|
|MaxLength|100|
|RequiredLevel|SystemRequired|
|Type|String|


### <a name="BKMK_OwningBusinessUnit"></a> OwningBusinessUnit

|Property|Value|
|--------|-----|
|Description|Business unit that owns the data map.|
|DisplayName|Owning Business Unit|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|owningbusinessunit|
|RequiredLevel|None|
|Targets|businessunit|
|Type|Lookup|


### <a name="BKMK_OwningTeam"></a> OwningTeam

|Property|Value|
|--------|-----|
|Description|Unique identifier of the team who owns the data map.|
|DisplayName|Owning Team|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|owningteam|
|RequiredLevel|None|
|Targets|team|
|Type|Lookup|


### <a name="BKMK_OwningUser"></a> OwningUser

|Property|Value|
|--------|-----|
|Description|Unique identifier of the user who owns the data map.|
|DisplayName|Owning User|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|owninguser|
|RequiredLevel|None|
|Targets|systemuser|
|Type|Lookup|


### <a name="BKMK_SolutionId"></a> SolutionId

|Property|Value|
|--------|-----|
|Description|Unique identifier of the associated solution.|
|DisplayName|Solution|
|IsValidForForm|False|
|IsValidForRead|True|
|LogicalName|solutionid|
|RequiredLevel|SystemRequired|
|Type|Uniqueidentifier|


### <a name="BKMK_SupportingSolutionId"></a> SupportingSolutionId

|Property|Value|
|--------|-----|
|Description|For internal use only.|
|DisplayName|Solution|
|IsValidForForm|False|
|IsValidForRead|False|
|LogicalName|supportingsolutionid|
|RequiredLevel|None|
|Type|Uniqueidentifier|


### <a name="BKMK_TargetEntity"></a> TargetEntity

|Property|Value|
|--------|-----|
|Description|Select the name of the Microsoft Dynamics 365 record type that this data map is defined for.|
|DisplayName|Record Type|
|IsValidForForm|True|
|IsValidForRead|True|
|LogicalName|targetentity|
|RequiredLevel|ApplicationRequired|
|Type|Picklist|

#### TargetEntity Options

|Value|Label|
|-----|-----|
|1|Account|
|2|Contact|
|3|Opportunity|
|4|Lead|
|5|Note|
|6|Business Unit Map|
|7|Owner|
|8|User|
|9|Team|
|10|Business Unit|
|14|System User Principal|
|16|AccountLeads|
|17|ContactInvoices|
|18|ContactQuotes|
|19|ContactOrders|
|20|Service Contract Contact|
|21|ProductSalesLiterature|
|22|ContactLeads|
|24|LeadCompetitors|
|25|OpportunityCompetitors|
|26|CompetitorSalesLiterature|
|27|LeadProduct|
|29|Subscription|
|30|Filter Template|
|31|Privilege Object Type Code|
|32|Sales Process Instance|
|33|Subscription Synchronization Information|
|35|Tracking information for deleted entities|
|36|Client update|
|37|Subscription Manually Tracked Object|
|42|SystemUser BusinessUnit Entity Map|
|44|Field Sharing|
|45|Subscription Statistic Offline|
|46|Subscription Statistic Outlook|
|47|Subscription Sync Entry Offline|
|48|Subscription Sync Entry Outlook|
|50|Position|
|51|System User Manager Map|
|52|User Search Facet|
|54|Global Search Configuration|
|55|FileAttachment|
|78|Virtual Entity Data Provider|
|85|Virtual Entity Data Source|
|92|Team template|
|99|Social Profile|
|112|Case|
|113|Child Incident Count|
|123|Competitor|
|126|Indexed Article|
|127|Article|
|129|Subject|
|132|Announcement|
|135|Activity Party|
|150|User Settings|
|300|Canvas App|
|301|Callback Registration|
|371|Connector|
|950|New Process|
|951|Translation Process|
|952|Phone To Case Process|
|953|Opportunity Sales Process|
|954|Lead To Opportunity Sales Process|
|955|Expired Process|
|1001|Attachment|
|1002|Attachment|
|1003|Internal Address|
|1004|Competitor Address|
|1006|Competitor Product|
|1007|Image Descriptor|
|1010|Contract|
|1011|Contract Line|
|1013|Discount|
|1016|Article Template|
|1017|Lead Address|
|1019|Organization|
|1021|Organization UI|
|1022|Price List|
|1023|Privilege|
|1024|Product|
|1025|Product Association|
|1026|Price List Item|
|1028|Product Relationship|
|1030|System Form|
|1031|User Dashboard|
|1036|Security Role|
|1037|Role Template|
|1038|Sales Literature|
|1039|View|
|1043|String Map|
|1048|Property|
|1049|Property Option Set Item|
|1055|Unit|
|1056|Unit Group|
|1070|Sales Attachment|
|1071|Address|
|1072|Subscription Clients|
|1075|Status Map|
|1080|Discount List|
|1082|Article Comment|
|1083|Opportunity Line|
|1084|Quote|
|1085|Quote Line|
|1086|User Fiscal Calendar|
|1088|Order|
|1089|Order Line|
|1090|Invoice|
|1091|Invoice Line|
|1094|Authorization Server|
|1095|Partner Application|
|1111|System Chart|
|1112|User Chart|
|1113|Ribbon Tab To Command Mapping|
|1115|Ribbon Context Group|
|1116|Ribbon Command|
|1117|Ribbon Rule|
|1120|Application Ribbons|
|1130|Ribbon Difference|
|1140|Replication Backlog|
|1141|Characteristic|
|1142|Rating Value|
|1144|Rating Model|
|1145|Bookable Resource Booking|
|1146|Bookable Resource Booking Header|
|1147|Bookable Resource Category|
|1148|Bookable Resource Characteristic|
|1149|Bookable Resource Category Assn|
|1150|Bookable Resource|
|1151|Bookable Resource Group|
|1152|Booking Status|
|1189|Document Suggestions|
|1190|SuggestionCardTemplate|
|1200|Field Security Profile|
|1201|Field Permission|
|1203|Team Profiles|
|1234|Channel Property Group|
|1235|Property Association|
|1236|Channel Property|
|1300|SocialInsightsConfiguration|
|1309|Saved Organization Insights Configuration|
|1333|Property Instance|
|1400|Sync Attribute Mapping Profile|
|1401|Sync Attribute Mapping|
|1403|Team Sync-Attribute Mapping Profiles|
|1404|Principal Sync Attribute Map|
|2000|Annual Fiscal Calendar|
|2001|Semiannual Fiscal Calendar|
|2002|Quarterly Fiscal Calendar|
|2003|Monthly Fiscal Calendar|
|2004|Fixed Monthly Fiscal Calendar|
|2010|Email Template|
|2011|Contract Template|
|2012|Unresolved Address|
|2013|Territory|
|2015|Theme|
|2016|User Mapping|
|2020|Queue|
|2023|QueueItemCount|
|2024|QueueMemberCount|
|2027|License|
|2029|Queue Item|
|2500|User Entity UI Settings|
|2501|User Entity Instance Data|
|3000|Integration Status|
|3005|Channel Access Profile|
|3008|External Party|
|3231|Connection Role|
|3233|Connection Role Object Type Code|
|3234|Connection|
|4000|Facility/Equipment|
|4001|Service|
|4002|Resource|
|4003|Calendar|
|4004|Calendar Rule|
|4005|Scheduling Group|
|4006|Resource Specification|
|4007|Resource Group|
|4009|Site|
|4010|Resource Expansion|
|4011|Inter Process Lock|
|4023|Email Hash|
|4101|Display String Map|
|4102|Display String|
|4110|Notification|
|4120|Exchange Sync Id Mapping|
|4200|Activity|
|4201|Appointment|
|4202|Email|
|4204|Fax|
|4206|Case Resolution|
|4207|Letter|
|4208|Opportunity Close|
|4209|Order Close|
|4210|Phone Call|
|4211|Quote Close|
|4212|Task|
|4214|Service Activity|
|4215|Commitment|
|4216|Social Activity|
|4220|UntrackedEmail|
|4230|Saved View|
|4231|Metadata Difference|
|4232|Business Data Localized Label|
|4250|Recurrence Rule|
|4251|Recurring Appointment|
|4299|Email Search|
|4300|Marketing List|
|4301|Marketing List Member|
|4400|Campaign|
|4401|Campaign Response|
|4402|Campaign Activity|
|4403|Campaign Item|
|4404|Campaign Activity Item|
|4405|Bulk Operation Log|
|4406|Quick Campaign|
|4410|Data Import|
|4411|Data Map|
|4412|Import Source File|
|4413|Import Data|
|4414|Duplicate Detection Rule|
|4415|Duplicate Record|
|4416|Duplicate Rule Condition|
|4417|Column Mapping|
|4418|List Value Mapping|
|4419|Lookup Mapping|
|4420|Owner Mapping|
|4421|Bookable Resource Booking to Exchange Id Mapping|
|4423|Import Log|
|4424|Bulk Delete Operation|
|4425|Bulk Delete Failure|
|4426|Transformation Mapping|
|4427|Transformation Parameter Mapping|
|4428|Import Entity Mapping|
|4450|Data Performance Dashboard|
|4490|Office Document|
|4500|Relationship Role|
|4501|Relationship Role Map|
|4502|Customer Relationship|
|4503|Opportunity Relationship|
|4545|Entitlement Template Product|
|4567|Auditing|
|4579|Ribbon Client Metadata.|
|4600|Entity Map|
|4601|Attribute Map|
|4602|Plug-in Type|
|4603|Plug-in Type Statistic|
|4605|Plug-in Assembly|
|4606|Sdk Message|
|4607|Sdk Message Filter|
|4608|Sdk Message Processing Step|
|4609|Sdk Message Request|
|4610|Sdk Message Response|
|4611|Sdk Message Response Field|
|4613|Sdk Message Pair|
|4614|Sdk Message Request Field|
|4615|Sdk Message Processing Step Image|
|4616|Sdk Message Processing Step Secure Configuration|
|4618|Service Endpoint|
|4619|Plug-in Trace Log|
|4700|System Job|
|4702|Workflow Wait Subscription|
|4703|Process|
|4704|Process Dependency|
|4705|ISV Config|
|4706|Process Log|
|4707|Application File|
|4708|Organization Statistic|
|4709|Site Map|
|4710|Process Session|
|4711|Expander Event|
|4712|Process Trigger|
|4724|Process Stage|
|4725|Business Process Flow Instance|
|4800|Web Wizard|
|4802|Wizard Page|
|4803|Web Wizard Access Privilege|
|4810|Time Zone Definition|
|4811|Time Zone Rule|
|4812|Time Zone Localized Name|
|6363|Entitlement Product|
|7000|System Application Metadata|
|7001|User Application Metadata|
|7100|Solution|
|7101|Publisher|
|7102|Publisher Address|
|7103|Solution Component|
|7105|Dependency|
|7106|Dependency Node|
|7107|Invalid Dependency|
|7108|Dependency Feature|
|7200|RuntimeDependency|
|7272|Entitlement Contact|
|8000|Post|
|8001|Post Role|
|8002|Post Regarding|
|8003|Follow|
|8005|Comment|
|8006|Like|
|8040|ACIViewMapper|
|8050|Trace|
|8051|Trace Association|
|8052|Trace Regarding|
|8181|Routing Rule Set|
|8199|Rule Item|
|8700|AppModule Metadata|
|8701|AppModule Metadata Dependency|
|8702|AppModule Metadata Async Operation|
|8840|Hierarchy Rule|
|9006|Model-driven App|
|9007|App Module Component|
|9009|App Module Roles|
|9011|App Config Master|
|9012|App Configuration|
|9013|App Configuration Instance|
|9100|Report|
|9101|Report Related Entity|
|9102|Report Related Category|
|9103|Report Visibility|
|9104|Report Link|
|9105|Currency|
|9106|Mail Merge Template|
|9107|Import Job|
|9201|LocalConfigStore|
|9300|Record Creation and Update Rule|
|9301|Record Creation and Update Rule Item|
|9333|Web Resource|
|9400|Channel Access Profile Rule|
|9401|Channel Access Profile Rule Item|
|9502|SharePoint Site|
|9507|Sharepoint Document|
|9508|Document Location|
|9509|SharePoint Data|
|9510|Rollup Properties|
|9511|Rollup Job|
|9600|Goal|
|9602|Rollup Query|
|9603|Goal Metric|
|9604|Rollup Field|
|9605|Email Server Profile|
|9606|Mailbox|
|9607|Mailbox Statistics|
|9608|Mailbox Auto Tracking Folder|
|9609|Mailbox Tracking Category|
|9650|Process Configuration|
|9690|Organization Insights Notification|
|9699|Organization Insights Metric|
|9700|Entitlement|
|9701|Entitlement Channel|
|9702|Entitlement Template|
|9703|Entitlement Template Channel|
|9704|Entitlement Entity Allocation Type Mapping|
|9750|SLA|
|9751|SLA Item|
|9752|SLA KPI Instance|
|9753|Custom Control|
|9754|Custom Control Resource|
|9755|Custom Control Default Config|
|9866|Mobile Offline Profile|
|9867|Mobile Offline Profile Item|
|9868|Mobile Offline Profile Item Association|
|9869|Sync Error|
|9870|Offline Command Definition|
|9875|Language Provisioning State|
|9890|SolutionHistoryData|
|9900|Navigation Setting|
|9910|MultiEntitySearch|
|9912|Multi Select Option Value|
|9919|Hierarchy Security Configuration|
|9930|Knowledge Base Record|
|9931|Incident KnowledgeBaseRecord|
|9932|Time Stamp Date Mapping|
|9936|Azure Service Connection|
|9940|Document Template|
|9941|Personal Document Template|
|9942|Topic Model Configuration|
|9943|Topic Model Execution History|
|9944|Topic Model|
|9945|Text Analytics Entity Mapping|
|9946|Topic History|
|9947|Knowledge Search Model|
|9948|Text Analytics Topic|
|9949|Advanced Similarity Rule|
|9950|Office Graph Document|
|9951|Similarity Rule|
|9953|Knowledge Article|
|9954|Knowledge Article Incident|
|9955|Knowledge Article Views|
|9957|Language|
|9958|Feedback|
|9959|Category|
|9960|Knowledge Article Category|
|9961|DelveActionHub|
|9962|Action Card|
|9968|ActionCardUserState|
|9973|Action Card User Settings|
|9983|Action Card Type|
|9986|Interaction for Email|
|9987|External Party Item|
|9996|HolidayWrapper|
|9997|Email Signature|
|10000|OData v4 Data Source|
|10001|Solution Component Summary|
|10002|Solution Component Data Source|
|10003|Solution History|
|10004|Solution History Data Source|
|10005|Component Layer|
|10006|Component Layer Data Source|
|10007|Database Version|
|10008|Upgrade Run|
|10009|Upgrade Step|
|10010|Upgrade Version|
|10011|Playbook Callable Context|
|10012|Playbook activity|
|10013|Playbook activity attribute|
|10014|Playbook category|
|10015|Playbook|
|10016|Playbook template|
|10018|admin_settings_entity|
|10019|Forecast definition|
|10020|Forecast|
|10021|Forecast recurrence|
|10022|msdyn_relationshipinsightsunifiedconfig|
|10023|siconfig|
|10024|UntrackedAppointment|
|10025|Notes analysis Config|
|10026|icebreakersconfig|
|10027|Profile Album|
|10028|Post Configuration|
|10029|Post Rule Configuration|
|10030|Wall View|
|10031|Filter|
|10032|Survey email template|
|10033|Survey question|
|10034|Survey question response|
|10035|Survey|
|10036|Survey invite|
|10037|Survey response|
|10038|Unsubscribed recipient|
|10039|Microsoft Teams Collaboration entity|
|10040|Actual|
|10041|Bookable Resource Association|
|10042|Booking Alert|
|10043|Booking Alert Status|
|10044|Booking Change|
|10045|Booking Rule|
|10046|Booking Setup Metadata|
|10047|Business Closure|
|10048|Client Extension|
|10049|Configuration|
|10050|Organizational Unit|
|10051|Priority|
|10052|Requirement Characteristic|
|10053|Requirement Group|
|10054|Requirement Organization Unit|
|10055|Requirement Relationship|
|10056|Requirement Resource Category|
|10057|Requirement Resource Preference|
|10058|Requirement Status|
|10059|Resource Requirement|
|10060|Resource Requirement Detail|
|10061|Resource Territory|
|10062|Schedule Board Setting|
|10063|Scheduling Parameter|
|10064|System User Scheduler Setting|
|10065|Fulfillment Preference|
|10066|Time Group Detail|
|10067|Transaction Origin|
|10068|Work template|
|10069|Account Project Price List|
|10070|Project Service Approval|
|10071|Batch Job|
|10072|Project Stages|
|10073|Invoice Process|
|10074|Competency Requirement (Deprecated)|
|10075|Contact Price List|
|10076|Project Contract Line Invoice Schedule|
|10077|Project Contract Line Milestone|
|10078|Actual Data Export (Deprecated)|
|10079|Delegation|
|10080|Pricing Dimension|
|10081|Pricing Dimension Field Name|
|10082|Estimate|
|10083|Estimate Line|
|10084|Expense|
|10085|Expense Category|
|10086|Expense Receipt|
|10087|Fact|
|10088|Field Computation|
|10089|Find Work Event (Deprecated in v3.0)|
|10090|Integration Job|
|10091|Integration Job Detail|
|10092|Invoice Frequency|
|10093|Invoice Frequency Detail|
|10094|Invoice Line Detail|
|10095|Journal|
|10096|Journal Line|
|10097|Result Cache|
|10098|Opportunity Line Resource Category (Deprecated)|
|10099|Opportunity Line Detail (Deprecated)|
|10100|Opportunity Line Transaction Category (Deprecated)|
|10101|Opportunity Line Transaction Classification (Deprecated)|
|10102|Opportunity Project Price List|
|10103|Project Contract Line Resource Category|
|10104|Project Contract Line Detail|
|10105|Project Contract Line Transaction Category|
|10106|Project Contract Line Transaction Classification|
|10107|Project Contract Project Price List|
|10108|Process Notes|
|10109|Project|
|10110|Project Approval|
|10111|Project Parameter|
|10112|Project Parameter Price List|
|10113|Project Price List|
|10114|Project Task|
|10115|Project Task Dependency|
|10116|Project Task Status User|
|10117|Project Team Member|
|10118|Project Team Member Sign-Up (Deprecated in v3.0)|
|10119|Project Transaction Category (Deprecated)|
|10120|Quote Line Analytics Breakdown|
|10121|Quote Line Invoice Schedule|
|10122|Quote Line Resource Category|
|10123|Quote Line Milestone|
|10124|Quote Line Detail|
|10125|Quote Line Transaction Category|
|10126|Quote Line Transaction Classification|
|10127|Quote Project Price List|
|10128|Resource Assignment|
|10129|Resource Assignment Detail (Deprecated in v2.0)|
|10130|Role Price Markup|
|10131|Role Price|
|10132|Resource Request|
|10133|Role competency requirement|
|10134|Role Utilization|
|10135|Time Entry|
|10136|Time Off Calendar|
|10137|Transaction Category|
|10138|Transaction Category Classification|
|10139|Transaction Category Hierarchy Element|
|10140|Transaction Category Price|
|10141|Transaction Connection|
|10142|Transaction Type|
|10143|User Work History|
|10148|Three-Dimensional Model|
|10149|Analysis Component|
|10150|Analysis Job|
|10151|Analysis Result|
|10152|Analysis Result Detail|
|10153|Solution Health Rule|
|10154|Solution Health Rule Argument|
|10155|Solution Health Rule Set|
|10156|Agreement|
|10157|Agreement Booking Date|
|10158|Agreement Booking Incident|
|10159|Agreement Booking Product|
|10160|Agreement Booking Service|
|10161|Agreement Booking Service Task|
|10162|Agreement Booking Setup|
|10163|Agreement Invoice Date|
|10164|Agreement Invoice Product|
|10165|Agreement Invoice Setup|
|10166|Agreement Substatus|
|10167|Booking Journal|
|10168|Booking Timestamp|
|10169|Purchase Order Business Process|
|10170|Case to Work Order Business Process|
|10171|Agreement Business Process|
|10172|Work Order Business Process|
|10173|Customer Asset|
|10174|Customer Asset Category|
|10175|Entitlement Application|
|10176|Field Service Price List Item|
|10177|Field Service Setting|
|10178|Field Service SLA Configuration|
|10179|Field Service System Job|
|10180|Incident Type|
|10181|Incident Type Characteristic|
|10182|Incident Type Product|
|10183|Incident Type Service|
|10184|Incident Type Service Task|
|10185|Incident Types Setup|
|10186|Incident Type Requirement Group|
|10187|Inventory Adjustment|
|10188|Inventory Adjustment Product|
|10189|Inventory Journal|
|10190|Inventory Transfer|
|10191|Order Invoicing Date|
|10192|Order Invoicing Product|
|10193|Order Invoicing Setup|
|10194|Order Invoicing Setup Date|
|10195|Payment|
|10196|Payment Detail|
|10197|Payment Method|
|10198|Payment Term|
|10199|Postal Code|
|10200|Product Inventory|
|10201|Purchase Order|
|10202|Purchase Order Bill|
|10203|Purchase Order Product|
|10204|Purchase Order Receipt|
|10205|Purchase Order Receipt Product|
|10206|Purchase Order SubStatus|
|10207|Quote Booking Incident|
|10208|Quote Booking Product|
|10209|Quote Booking Service|
|10210|Quote Booking Service Task|
|10211|Quote Booking Setup|
|10212|Quote Invoicing Product|
|10213|Quote Invoicing Setup|
|10214|Resource Pay Type|
|10215|RMA|
|10216|RMA Product|
|10217|RMA Receipt|
|10218|RMA Receipt Product|
|10219|RMA SubStatus|
|10220|RTV|
|10221|RTV Product|
|10222|RTV Substatus|
|10223|Service Task Type|
|10224|Ship Via|
|10225|Tax Code|
|10226|Tax Code Detail|
|10227|Time Off Request|
|10228|Unique Number|
|10229|Warehouse|
|10230|Work Order|
|10231|Work Order Characteristic (Deprecated)|
|10232|Work Order Details Generation Queue (Deprecated)|
|10233|Work Order Incident|
|10234|Work Order Product|
|10235|Resource Restriction (Deprecated)|
|10236|Work Order Service|
|10237|Work Order Service Task|
|10238|Work Order Substatus|
|10239|Work Order Type|
|10241|IoT Alert|
|10242|IoT Device|
|10243|IoT Device Category|
|10244|IoT Device Command|
|10245|IoT Device Command Definition|
|10246|IoT Device Data History|
|10247|IoT Device Property|
|10248|IoT Device Registration History|
|10249|IoT Property Definition|
|10250|IoT Settings|
|10253|CFS - IoT Alert Process Flow|
|10254|Entity Configuration|
|10255|Geofence|
|10256|Geofence Event|
|10257|Geofencing Settings|


<a name="onetomany"></a>

## One-To-Many Relationships

Listed by **SchemaName**.

- [TransformationMapping_ImportMap](#BKMK_TransformationMapping_ImportMap)
- [OwnerMapping_ImportMap](#BKMK_OwnerMapping_ImportMap)
- [ImportMap_AsyncOperations](#BKMK_ImportMap_AsyncOperations)
- [ImportMap_ImportFile](#BKMK_ImportMap_ImportFile)
- [ImportMap_BulkDeleteFailures](#BKMK_ImportMap_BulkDeleteFailures)
- [ImportEntityMapping_ImportMap](#BKMK_ImportEntityMapping_ImportMap)
- [ImportMap_SyncErrors](#BKMK_ImportMap_SyncErrors)
- [ColumnMapping_ImportMap](#BKMK_ColumnMapping_ImportMap)


### <a name="BKMK_TransformationMapping_ImportMap"></a> TransformationMapping_ImportMap

Same as transformationmapping entity [TransformationMapping_ImportMap](transformationmapping.md#BKMK_TransformationMapping_ImportMap) Many-To-One relationship.

|Property|Value|
|--------|-----|
|ReferencingEntity|transformationmapping|
|ReferencingAttribute|importmapid|
|IsHierarchical|False|
|IsCustomizable|False|
|ReferencedEntityNavigationPropertyName|TransformationMapping_ImportMap|
|AssociatedMenuConfiguration|Behavior: DoNotDisplay<br />Group: Details<br />Label: <br />Order: |
|CascadeConfiguration|Assign: NoCascade<br />Delete: Cascade<br />Merge: NoCascade<br />Reparent: NoCascade<br />Share: NoCascade<br />Unshare: NoCascade|


### <a name="BKMK_OwnerMapping_ImportMap"></a> OwnerMapping_ImportMap

Same as ownermapping entity [OwnerMapping_ImportMap](ownermapping.md#BKMK_OwnerMapping_ImportMap) Many-To-One relationship.

|Property|Value|
|--------|-----|
|ReferencingEntity|ownermapping|
|ReferencingAttribute|importmapid|
|IsHierarchical|False|
|IsCustomizable|False|
|ReferencedEntityNavigationPropertyName|OwnerMapping_ImportMap|
|AssociatedMenuConfiguration|Behavior: DoNotDisplay<br />Group: Details<br />Label: <br />Order: |
|CascadeConfiguration|Assign: NoCascade<br />Delete: Cascade<br />Merge: NoCascade<br />Reparent: NoCascade<br />Share: NoCascade<br />Unshare: NoCascade|


### <a name="BKMK_ImportMap_AsyncOperations"></a> ImportMap_AsyncOperations

Same as asyncoperation entity [ImportMap_AsyncOperations](asyncoperation.md#BKMK_ImportMap_AsyncOperations) Many-To-One relationship.

|Property|Value|
|--------|-----|
|ReferencingEntity|asyncoperation|
|ReferencingAttribute|regardingobjectid|
|IsHierarchical|False|
|IsCustomizable|False|
|ReferencedEntityNavigationPropertyName|ImportMap_AsyncOperations|
|AssociatedMenuConfiguration|Behavior: DoNotDisplay<br />Group: Details<br />Label: <br />Order: |
|CascadeConfiguration|Assign: NoCascade<br />Delete: NoCascade<br />Merge: NoCascade<br />Reparent: NoCascade<br />Share: NoCascade<br />Unshare: NoCascade|


### <a name="BKMK_ImportMap_ImportFile"></a> ImportMap_ImportFile

Same as importfile entity [ImportMap_ImportFile](importfile.md#BKMK_ImportMap_ImportFile) Many-To-One relationship.

|Property|Value|
|--------|-----|
|ReferencingEntity|importfile|
|ReferencingAttribute|importmapid|
|IsHierarchical|False|
|IsCustomizable|False|
|ReferencedEntityNavigationPropertyName|ImportMap_ImportFile|
|AssociatedMenuConfiguration|Behavior: DoNotDisplay<br />Group: Details<br />Label: <br />Order: |
|CascadeConfiguration|Assign: NoCascade<br />Delete: RemoveLink<br />Merge: NoCascade<br />Reparent: NoCascade<br />Share: NoCascade<br />Unshare: NoCascade|


### <a name="BKMK_ImportMap_BulkDeleteFailures"></a> ImportMap_BulkDeleteFailures

Same as bulkdeletefailure entity [ImportMap_BulkDeleteFailures](bulkdeletefailure.md#BKMK_ImportMap_BulkDeleteFailures) Many-To-One relationship.

|Property|Value|
|--------|-----|
|ReferencingEntity|bulkdeletefailure|
|ReferencingAttribute|regardingobjectid|
|IsHierarchical|False|
|IsCustomizable|False|
|ReferencedEntityNavigationPropertyName|ImportMap_BulkDeleteFailures|
|AssociatedMenuConfiguration|Behavior: DoNotDisplay<br />Group: Details<br />Label: <br />Order: |
|CascadeConfiguration|Assign: NoCascade<br />Delete: Cascade<br />Merge: NoCascade<br />Reparent: NoCascade<br />Share: NoCascade<br />Unshare: NoCascade|


### <a name="BKMK_ImportEntityMapping_ImportMap"></a> ImportEntityMapping_ImportMap

Same as importentitymapping entity [ImportEntityMapping_ImportMap](importentitymapping.md#BKMK_ImportEntityMapping_ImportMap) Many-To-One relationship.

|Property|Value|
|--------|-----|
|ReferencingEntity|importentitymapping|
|ReferencingAttribute|importmapid|
|IsHierarchical|False|
|IsCustomizable|False|
|ReferencedEntityNavigationPropertyName|ImportEntityMapping_ImportMap|
|AssociatedMenuConfiguration|Behavior: DoNotDisplay<br />Group: Details<br />Label: <br />Order: |
|CascadeConfiguration|Assign: NoCascade<br />Delete: Cascade<br />Merge: NoCascade<br />Reparent: NoCascade<br />Share: NoCascade<br />Unshare: NoCascade|


### <a name="BKMK_ImportMap_SyncErrors"></a> ImportMap_SyncErrors

Same as syncerror entity [ImportMap_SyncErrors](syncerror.md#BKMK_ImportMap_SyncErrors) Many-To-One relationship.

|Property|Value|
|--------|-----|
|ReferencingEntity|syncerror|
|ReferencingAttribute|regardingobjectid|
|IsHierarchical|False|
|IsCustomizable|True|
|ReferencedEntityNavigationPropertyName|ImportMap_SyncErrors|
|AssociatedMenuConfiguration|Behavior: DoNotDisplay<br />Group: Details<br />Label: <br />Order: |
|CascadeConfiguration|Assign: Cascade<br />Delete: Cascade<br />Merge: Cascade<br />Reparent: Cascade<br />Share: Cascade<br />Unshare: Cascade|


### <a name="BKMK_ColumnMapping_ImportMap"></a> ColumnMapping_ImportMap

Same as columnmapping entity [ColumnMapping_ImportMap](columnmapping.md#BKMK_ColumnMapping_ImportMap) Many-To-One relationship.

|Property|Value|
|--------|-----|
|ReferencingEntity|columnmapping|
|ReferencingAttribute|importmapid|
|IsHierarchical|False|
|IsCustomizable|False|
|ReferencedEntityNavigationPropertyName|ColumnMapping_ImportMap|
|AssociatedMenuConfiguration|Behavior: DoNotDisplay<br />Group: Details<br />Label: <br />Order: |
|CascadeConfiguration|Assign: NoCascade<br />Delete: Cascade<br />Merge: NoCascade<br />Reparent: NoCascade<br />Share: NoCascade<br />Unshare: NoCascade|

<a name="manytoone"></a>

## Many-To-One Relationships

Each Many-To-One relationship is defined by a corresponding One-To-Many relationship with the related entity. Listed by **SchemaName**.

- [lk_importmapbase_createdby](#BKMK_lk_importmapbase_createdby)
- [lk_importmap_createdonbehalfby](#BKMK_lk_importmap_createdonbehalfby)
- [BusinessUnit_ImportMaps](#BKMK_BusinessUnit_ImportMaps)
- [team_ImportMaps](#BKMK_team_ImportMaps)
- [lk_importmap_modifiedonbehalfby](#BKMK_lk_importmap_modifiedonbehalfby)
- [SystemUser_ImportMaps](#BKMK_SystemUser_ImportMaps)
- [lk_importmapbase_modifiedby](#BKMK_lk_importmapbase_modifiedby)


### <a name="BKMK_lk_importmapbase_createdby"></a> lk_importmapbase_createdby

See systemuser Entity [lk_importmapbase_createdby](systemuser.md#BKMK_lk_importmapbase_createdby) One-To-Many relationship.

### <a name="BKMK_lk_importmap_createdonbehalfby"></a> lk_importmap_createdonbehalfby

See systemuser Entity [lk_importmap_createdonbehalfby](systemuser.md#BKMK_lk_importmap_createdonbehalfby) One-To-Many relationship.

### <a name="BKMK_BusinessUnit_ImportMaps"></a> BusinessUnit_ImportMaps

See businessunit Entity [BusinessUnit_ImportMaps](businessunit.md#BKMK_BusinessUnit_ImportMaps) One-To-Many relationship.

### <a name="BKMK_team_ImportMaps"></a> team_ImportMaps

See team Entity [team_ImportMaps](team.md#BKMK_team_ImportMaps) One-To-Many relationship.

### <a name="BKMK_lk_importmap_modifiedonbehalfby"></a> lk_importmap_modifiedonbehalfby

See systemuser Entity [lk_importmap_modifiedonbehalfby](systemuser.md#BKMK_lk_importmap_modifiedonbehalfby) One-To-Many relationship.

### <a name="BKMK_SystemUser_ImportMaps"></a> SystemUser_ImportMaps

See systemuser Entity [SystemUser_ImportMaps](systemuser.md#BKMK_SystemUser_ImportMaps) One-To-Many relationship.

### <a name="BKMK_lk_importmapbase_modifiedby"></a> lk_importmapbase_modifiedby

See systemuser Entity [lk_importmapbase_modifiedby](systemuser.md#BKMK_lk_importmapbase_modifiedby) One-To-Many relationship.

### See also

[About the Entity Reference](../about-entity-reference.md)<br />
[Programming reference for Dynamics 365 Customer Engagement](../programming-reference.md)<br />
[Web API Reference](/dynamics365/customer-engagement/web-api/about)<br />
<xref href="Microsoft.Dynamics.CRM.importmap?text=importmap EntityType" />

[!INCLUDE[footer-include](../../../../includes/footer-banner.md)]