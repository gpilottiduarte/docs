# Reference for Application settings

In this document, you will find all the information about the **Activation** menu of the **Orbit Web** interface.

## Access Path
1. In senhasegura, at the top left corner, click on the **Grid Menu**, represented by the nine squares, and select **Orbit Config Manager**.
2. In the side menu, select **Settings > Application**.

### Application Settings
| Item                  | Description                                                                                                                                   |
|-----------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
| **Enable Application** | An instance can be *Activated* or *Deactivated*. The *Activated* status indicates that this instance can be accessed by users in all functionalities. When *Deactivated*, only administrators can log in and will be limited to using only the Orbit web interface. |
| **Enable Robots**          | Determines whether the instance will run asynchronous tasks or not.                                                                              |
| **Restart process every minute** | Indicates if asynchronous services should be restarted every minute during idle periods.                                                    |
| **Company Name**           | The company name                                                                                                                                                 |
| **Application title**      | This title will be displayed as page titles and can be customized by the client.                                                               |
| **Application URL**        | URL to be used in the configuration of other senhasegura services for communication.                                                         |
| **Virtual IP Address**       | Allows access to a Virtual IP Load Balancer (VIP).                                                                                              |
| **Clear all aache**       | This button allows clearing the caches generated by senhasegura.                                                                                 |
| **Notification e-mail**     | List of emails that will receive incident notifications issued by Orbit.                                                                       |

### Zabbix Configuration
| Item                 | Description                                                    |
|----------------------|----------------------------------------------------------------|
| **Use TLS**          | Choose whether to use TLS protocol or not.                     |
| **Server IP 1**      | Destination server data.                                       |
| **Server Port 1** | Destination server data.                                       |
| **Server IP 2**      | Destination server data.                                       |
| **Server IP 3**      | Destination server data.                                       |
| **Server Port 3** | Destination server data.                                       |
| **Listen IP**        | Instance access interface IP.                                  |
| **Listen port**      | Instance access interface port.                                |

### Syslog Configuration
| Item                      | Description                                                  |
|---------------------------|--------------------------------------------------------------|
| **Message format**        | Refers to the selected message format to be sent, which can be CEF, Syslog (RFC 5424), or Sensage. |
| **Notification plugin**   | Used only in cases of paid customization projects. Keep this field with its default value. It is not recommended to manipulate this control without the supervision of the support team. |
| **Message sending protocol** | Choose between TCP or UDP.                                    |
| **Network Connector**     | Refers to the network connector to send the message.         |
| **Use Network Connector?** | Indicates whether the selected network connector will be used in the Syslog message sending configuration. |
| **Servers for message sending** | A list of IPv4 servers, separated by commas, that will receive the messages. |
| **Save**                  | Button to save the configurations.                           |