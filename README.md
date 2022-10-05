./rploader.sh update now
./rploader.sh fullupgrade now
./rploader.sh serialgen DS3622xs+

./rploader.sh ext broadwellnk-7.0.1-42218 add https://raw.githubusercontent.com/pocopico/rp-ext/master/arcmsr/rpext-index.json

./rploader.sh identifyusb now
 XXXXX ./rploader.sh satamap now 

"SataPortMap": "4"    "9"
"DiskIdxMap": "00"    "0"
"netif_num": "1",

./rploader.sh ext broadwellnk-7.0.1-42218 add https://raw.githubusercontent.com/pocopico/rp-ext/master/r8101/rpext-index.json

./rploader.sh ext broadwellnk-7.0.1-42218 add https://raw.githubusercontent.com/pocopico/rp-ext/master/r8125/rpext-index.json

./rploader.sh ext broadwellnk-7.0.1-42218 add https://raw.githubusercontent.com/pocopico/rp-ext/master/r8152/rpext-index.json

./rploader.sh ext broadwellnk-7.0.1-42218 add https://raw.githubusercontent.com/pocopico/rp-ext/master/r8168/rpext-index.json

./rploader.sh ext broadwellnk-7.0.1-42218 add https://raw.githubusercontent.com/pocopico/rp-ext/master/r8169/rpext-index.json

./rploader.sh ext broadwellnk-7.0.1-42218 add https://raw.githubusercontent.com/pocopico/rp-ext/master/igp/rpext-index.json

./rploader.sh ext broadwellnk-7.0.1-42218 add https://raw.githubusercontent.com/pocopico/rp-ext/master/e1000/rpext-index.json

./rploader.sh ext broadwellnk-7.0.1-42218 add https://raw.githubusercontent.com/pocopico/rp-ext/master/e1000e/rpext-index.json

./rploader.sh ext broadwellnk-7.0.1-42218 add https://raw.githubusercontent.com/pocopico/rp-ext/master/mpt3sas/rpext-index.json

./rploader.sh build broadwellnk-7.1.0-42661

exec sudo reboot

./rploader.sh clean now
./rploader.sh build broadwellnk-7.1.0-42661

./rploader.sh clean now; rm -rf /mnt/sdb3/auxfiles; rm -rf /home/tc/custom-module; ./rploader.sh backup now;

exec sudo reboot
