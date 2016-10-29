### Angular with Google API 


###Update Your Client ID
```HTML
 <meta name="google-signin-client_id" content="{YOUR_CLIENT_ID}">
```

###Call GAPI Function 

```JAVASCRIPT
 gapi.client.load('gmail', 'v1', listLabels);
```

###The Request of Gmail Message API

```JAVASCRIPT
 var request = gapi.client.gmail.users.messages.list({
 'userId': 'me'
 });
```





