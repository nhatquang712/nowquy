#!name=Locket Gold 
#!desc=By: quangdbrr
[Script]
revenuecat = type=http-response, pattern=^https:\/\/api\.revenuecat\.com\/.+\/(receipts$|subscribers\/[^/]+$), script-path=requires-body=true, max-size=-1, timeout=60
deleteHeader = type=http-request, pattern=^https:\/\/api\.revenuecat\.com\/.+\/(receipts|subscribers), script-path= timeout=60
[MITM]
hostname = %APPEND% api.revenuecat.com
