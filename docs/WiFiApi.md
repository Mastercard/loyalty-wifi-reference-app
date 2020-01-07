# WiFiApi

All URIs are relative to *https://api.mastercard.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**loyaltyWifiHotspotsGet**](WiFiApi.md#loyaltyWifiHotspotsGet) | **GET** /loyalty/wifi/hotspots | Find Wi-Fi hotspots nearby


<a name="loyaltyWifiHotspotsGet"></a>
# **loyaltyWifiHotspotsGet**
> List&lt;Hotspot&gt; loyaltyWifiHotspotsGet(latitude, longitude, radius)

Find Wi-Fi hotspots nearby

### Example
```java
// Import classes:
//import com.mastercard.developer.loyalty_wifi_client.ApiException;
//import com.mastercard.developer.loyalty_wifi_client.api.WiFiApi;


WiFiApi apiInstance = new WiFiApi();
String latitude = 77.11112223331; // String | Geographical coordinate of a place to find nearby hotspots
String longitude = 149.99999999; // String | Geographical coordinate of a place to find nearby hotspots
Integer radius = 200; // Integer | Search radius in meters.  Defaults to 500.
try {
    List<Hotspot> result = apiInstance.loyaltyWifiHotspotsGet(latitude, longitude, radius);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling WiFiApi#loyaltyWifiHotspotsGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **latitude** | **String**| Geographical coordinate of a place to find nearby hotspots |
 **longitude** | **String**| Geographical coordinate of a place to find nearby hotspots |
 **radius** | **Integer**| Search radius in meters.  Defaults to 500. | [optional]

### Return type

[**List&lt;Hotspot&gt;**](Hotspot.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

