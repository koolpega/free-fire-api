# 📝 Documentación de la API

## API de Información del Jugador
Ruta de la API = https://free-fire-data.vercel.app/api/data?region={region}&uid={uid}&key={key}

**Endpoint:** `api/data`  
**Clave:** `TU-CLAVE`  
**Método:** `GET`  

Este endpoint recupera información del jugador basada en la región y el ID de usuario especificados.

### 📨 Ejemplo de Solicitud
```http
GET https://free-fire-data.vercel.app/api/data?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parámetros de Consulta

| Parámetro | Tipo   | Requerido | Descripción                           |
|-----------|--------|-----------|---------------------------------------|
| `region`  | string | Sí        | El código de la región (`sg`, `ind`, `br`) |
| `uid`     | int    | Sí        | El ID del usuario                     |
| `key`     | string | Sí        | Compra la clave en https://t.me/TrueClasher4 |

### ℹ️ Nota Importante

El parámetro de consulta `SG` es para todas las regiones que están bajo `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

El parámetro de consulta `IND` es solo para India y está bajo `client.ind.freefiremobile.com`  
[`IND`]

El parámetro de consulta `BR` es para todas las regiones que están bajo `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Ejemplo de una Respuesta Exitosa Puede Ser Así,
```json
{
  "basicInfo": {
    "accountId": 2129250963,
    "accountType": 1,
    "bannerId": 901026021,
    "bpStatus": null,
    "brMaxRank": 316,
    "brRank": 2768,
    "createAt": 1747304828,
    "csMaxRank": 316,
    "csRank": 45,
    "exp": 133627,
    "headPic": 902000057,
    "lastLoginAt": 1593158767,
    "level": 42,
    "liked": 4957,
    "nickname": "SOUNAVA 500K",
    "region": "IND",
    "releaseVersion": "OB48",
    "showBrRank": true,
    "showCsRank": true,
    "title": 904090024
  },
  "captainBasicInfo": {
    "accountId": 2129250963,
    "accountType": 1,
    "badgeCnt": 42,
    "bannerId": 901026021,
    "brMaxRank": 316,
    "brRank": 316,
    "brRankingPoints": 2768,
    "createAt": 1593158767,
    "csMaxRank": 305,
    "csRank": 305,
    "csRankingPoints": 17,
    "exp": 133627,
    "headPic": 902000057,
    "lastLoginAt": 1747304828,
    "level": 42,
    "liked": 4957,
    "nickname": "SOUNAVA 500K",
    "region": "IND",
    "releaseVersion": "OB48",
    "seasonId": 45
  },
  "clanBasicInfo": [
    {
      "capacity": 25,
      "captainId": 2129250963,
      "clanId": 3000167557,
      "clanLevel": 1,
      "clanName": "〆ᗷᖇᝪᎢᕼᗴᖇ",
      "memberNum": 5
    }
  ],
  "creditScoreInfo": {
    "creditScore": 100,
    "periodicSummaryEndTime": 1747564036,
    "periodicSummaryStartTime": 1747304836,
    "rewardState": 2
  },
  "petInfo": {
    "exp": 548,
    "id": 1300000120,
    "level": 4,
    "nickname": null,
    "selectedSkillId": 1310000201,
    "skinId": 1315000010
  },
  "socialInfo": {
    "accountId": 2129250963,
    "brRankShow": 1,
    "csRankShow": null,
    "signature": "Sounava777 Never Dies."
  }
}
```

## API de Estadísticas del Jugador
Ruta de la API = https://free-fire-data.vercel.app/api/stats?region={region}&uid={uid}&key={key}

**Endpoint:** `api/stats`  
**Clave:** `TU-CLAVE`  
**Método:** `GET`  

Este endpoint recupera información de estadísticas del jugador basada en la región y el ID de usuario especificados.

### 📨 Ejemplo de Solicitud
```http
GET https://free-fire-data.vercel.app/api/stats?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parámetros de Consulta

| Parámetro | Tipo   | Requerido | Descripción                           |
|-----------|--------|-----------|---------------------------------------|
| `region`  | string | Sí        | El código de la región (`sg`, `ind`, `br`) |
| `uid`     | int    | Sí        | El ID del usuario                     |
| `key`     | string | Sí        | Compra la clave en https://t.me/TrueClasher4 |

### ℹ️ Nota Importante

El parámetro de consulta `SG` es para todas las regiones que están bajo `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

El parámetro de consulta `IND` es solo para India y está bajo `client.ind.freefiremobile.com`  
[`IND`]

El parámetro de consulta `BR` es para todas las regiones que están bajo `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Ejemplo de una Respuesta Exitosa Puede Ser Así,
```json
{
  "success": true,
  "soloStats": {
    "accountId": "10000001",
    "gamesPlayed": 2,
    "kills": 7,
    "detailedStats": {
      "deaths": 2,
      "distanceTravelled": 5309,
      "survivalTime": 587,
      "highestKills": 4,
      "damage": 1764,
      "headshots": 1,
      "headshotKills": 1,
      "pickUps": 146
    }
  },
  "duoStats": {
    "accountId": "10000001",
    "detailedStats": {

    }
  },
  "quadStats": {
    "accountId": "10000001",
    "gamesPlayed": 13,
    "wins": 3,
    "kills": 36,
    "detailedStats": {
      "deaths": 10,
      "topNTimes": 6,
      "distanceTravelled": 60689,
      "survivalTime": 9210,
      "revives": 4,
      "highestKills": 6,
      "damage": 17872,
      "headshots": 16,
      "headshotKills": 5,
      "knockDown": 42,
      "pickUps": 1536
    }
  }
}
```

## API de Me Gusta
Ruta de la API = https://free-fire-data.vercel.app/api/like?region={region}&uid={uid}&key={key}

**Endpoint:** `api/like`  
**Clave:** `TU-CLAVE`  
**Método:** `GET`  

Este endpoint envía 100 me gusta a la cuenta del jugador basada en la región y el ID de usuario especificados.

### 📨 Ejemplo de Solicitud
```http
GET https://free-fire-data.vercel.app/api/like?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parámetros de Consulta

| Parámetro | Tipo   | Requerido | Descripción                           |
|-----------|--------|-----------|---------------------------------------|
| `region`  | string | Sí        | El código de la región (`sg`, `ind`, `br`) |
| `uid`     | int    | Sí        | El ID del usuario                     |
| `key`     | string | Sí        | Compra la clave en https://t.me/TrueClasher4 |

### ℹ️ Nota Importante

El parámetro de consulta `SG` es para todas las regiones que están bajo `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

El parámetro de consulta `IND` es solo para India y está bajo `client.ind.freefiremobile.com`  
[`IND`]

El parámetro de consulta `BR` es para todas las regiones que están bajo `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Ejemplo de una Respuesta Exitosa Puede Ser Así,
```json
{
  "response": {
    "KeyExpiresAt": "2025-03-20T90:30:00.696969",
    "KeyRemainingRequests": "69/100",
    "LikesGivenByAPI": 100,
    "LikesafterCommand": 6969,
    "LikesbeforeCommand": 6869,
    "PlayerLevel": 69,
    "PlayerNickname": "SOUNAVA 500K",
    "UID": "2129250963"
  },
  "status": 1
}
```

## API de Visitas
Ruta de la API = https://free-fire-data.vercel.app/api/visit?region={region}&uid={uid}&key={key}

**Endpoint:** `api/visit`  
**Clave:** `TU-CLAVE`  
**Método:** `GET`  

Este endpoint envía 100 visitas a la cuenta del jugador basada en la región y el ID de usuario especificados.

### 📨 Ejemplo de Solicitud
```http
GET https://free-fire-data.vercel.app/api/visit?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parámetros de Consulta

| Parámetro | Tipo   | Requerido | Descripción                           |
|-----------|--------|-----------|---------------------------------------|
| `region`  | string | Sí        | El código de la región (`sg`, `ind`, `br`) |
| `uid`     | int    | Sí        | El ID del usuario                     |
| `key`     | string | Sí        | Compra la clave en https://t.me/TrueClasher4 |

### ℹ️ Nota Importante

El parámetro de consulta `SG` es para todas las regiones que están bajo `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

El parámetro de consulta `IND` es solo para India y está bajo `client.ind.freefiremobile.com`  
[`IND`]

El parámetro de consulta `BR` es para todas las regiones que están bajo `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Ejemplo de una Respuesta Exitosa Puede Ser Así,
```json
{
  "response": {
    "KeyExpiresAt": "2025-03-20T90:30:00.696969",
    "KeyRemainingRequests": "69/100",
    "VisitsSentByAPI": 100,
    "PlayerLevel": 69,
    "PlayerNickname": "SOUNAVA 500K",
    "UID": "2129250963"
  },
  "status": 1
}
```

## API de Spam
Ruta de la API = https://free-fire-data.vercel.app/api/spam?region={region}&uid={uid}&key={key}

**Endpoint:** `api/spam`  
**Clave:** `TU-CLAVE`  
**Método:** `GET`  

Este endpoint envía 100 solicitudes de amistad a la cuenta del jugador basada en la región y el ID de usuario especificados.

### 📨 Ejemplo de Solicitud
```http
GET https://free-fire-data.vercel.app/api/spam?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parámetros de Consulta

| Parámetro | Tipo   | Requerido | Descripción                           |
|-----------|--------|-----------|---------------------------------------|
| `region`  | string | Sí        | El código de la región (`sg`, `ind`, `br`) |
| `uid`     | int    | Sí        | El ID del usuario                     |
| `key`     | string | Sí        | Compra la clave en https://t.me/TrueClasher4 |

### ℹ️ Nota Importante

El parámetro de consulta `SG` es para todas las regiones que están bajo `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

El parámetro de consulta `IND` es solo para India y está bajo `client.ind.freefiremobile.com`  
[`IND`]

El parámetro de consulta `BR` es para todas las regiones que están bajo `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Ejemplo de una Respuesta Exitosa Puede Ser Así,
```json
{
  "response": {
    "KeyExpiresAt": "2025-03-20T90:30:00.696969",
    "KeyRemainingRequests": "69/100",
    "FriendRequestsSentByAPI": 100,
    "isPlayerOnline": true,
    "PlayerLevel": 69,
    "PlayerNickname": "SOUNAVA 500K",
    "UID": "2129250963"
  },
  "status": 1
}
```

## API de Imágenes
Ruta de la API = https://free-fire-data.vercel.app/api/images?iconName={iconName}&key={key}

**Endpoint:** `api/images`  
**Clave:** `TU-CLAVE`  
**Método:** `GET`  

Este endpoint recupera información del jugador basada en la región y el ID de usuario especificados.

### 📨 Ejemplo de Solicitud
```http
GET https://free-fire-data.vercel.app/api/images?iconName=Icon_avatar_hair_cos_eggday2021_headwear_blue&key=KEY123
```

### ☑️ Parámetros de Consulta

| Parámetro   | Tipo   | Requerido | Descripción                           |
|-------------|--------|-----------|---------------------------------------|
| `iconName`  | string | Sí        | El nombre del ícono.                  |
| `key`       | string | Sí        | Compra la clave en https://t.me/TrueClasher4 |

### 💬 Ejemplo de una Respuesta Exitosa Puede Ser Así,

![Icon_avatar_hair_cos_eggday2021_headwear_blue](https://github.com/realpega/free-fire-api/blob/main/images.png)

## API de Información de Mapas Craftland
Ruta de la API = https://free-fire-data.vercel.app/api/maps?region={region}&code=%23{CODE}&key={key}

**Endpoint:** `api/maps`  
**Clave:** `TU-CLAVE`  
**Método:** `GET`  

Este endpoint recupera información del jugador basada en la región y el ID de usuario especificados.

### 📨 Ejemplo de Solicitud
```http
GET https://free-fire-data.vercel.app/api/maps?region=sg&code=%23FREEFIREMAPCODE6969&key=KEY123
```

### ☑️ Parámetros de Consulta

| Parámetro | Tipo   | Requerido | Descripción                           |
|-----------|--------|-----------|---------------------------------------|
| `region`  | string | Sí        | El código de la región (`sg`, `ind`, `br`) |
| `uid`     | int    | Sí        | El ID del usuario                     |
| `key`     | string | Sí        | Compra la clave en https://t.me/TrueClasher4 |

### ℹ️ Nota Importante

El parámetro de consulta `SG` es para todas las regiones que están bajo `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

El parámetro de consulta `IND` es solo para India y está bajo `client.ind.freefiremobile.com`  
[`IND`]

El parámetro de consulta `BR` es para todas las regiones que están bajo `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Ejemplo de una Respuesta Exitosa Puede Ser Así,
```json
{
  "code": 0,
  "status": "success",
  "msg": "",
  "data": {
    "region_lang": "SG_en",
    "start_time": 1,
    "end_time": 1890713325,
    "rule": "Garena Free Fire",
    "region": "SG",
    "lang": "en",
    "title": "Garena Free Fire",
    "android_download_url": "https://play.google.com/store/apps/details?id=com.dts.freefireth&referrer=af_tranid%3DgTVeQgRDoYWAmOvmEZz6Xw%26pid%3DOrganicA%26c%3Dmainpage_AND%26af_web_id%3Da209618f-0ae1-4239-bed0-46bcfb0c9656-c",
    "ios_download_url": "https://apps.apple.com/US/app/id1300146617?mt=8",
    "ugc_url": "https://createofficial.garena.com/",
    "imgs": [
      "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/BACKGROUND01.png",
      "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/BACKGROUND02.png",
      "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/BACKGROUND03.png",
      "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/BACKGROUND04.png",
      "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/BACKGROUND05.png"
    ],
    "game_icon": "https://dl.dir.freefiremobile.com/common/OB45/CSH/abcdfallstorebanners/appicon/FF_AndroidIcon_512.png",
    "game_name": "Free Fire: 7th Anniversary!",
    "transify": {
      "COMMON_ACCEPT": "ACEPTAR",
      "COMMON_BACK": "Volver",
      "COMMON_CANCEL": "Cancelar",
      "COMMON_CONFIRM": "Confirmar",
      "COMMON_CONTINUE_PURCHASE": "Continuar para comprar",
      "COMMON_COPY": "Copiar",
      "COMMON_COPY_FAILED": "Copia fallida",
      "COMMON_COPY_SUCCESS": "Copia exitosa",
      "COMMON_EXCHANGE": "Canjear",
      "COMMON_EXCHANGED": "Canjeado",
      "COMMON_FFTOKEN_HINT": "Convertido a {num}{ícono de token ff}",
      "COMMON_FREE": "Gratis",
      "COMMON_GEM_CONFIRM": "¿Gastar {cost} gema(s) para comprar {NAME}?",
      "COMMON_GEM_CONFIRM2": "¿Gastar {cost} gemas para {num} giro(s)?",
      "COMMON_HISTORY_DRAW": "Historial",
      "COMMON_HISTORY_NORECORDS": "Sin registros",
      "COMMON_HISTORY_PURCHASE": "Historial de compras",
      "COMMON_HISTORY_REDEEM": "Historial de canjes",
      "COMMON_NO": "No",
      "COMMON_OWNED": "POSEÍDO",
      "COMMON_PRIZEPOOL": "Piscina de recompensas",
      "COMMON_PURCHASE": "Comprar",
      "COMMON_PURCHASED": "Comprado",
      "COMMON_QUANTITY_MAX": "Máximo",
      "COMMON_REDEEM_CONFIRM": "¿Estás seguro de canjear este artículo?",
      "COMMON_REJECT": "Rechazar",
      "COMMON_RULE": "Reglas",
      "COMMON_SKIP": "Omitir animación",
      "COMMON_SKIPANIMATION_TIP": "Toca en cualquier lugar para omitir la animación",
      "COMMON_SPIN_AGAIN": "Girar de nuevo",
      "COMMON_TIPS_ITEM": "Las recompensas se enviarán directamente a tu bóveda",
      "COMMON_TIPS_TOKEN": "Los tokens se han acumulado automáticamente",
      "COMMON_VISIT_GIFT": "Regalo de bienvenida",
      "COMMON_YES": "Sí",
      "POPUP_NO_REMIND": "No me lo recuerdes de nuevo",
      "POPUP_TITLE_CONGRATULATIONS": "¡Felicidades!",
      "POPUP_TITLE_REDEEM": "¡Felicidades! Conseguiste",
      "POPUP_TITLE_UNIQUE": "Los artículos únicos que posees",
      "UNIQUE_BUY_ALREADY_HAVE": "Ya posees este artículo, si lo compras de nuevo, se convertirá en tokens FF",
      "UNIQUE_BUY_ALREADY_HAVE_PART": "Ya posees algunos de los artículo(s) seleccionados. Si los recibes de nuevo, se convertirán en tokens FF.",
      "UNIQUE_REDEEM_ALREADY_HAVE": "Ya posees este artículo, si lo recibes de nuevo, se convertirá en tokens FF.",
      "TOAST_ERROR_CODE": "Error desconocido, código de error {code}",
      "TOAST_EVENTOVER": "Evento finalizado",
      "TOAST_EVENT_CLOSED_AWHILE": "El evento está cerrado temporalmente. Por favor, verifica de nuevo más tarde.",
      "TOAST_EVENT_END": "Evento finalizado",
      "TOAST_EVENT_NOTOPEN": "El evento aún no ha comenzado",
      "TOAST_EXCHANGE_SUCCESS": "Canjeado con éxito",
      "TOAST_GEM_NOT_ENOUGH": "Diamantes insuficientes, por favor recarga y vuelve de nuevo",
      "TOAST_LOGIN_FAILED": "Inicio de sesión fallido",
      "TOAST_NETWORK_BUSY": "Servidor ocupado, por favor intenta de nuevo más tarde",
      "TOAST_NETWORK_ERROR": "Error de conexión de red, por favor intenta de nuevo más tarde",
      "TOAST_OPERATE_BUSY": "Demasiadas solicitudes, por favor intenta de nuevo más tarde",
      "TOAST_PAY_FAILED": "Compra fallida",
      "TOAST_PURCHASE_SUCCESS": "Compra exitosa",
      "TOAST_SERVER_BUSY": "Servidor ocupado, por favor intenta de nuevo más tarde",
      "TOAST_SERVER_NOTWORK": "Servicio no disponible",
      "TOAST_SERVER_TIMEOUT": "Tiempo de espera del servicio",
      "TOAST_WRONG_REGION": "Este evento no está disponible para tu región",
      "COMMON_CALLBACK": "¡Únete a la lucha!",
      "COMMON_JOIN": "Unirse",
      "COMMON_SHOOT": "Toca los objetivos",
      "COMMON_SHOOT_2": "¡Buen trabajo! Para continuar, por favor dirígete a Free Fire!",
      "UGC_46_MAPSHARE_GOBUTTON": "EXPLORAR MÁS",
      "UGC_46_MAPSHARE_PLAYBUTTON": "JUGAR AHORA",
      "UGC_46_MAPSHARE_WRONGMESSAGE": "LO SIENTO, ESTE MAPA NO ESTÁ DISPONIBLE EN ESTE MOMENTO.",
      "UGC_47_MAPSHARE_MAPCODE": "Código del Mapa",
      "UGC_47_MAPSHARE_NAME": "Nombre del Creador",
      "UGC_47_MAPSHARE_TOAST1": "Copiado con éxito",
      "UGC_47_MAPSHARE_TOAST2": "Fallo al copiar"
    },
    "share_img": "https://dl.dir.freefiremobile.com/common/OB46/CSH/Devs/WebCDN/SOFTFF.jpg",
    "desc_prefix": "[Free Fire]{desc}",
    "source_params": {
      "region": "",
      "lang": "en",
      "version": "",
      "action": "",
      "map_code": ""
    }
  }
}
```

## API de Lista de Deseos del Jugador
Ruta de la API = https://free-fire-data.vercel.app/api/wishlist?region={region}&uid={uid}&key={key}

**Endpoint:** `api/wishlist`  
**Clave:** `TU-CLAVE`  
**Método:** `GET`  

Este endpoint recupera información del jugador basada en la región y el ID de usuario especificados.

### 📨 Ejemplo de Solicitud
```http
GET https://free-fire-data.vercel.app/api/wishlist?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parámetros de Consulta

| Parámetro | Tipo   | Requerido | Descripción                           |
|-----------|--------|-----------|---------------------------------------|
| `region`  | string | Sí        | El código de la región (`sg`, `ind`, `br`) |
| `uid`     | int    | Sí        | El ID del usuario                     |
| `key`     | string | Sí        | Compra la clave en https://t.me/TrueClasher4 |

### ℹ️ Nota Importante

El parámetro de consulta `SG` es para todas las regiones que están bajo `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

El parámetro de consulta `IND` es solo para India y está bajo `client.ind.freefiremobile.com`  
[`IND`]

El parámetro de consulta `BR` es para todas las regiones que están bajo `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Ejemplo de una Respuesta Exitosa Puede Ser Así,
```json
{
  "items": [
    {
      "itemId": 102000035,
      "releaseTime": 1709233149
    },
    {
      "itemId": 203000036,
      "releaseTime": 1710238335
    },
    {
      "itemId": 203000981,
      "releaseTime": 1706079412
    },
    {
      "itemId": 204033044,
      "releaseTime": 1706079412
    },
    {
      "itemId": 205033048,
      "releaseTime": 1706079412
    },
    {
      "itemId": 211000411,
      "releaseTime": 1706079412
    },
    {
      "itemId": 211000894,
      "releaseTime": 1706079412
    },
    {
      "itemId": 214000023,
      "releaseTime": 1706079412
    },
    {
      "itemId": 901040034,
      "releaseTime": 1727692721
    },
    {
      "itemId": 902000003,
      "releaseTime": 1710238335
    },
    {
      "itemId": 902040026,
      "releaseTime": 1710238335
    },
    {
      "itemId": 902040029,
      "releaseTime": 1710238335
    },
    {
      "itemId": 902040030,
      "releaseTime": 1710238335
    },
    {
      "itemId": 903040007,
      "releaseTime": 1727692721
    },
    {
      "itemId": 903043010,
      "releaseTime": 1710238335
    },
    {
      "itemId": 904040010,
      "releaseTime": 1727692721
    },
    {
      "itemId": 904090027,
      "releaseTime": 1707398570
    },
    {
      "itemId": 905039004,
      "releaseTime": 1710238335
    },
    {
      "itemId": 906036010,
      "releaseTime": 1706524016
    },
    {
      "itemId": 907102508,
      "releaseTime": 1706079412
    },
    {
      "itemId": 907104073,
      "releaseTime": 1727692721
    },
    {
      "itemId": 907104074,
      "releaseTime": 1727692721
    },
    {
      "itemId": 907104075,
      "releaseTime": 1727692721
    },
    {
      "itemId": 907104076,
      "releaseTime": 1727692721
    },
    {
      "itemId": 907104077,
      "releaseTime": 1727692721
    },
    {
      "itemId": 909040014,
      "releaseTime": 1727692721
    },
    {
      "itemId": 909043013,
      "releaseTime": 1707543814
    },
    {
      "itemId": 911004301,
      "releaseTime": 1710238335
    },
    {
      "itemId": 912037001,
      "releaseTime": 1706079412
    },
    {
      "itemId": 921047018,
      "releaseTime": 1735657844
    }
  ]
}
```

📚 **Propósito de la API**

El propósito principal de proporcionar esta API gratuita es mejorar la experiencia de la comunidad de Free Fire. Garena Free Fire no ofrece APIs oficiales de información de cuentas, por lo que esta solución personalizada busca llenar ese vacío, proporcionando a los jugadores y desarrolladores datos valiosos de la cuenta.

🧩 **(Algunos de los🤫) Frameworks y Bibliotecas Utilizados**  
- **Flask**: Un microframework web para Python para construir los endpoints de la API.  
- **Flask-CORS**: Para manejar el Compartilhamento de Recursos de Origen Cruzado (CORS).  
- **PyCryptodome**: Para implementar desencriptación y encriptación.  
- **Requests**: Para realizar solicitudes HTTP al servidor.

# 📁 Información Adicional

- Esta respuesta de la API no representa la estructura real recibida del servidor oficial de Garena.  
- La estructura de la respuesta está simplificada en un formato amigable para el usuario para facilitar la comprensión de cualquier persona, en cualquier nivel de programación.

# 😵 Respuestas de Error
¡La API puede mostrar respuestas de error debido a solicitudes imprecisas de los usuarios!

### Instancias de Error y Soluciones

- **Código de Error:** 400
  - **Mensaje:** Región inválida.  
  - **Solución:** Asegúrate de estar usando un código de región válido.

- **Código de Error:** 429
  - **Mensaje:** Solicitudes anormales detectadas. ¡Por favor, evita usar incorrectamente la API de Información para Visitas o tu IP podría ser bloqueado!  
  - **Solución:** Evita solicitudes excesivas o contacta al proveedor de la API para asistencia.

- **Código de Error:** 500
  - **Mensaje:** Ocurrió un error al procesar tu solicitud. Por favor, revisa tu ID y Región nuevamente.  
  - **Solución:** Verifica nuevamente el ID de usuario y la región proporcionados e intenta de nuevo la solicitud. Si el problema persiste, contacta al proveedor de la API para soporte.

---

API creada por Sounava777,  
¡Todos los derechos reservados!
