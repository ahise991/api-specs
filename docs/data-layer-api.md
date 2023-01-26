# Data Layer API Reference

The [Data Layer API](/api-docs/store-management/data-layer-api) is a GraphQL management API that allows you to enable and disable the [Big Open Data Layer](/api-docs/analytics/bodl-for-storefronts) for a store.

Request URL: `https://api.bigcommerce.com/stores/{store_hash}/v3/...`

## OAuth Scopes

| UI Name | Permission | Parameter |
| :--- | :--- | :--- |
|  | modify |  |
|  | read-only |  |


## Schema Types

### Query
<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>store</strong></td>
<td valign="top"><a href="#store">Store</a>!</td>
<td>

A store.

</td>
</tr>
</tbody>
</table>

### Mutation
<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>settings</strong></td>
<td valign="top"><a href="#storesettingsmutation">StoreSettingsMutation</a></td>
<td>

Store settings

</td>
</tr>
</tbody>
</table>

### Objects

#### DataSolutionsMutations

Data solutions mutations.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>updateDataLayer</strong></td>
<td valign="top"><a href="#updatedatalayerresult">UpdateDataLayerResult</a></td>
<td>

Update data layer config.

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="#updatedatalayerinput">UpdateDataLayerInput</a>!</td>
<td></td>
</tr>
</tbody>
</table>

#### DataSolutionsSettings

Data solutions settings.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>isDataLayerEnabled</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

Indicates if a data layer(bodl) object is enabled for all storefronts.

</td>
</tr>
</tbody>
</table>

#### Store

A store.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>settings</strong></td>
<td valign="top"><a href="#storesettings">StoreSettings</a></td>
<td>

Store settings.

</td>
</tr>
</tbody>
</table>

#### StoreSettings

Store settings.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>dataSolutions</strong></td>
<td valign="top"><a href="#datasolutionssettings">DataSolutionsSettings</a></td>
<td>

Store settings.

</td>
</tr>
</tbody>
</table>

#### StoreSettingsMutation

Store Settings mutations

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>dataSolution</strong></td>
<td valign="top"><a href="#datasolutionsmutations">DataSolutionsMutations</a></td>
<td>

Store settings.

</td>
</tr>
</tbody>
</table>

#### UpdateDataLayerResult

Result of mutation.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>dataSolutions</strong></td>
<td valign="top"><a href="#datasolutionssettings">DataSolutionsSettings</a></td>
<td>

Data solutions that is updated as a result of mutation.

</td>
</tr>
</tbody>
</table>

### Inputs

#### UpdateDataLayerInput

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>isDataLayerEnabled</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td>

is data layer enabled

</td>
</tr>
</tbody>
</table>

### Scalars

#### Boolean

The `Boolean` scalar type represents `true` or `false`.

#### String

The `String` scalar type represents textual data, represented as UTF-8 character sequences. The String type is most often used by GraphQL to represent free-form human-readable text.

