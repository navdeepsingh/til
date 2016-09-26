# App Access Token for accessing public photos

Recently, I got work assigned to fetch recent 20 uploaded photos in Facebook Fan Page and then populate in DOM via jQuery. One thing I knew before giving estimate to this work that we need a user token to call FB API. As there is no FB Login to get user token, so I found that I can use App Access token to call FB API. Then I used hardcoded app access token to fetch all photos, and I dont feel any problem to use that as photos too public and there is nothing suspicious in Test app created at developers.facebook.com


Reference : https://developers.facebook.com/docs/facebook-login/access-tokens#apptokens

``` javascript
FB.api('/{app_id}/photos?type=uploaded&limit=20&fields=images',
        'get',
        {access_token : {app_id|app_secret},
        function(response) {
          // Process response
        });
      );
```
