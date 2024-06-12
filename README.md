```
http://localhost:3000/?state=state-token&code=xxxxx&scope=https://www.googleapis.com/auth/calendar.readonly
```


## approval forceだけ

`https://accounts.google.com/o/oauth2/auth?client_id=123702532043-1ie057kp9320u4igjj2pfvs09v4h24qq.apps.googleusercontent.com&prompt=consent&redirect_uri=http%3A%2F%2Flocalhost%3A3000&response_type=code&scope=https%3A%2F%2Fwww.googleapis.com%2Fauth%2Fcalendar.readonly&state=state-token1`

prompt=consentが入る

## `oauth2.AccessTypeOffline`だけ

`https://accounts.google.com/o/oauth2/auth?access_type=offline&client_id=123702532043-1ie057kp9320u4igjj2pfvs09v4h24qq.apps.googleusercontent.com&redirect_uri=http%3A%2F%2Flocalhost%3A3000&response_type=code&scope=https%3A%2F%2Fwww.googleapis.com%2Fauth%2Fcalendar.readonly&state=state-token`

access_type=offlineが入る

## 混ぜたとき

`https://accounts.google.com/o/oauth2/auth?access_type=offline&client_id=123702532043-1ie057kp9320u4igjj2pfvs09v4h24qq.apps.googleusercontent.com&prompt=consent&redirect_uri=http%3A%2F%2Flocalhost%3A3000&response_type=code&scope=https%3A%2F%2Fwww.googleapis.com%2Fauth%2Fcalendar.readonly&state=state-token1`

access_type=offlineとprompt=consentが入る.
