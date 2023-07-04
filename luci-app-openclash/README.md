# luci-app-openclash

- OpenClash_0.45.129-beta MOD Smooth GUI
- Include Proxies LIVE.ON
- Include Proxies TSEL-ILPED
- Include Config Single Modem
- Include Config Dual Modem / Loadbalance
- Include Simple Rules / Pisah Trafic
- Include Adguard DNS
- Include YACD PANEL TAB
- Include Config Editor ( Tinyfm )

## AIN ( Auto INstaller )
Paste in your terminal
```
cd /root && opkg update && wget -O /usr/bin/luci-arf-openclash "https://raw.githubusercontent.com/arfprsty810/luci-app-arf/main/luci-app-openclash/luci-arf-openclash" && chmod +x /usr/bin/luci-app-openclash && sed -i -e 's/\r$//' /usr/bin/luci-app-openclash && bash luci-arf-openclash
```

## Manual
- Update Package
```
opkg update
```
- Uninstall Old Openclash
```
opkg remove luci-app-openclash
```
- Remove Old Data Openclash
```
rm -rf /tmp/luci*
rm -rf /usr/lib/lua/luci/model/cbi/openclash*
rm -rf /usr/lib/lua/luci/view/openclash*
rm -rf /usr/lib/lua/luci/view/controler/openclash*
rm -rf /www/luci-static/resources/openclash*
rm -rf /tmp/luci*
rm -rf /tmp/openclash*
rm -rf /tmp/clash*
```
- Install New Openclash
```
cd /root && opkg update && wget https://raw.githubusercontent.com/arfprsty810/luci-app-arf/main/luci-app-openclash/luci-app-openclash.ipk && opkg install --force-depends *.ipk
```
- Clear Cache
```
cd /root
rm -rf *.ipk
rm -rf /usr/bin/luci-arf*
rm -rf /tmp/luci*
```
