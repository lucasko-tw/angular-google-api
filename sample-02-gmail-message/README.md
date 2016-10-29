### Angular with Google API 

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





