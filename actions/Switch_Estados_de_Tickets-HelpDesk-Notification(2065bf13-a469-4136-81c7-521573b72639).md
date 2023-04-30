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

## Switch\_Estados\_de\_Tickets

| Property   | Value                                                                         |
| ---------- | ----------------------------------------------------------------------------- |
| Name       | Switch\_Estados\_de\_Tickets                                                  |
| Type       | Switch                                                                        |
| Expression | @outputs('Obtener_Registo_de_lista_HelpDesk_Tickets')?['body/Estadodeticket'] |

### Inputs

| Property | Value                                                                                             |
| -------- | ------------------------------------------------------------------------------------------------- |
| metadata | <table><tr><td>operationMetadataId</td><td>a79a696c-2b20-4fc3-a113-025d965cb14d</td></tr></table> |

### Switch Actions

| Case Values | Action                                                                                                                                                                                    |
| ----------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Abierto     | [Correo\_a\_Usuario\_cuando\_se\_actualiza\_Ticket](Correo_a_Usuario_cuando_se_actualiza_Ticket-HelpDesk-Notification(2065bf13-a469-4136-81c7-521573b72639).md)                           |
| Cerrado     | [Enviar\_correo\_electrónico\_(V2)](Enviar_correo_electronico_(V2)-HelpDesk-Notification(2065bf13-a469-4136-81c7-521573b72639).md)                                                        |
| default     | [Obtener\_Correos\_Administradores\_de\_lista\_HelpDesk\_Config](Obtener_Correos_Administradores_de_lista_HelpDesk_Config-HelpDesk-Notification(2065bf13-a469-4136-81c7-521573b72639).md) |
| default     | [Correo\_Administradores\_lista\_HelpDesk\_Config](Correo_Administradores_lista_HelpDesk_Config-HelpDesk-Notification(2065bf13-a469-4136-81c7-521573b72639).md)                           |
