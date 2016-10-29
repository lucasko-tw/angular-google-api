### Angular with Google API 

###Call GAPI Function 

```HTML
 gapi.client.load('gmail', 'v1', listLabels);
```

###The Request of Gmail Message API

```HTML
        var request = gapi.client.gmail.users.messages.list({
          'userId': 'me'
        });
```





