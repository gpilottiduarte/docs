# GET | List a remote session by [id]

Access information of a proxy session registered in **PAM Core**.

## Requirements
*  Authorization with **access** permission to **PAM Core** granted by the administrator in **A2A**.
Access the document on [How to create an authorization for an application](/v3-33/docs/a2a-how-to-create-an-authorization-for-an-application) for more information.
* Remote session registered in **PAM Core**. 
Access the document on [How to configure a remote session (proxy)](/v3-33/docs/pam-session-configure-remote-session-proxy) for more information.

## Request
 <code><span style="color:green">GET</code></span> `api/pam/session/remotesessions/[id]`

## Request parameters

Send the parameter below in the <b>path</b> of the URL.

<summary><code>id</code> - <b>int</b> - <span style="color:red">required</span> - Unique hash generated by senhasegura to exclusively identify a specific session.</summary>
<p><b>Note</b>: this value is automatically assigned by senhasegura when the session is created and is obtained in the response to the request <a href="/v3-33/docs/api-get-list-all-remote-sessions">GET | List all remote sessions</a>.</p>

### Example request

<code><span style="color:green">GET</code></span> `{{url}}/api/session/remotesessions/53`

## Response

``` json
HTTP/1.1 200 OK
```

``` json
{
    "code": 200,
    "response": {
        "status": 200,
        "message": "",
        "error": false,
        "error_code": 0,
        "detail": "",
        "mensagem": "",
        "erro": false,
        "cod_erro": 0
    },
    "tenant": "senhasegura",
    "remote_session": [
        {
            "id": "30",
            "user": "MFASenhaSegura",
            "origin_ip": "172.16.20.158",
            "credential": "usrsudonopass",
            "device": "10.66.33.17:22",
            "protocol": "ssh",
            "proxy": "Web Proxy",
            "session_id": "df06257a1*********************9104dc43",
            "start": "2024-05-15 17:37:53",
            "end": "2024-05-15 17:38:00",
            "time": "00:00:07",
            "prevent_purge": "No",
            "request": null,
            "ITSM": null
        }
    ]
}
```


### Response body fields

<summary><code>remote_sessions</code> - <b>array of objects</b> - Data of the listed remote sessions.</summary>

<br>
<summary>&nbsp;&emsp;&emsp;&nbsp;→<code>id</code> - <b><b>int</b></b> - Unique identification code for the remote session.</summary>&nbsp;&emsp;&emsp;&nbsp;<b>Note</b>: this value is automatically assigned by senhasegura when the session is created and should not be confused with the <code>session_id</code> parameter.

<br>
<summary>&nbsp;&emsp;&emsp;&nbsp;→<code>user</code> - <b><b>string</b></b> - Username used for authentication.</summary>

<br>
<summary>&nbsp;&emsp;&emsp;&nbsp;→<code>origin_ip</code> - <b><b>string</b></b> - IP address of the session's originating device.</summary>

<br>
<summary>&nbsp;&emsp;&emsp;&nbsp;→<code>credential</code> - <b>string</b> - Credential used for the session.</summary>

<br>
<summary>&nbsp;&emsp;&emsp;&nbsp;→<code>device</code> - <b>string</b> - Hostname or IP address of the target device.</summary>
  
<br>
<summary>&nbsp;&emsp;&emsp;&nbsp;→<code>protocol</code> - <b>string</b> - Network protocol (SSH, RDP, HTTPS, among others).</summary>

<br>
<summary>&nbsp;&emsp;&emsp;&nbsp;→<code>proxy</code> - <b>string</b> - Type of proxy session.</summary>

<br>
<summary>&nbsp;&emsp;&emsp;&nbsp;→<code>session_id</code> - <b>string</b> - Unique hash generated by senhasegura to exclusively identify a specific session.</summary>&nbsp;&emsp;&emsp;&nbsp;<b>Example</b>: <code>df06257a1*********************9104dc43</code>

&nbsp;&emsp;&emsp;&nbsp;<b>Note</b>: this identifier is used internally by the application for operations related to the session, such as access control, activity tracking, and resource management. Each time a session is started, a new <code>session_id</code> is generated for that specific session.

<br>
<summary>&nbsp;&emsp;&emsp;&nbsp;→<code>start</code> - <b>string</b> - Start date and time of the session in ISO 8601 format.</summary>
&nbsp;&emsp;&emsp;&nbsp;<b>Example</b>: <code>2024-05-06 16:05:07</code></p>

<br>
<summary>&nbsp;&emsp;&emsp;&nbsp;→<code>end</code> - <b>string</b> - End date and time of the session in ISO 8601 format.</summary>
&nbsp;&emsp;&emsp;&nbsp;<b>Example</b>: <code>2024-05-06 16:07:59</code></p>

<br>
<summary>&nbsp;&emsp;&emsp;&nbsp;→<code>time</code> - <b>string</b> - Duration of the session.</summary>
&nbsp;&emsp;&emsp;&nbsp;<b>Example</b>: <code>00:02:52</code></p>

<br>
<summary>&nbsp;&emsp;&emsp;&nbsp;→<code>prevent_purge</code> - <b>string</b> - Indicates whether the session data will be automatically deleted.</summary>
&nbsp;&emsp;&emsp;&nbsp;<b>Example</b>: <code>No</code></p>

<br>
<summary>&nbsp;&emsp;&emsp;&nbsp;→<code>request</code> - <b>string</b> - Request made by the user.</summary>

<br>
<summary>&nbsp;&emsp;&emsp;&nbsp;→<code>ITSM</code> - <b>string</b> - ITSM software code.</summary>


 ## Errors
 
<details>
<summary><b><span style="color:red">404</span> - Not Found</b></summary>

***
<b>Message: "Resource sub not found"</b><br>

<p><b>Possible cause</b>: the URL or the requested resource isn’t correct.<br>
        
<b>Solution</b>: check the URL and make sure the parameter is correct.</p>
* * *
</details>


<details>
 
<summary><b><span style="color:red">500</span> - Internal Server Error</b></summary>

***
    
<b>Message: "Unexpected error."</b><br>
 
<p><b>Possible cause</b>: the error is in the senhasegura server.<br>
        
<b>Solution</b>: contact the support team for more information.</p>

***

<b>Message: "You are not authorized to access this resource."</b>

<p><b>Possible cause</b>: you don’t have the authorization to access this resource.<br>
        
<b>Solution</b>: ask the administrator to check your permission to access the <b>Web Proxy Session</b> resources in <b>A2A</b>.</p>

* * *
 </details>   

  

<details>
<summary><b>Client authentication failed</b></summary>

*** 
   
<b>Message: "Client authentication failed."</b>
<p><b>Possible cause</b>: failure in your application authentication with the senhasegura server. <br>
        
<b>Solution</b>: check the authentication parameters such as <code>Access Token URL</code>, <code>Client ID</code> e <code>Client secret</code> and request a new access token.</p>
 
* * *   
</details>
     
  

<details>
<summary><b>Invalid signature</b></summary>

*** 
    
<b>Message: "Invalid signature"</b>
    
<p><b>Possible cause</b>: failure in recognizing the URL of the client application.
        
<b>Solution</b>: check the URL of the client application and resent the request.</p>

* * * 
</details>
     

<details>
    <summary><b>No route matched with those values</b></summary>
    
***   
    
<b>Message: "No route matched with those values."</b>
   <p><b>Possible cause</b>: the authorization header is missing in the API request.<br>
        
  <b>Solution</b>: request a new access token.</p>
   
 * * *
</details>
 

<details>
    <summary><b> Request timed out</b></summary>
    
***
    
<b>Message: "Request timed out."</b>
<p><b>Possible cause</b>: the request time has expired.<br>
        
<b>Solution</b>: check the connectivity between the source of the request and the senhasegura server.</p>
</details>