#!name=Locket Gold 
#!desc=By: quangdbrr
[Script]
revenuecat = type=http-response, pattern=^https:\/\/api\.revenuecat\.com\/.+\/(receipts$|subscribers\/[^/]+$), script-path=https://raw.githubusercontent.com/Nhatquang0712207/13022008/refs/heads/Module/Locket_Gold.js, requires-body=true, max-size=-1, timeout=60
deleteHeader = type=http-request, pattern=^https:\/\/api\.revenuecat\.com\/.+\/(receipts|subscribers), script-path= timeout=60
[MITM]
hostname = %APPEND% api.revenuecat.com
