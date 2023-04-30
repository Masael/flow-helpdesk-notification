# Flow Documentation \- HelpDesk Notification

| Flow Name                  | HelpDesk Notification                    |
| -------------------------- | ---------------------------------------- |
| Flow Name                  | HelpDesk Notification                    |
| Flow ID                    | 2065bf13\-a469\-4136\-81c7\-521573b72639 |
| Documentation generated at | domingo, 30 de abril de 2023 02:45 p. m. |
| Number of Variables        | 0                                        |
| Number of Actions          | 6                                        |

- [Overview](../index-HelpDesk-Notification(2065bf13-a469-4136-81c7-521573b72639).md)
- [Connection References](../connections-HelpDesk-Notification(2065bf13-a469-4136-81c7-521573b72639).md)
- [Variables](../variables-HelpDesk-Notification(2065bf13-a469-4136-81c7-521573b72639).md)
- [Triggers & Actions](../triggersactions-HelpDesk-Notification(2065bf13-a469-4136-81c7-521573b72639).md)

## Obtener\_Registo\_de\_lista\_HelpDesk\_Tickets

| Property   | Value                                                                                                               |
| ---------- | ------------------------------------------------------------------------------------------------------------------- |
| Name       | Obtener\_Registo\_de\_lista\_HelpDesk\_Tickets                                                                      |
| Type       | OpenApiConnection                                                                                                   |
| Connection | [![sharepointonline](../sharepointonline32.png) SharePoint](https://docs.microsoft.com/connectors/sharepointonline) |

### Inputs

| Property       | Value                                                                                                                                                                                                                            |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| metadata       | <table><tr><td>operationMetadataId</td><td>ad56ce5a-23f8-4f99-8209-c638b563f32c</td></tr></table>                                                                                                                                |
| host           | <table><tr><td>apiId</td><td>/providers/Microsoft.PowerApps/apis/shared_sharepointonline</td></tr><tr><td>connectionName</td><td>shared_sharepointonline</td></tr><tr><td>operationId</td><td>GetItem</td></tr></table>          |
| parameters     | <table><tr><td>dataset</td><td>https://canopiacarbon918.sharepoint.com/sites/intranet</td></tr><tr><td>table</td><td>1e1e4d5d-9fd8-4769-803b-b826234e2eda</td></tr><tr><td>id</td><td>@triggerBody()['number']</td></tr></table> |
| authentication | <table><tr><td>value</td><td>@json(decodeBase64(triggerOutputs().headers['X-MS-APIM-Tokens']))['$ConnectionKey']</td></tr><tr><td>type</td><td>Raw</td></tr></table>                                                             |

### Next Action(s) Conditions

| Next Action                                                                                                                            |
| -------------------------------------------------------------------------------------------------------------------------------------- |
| [Switch\_Estados\_de\_Tickets \[Succeeded\]](Switch_Estados_de_Tickets-HelpDesk-Notification(2065bf13-a469-4136-81c7-521573b72639).md) |
