
# Seven-Lives




## **Root Projects**




### **Interesting Curl Requests on Public API's**



**1) Hotstar seachbar suggestion :** 
  
curl "https://api.hotstar.com/s/v1/scout?q=A&perPage=10" -H "x-country-code: IN" -H "x-client-code: LR"  -H "x-platform-code: PCTV"  -v

parameters : perPage = 0-100? , q = [Search String]

**Result**
{"body":{"results":{"items":[{"title":"NewsState MP CG","contentId":1260012060,"uri":"https://api.hotstar.com/o/v1/content/detail?id=610688&contentId=1260012060&offset=0&size=20&tao=0&tas=5","id":610688,"description":"News State Madhya Pradesh/ Chhattisgarh gives in-depth coverage of Madhya Pradesh & Chhattisgarh, giving local and topical News relevant to MP & CG and has been the content leader since its launch in March 2018.","duration":0,"entityType":"CLIP","contentType":"SHOW_LIVE","contentProvider":"NewsState MP CG","cpDisplayName":"NewsState MP CG","cpLogoUrl":"https://secure-media.hotstar.com/static/NewsV2/PartnerLogos/NewsStateMPCG.png","assetType":"VIDEO","genre":["News"],"lang":["Hindi"],"premium":false,"live":true,"hboContent":false,"vip":false,"encrypted":false,"startDate":1570455513,"endDate":1619803800,"playbackUri":"https://api.hotstar.com/h/v1/play?contentId=1260012060","images":{"v":"sources/r1/cms/prod/259/590259-v","h":"sources/r1/cms/prod/538/570538-h"},"imageSets":{"DEFAULT":{"v":"sources/r1/cms/prod/259/590259-v","h":"sources/r1/cms/prod/538/570538-h"}},"contentDownloadable":false,"playbackType":"INTERNAL","monetisable":true,"langObjs":[{"id":9,"name":"Hindi","iso3code":"hin","detailUrl":"https://api.hotstar.com/o/v1/language/detail?id=9&offset=0&size=20","displayName":"αñ╣αñ┐αñéαñªαÑÇ"}],"genreObjs":[{"id":48,"name":"News","detailUrl":"https://api.hotstar.com/o/v1/genre/detail?id=48&offset=0&size=20"}],"languageSelector":1,"drmClass":"BEST_EFFORT","downloadDrmClass":"BEST_EFFORT","contentStartPointSeconds":0,"badges":["NP"],"labels":["LIVE"],"clipType":"VOD","parentalRating":1,"parentalRatingName":"G","crisp":"Suitable for all","detail":"Suitable for all","isSocialEnabled":false,"orientation":"HORIZONTAL"},{"title":"NewsState UP UK"....},{..},{..},...



**2)Hotstar Login OTP sender : **

curl "https://api.hotstar.com/in/aadhar/v2/web/in/user/register" -H "User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.113 Safari/537.36" -H "Content-Type: application/json" --data-binary "{\"userData\":{\"username\":\"6366031315\",\"usertype\":\"phone\",\"deviceId\":\"2df3bf63-3f94-4782-8135-4bc13bb45f51\"},\"activation\":{\"mode\":\"otp\"}}"

parameters : username = [Enter Mobile Number to send OTP] 


**Result**
{"description":{"phone":"******1315"},"message":"User verification initiated","appCode":"UMSP_700"}




**2)Hotstar Login OTP sender : **
