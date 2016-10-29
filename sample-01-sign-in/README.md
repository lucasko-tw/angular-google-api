### Angular with Google API 

###Update Your Client ID
```HTML
 <meta name="google-signin-client_id" content="{YOUR_CLIENT_ID}">
```

###Auth Code

```HTML
<script>

  var myApp = angular.module('myApp', [  ]);
  myApp.controller('myCtrl', function ($scope) {
  $scope.options = {
            'onsuccess': function(response) {
              console.log(response);
            }
          }
  });

  myApp.directive('googleSignInButton', function () {
  return {
          scope: {
            buttonId: '@',
            options: '&'
          },
          template: '<div></div>',
          link: function(scope, element, attrs) {
            var div = element.find('div')[0];
            div.id = attrs.buttonId;
            gapi.signin2.render(div.id, scope.options());
          }
        };
  });

</script>


```

