# drachtio-basic-registrar

A SIP registrar built using [drachtio](https://drachtio.org) and [rtpengine](https://github.com/sipwise/rtpengine).

Features:

- supports nat'ed sip clients
- supports webrtc clients
- connectable to your SIP trunking provider

## Installing

- install [drachtio](https://drachtio.org), [rtpengine](https://github.com/sipwise/rtpengine) and [redis](https://redis.io) somewhere in your network (drachtio and rtpengine must have public IP addresses),
- create a config file (see [config/default.json](config/default.json) for example settings),
- add your sip user credentials to the config file,
- add your SIP trunking provider details (If you have one) to the config file, then
```bash
$ npm install
$ npm start
```
Then point your sip phones and webrtc clients to the server and enjoy!

## Testing
```
npm test
```
