# Fewer default fields for faster performace

I got surprised when i tried to get Albmum photos with FB.api but didn't get all fields in response. As i googled, I found The Graph API v2.4 reduces the number of fields in default responses.

Reference : https://developers.facebook.com/blog/post/2015/07/08/graph-api-v2.4/

```
Fewer default fields for faster performance: To help improve performance on mobile network connections, we've reduced the number of fields that the API returns by default. You should now use the ?fields=field1,field2 syntax to declare all the fields you want the API to return.
```
