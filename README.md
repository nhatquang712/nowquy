#!name=Locket Gold 
#!desc=By: Nobita (MOD CSA4G)

[Script]
revenuecat = type=http-response, pattern=^https:\/\/api\.revenuecat\.com\/.+\/(receipts$|subscribers\/[^/]+$), script-path=https://raw.githubusercontent.com/DungHoang120401/Nobita/refs/heads/Module/Locket_Gold.js, requires-body=true, max-size=-1, timeout=60

deleteHeader = type=http-request, pattern=^https:\/\/api\.revenuecat\.com\/.+\/(receipts|subscribers), script-path=https://raw.githubusercontent.com/DungHoang120401/Nobita/refs/heads/Module/LKG_delete_header.js, timeout=60

[MITM]
hostname = %APPEND% api.revenuecat.com
