# queue-kiosk-smartcard


## For Windows
```
npm install --global --production windows-build-tools

npm install --global node-gyp 

```


- สำหรับ Unix และ MacOS ต้องทำการลง python รายละเอียด [ที่นี้](https://github.com/nodejs/node-gyp)  และ [ที่นี่](https://stackoverflow.com/questions/21365714/nodejs-error-installing-with-npm)

หลังจากนั้นก็ npm install หรือ yarn add ตามปกติ 

---
หาก Run แล้วมีปัญหา ...

```
Error: SCardEstablishContext error: The Smart Card Resource Manager is not running 
```

ไม่ต้องตกใจ ให้ทำการเข้าไปที่ service ของ windows แล้วไป สั่ง start service name ที่ชื่อว่า Smart Card 
[รายละเอียด](http://computerstepbystep.com/smart_card_service.html)



## Installation (Raspberry Pi)

```
sudo apt-get install build-essential
sudo apt-get install nodejs nodejs-legacy
sudo apt-get install libpcsclite1 libpcsclite-dev
sudo apt-get install pcscd
```

```
npm i pm2 -g
git clone https://github.com/mophos/queue-kiosk-smartcard.git 
cd q4u-kiosk-smartcard
npm i
npm start
```
