# <a href="README_BR.md">Leia em Português</a>
# <a href="README_ES.md">Leer en Español</a>
# <a href="README_RU.md">Читать на Русском языке</a>
# <a href="README_AR.md">اقرأ باللغة العربية</a>
# <a href="README_ID.md">Baca dalam bahasa Indonesia</a>
# <a href="README_VN.md">Đọc bằng tiếng Việt</a>

<br />

# 📝 API Documentation

##  Player Information API
API Route = https://ff.deaddos.online/api/data?region={region}&uid={uid}&key={key}

**Endpoint:** `api/data`
**key:** `YOUR-KEY`
**Method:** `GET`  

This Endpoint Retrieves Player Information based on the Specified Region and User ID.

### 📨 Request Example
```http
GET https://ff.deaddos.online/api/data?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `region`  | string | Yes      | The region code (`sg`, `ind`, `br`)|
| `uid`     | int    | Yes      | The user ID                   |
| `key`     | string | Yes      | Buy Key from https://t.me/TrueClasher4                  |

### ℹ️ Important Note

Query Parameter `SG` is for all regions that come under `clientbp.ggblueshark.com`
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Query Parameter `IND` is only for India and it comes under `client.ind.freefiremobile.com `
[`IND`]

Query Parameter `BR` is for all regions that come under `client.us.freefiremobile.com`
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Example of a Successful Reponse May Look Like this,
```json
{
  "basicInfo": {
    "accountId": "2129250963",
    "accountPrefers": {
      "brPregameShowChoices": [1]
    },
    "accountType": 1,
    "badgeCnt": 9,
    "badgeId": "1001000088",
    "bannerId": "901000262",
    "createAt": "1593158767",
    "csMaxRank": 321,
    "csRank": 321,
    "csRankingPoints": 90,
    "exp": "271246",
    "externalIconInfo": {
      "showType": 1,
      "status": 1
    },
    "headPic": "902050009",
    "lastLoginAt": "1757418491",
    "level": 49,
    "liked": 9466,
    "maxRank": 316,
    "nickname": "GM SOUNAVA",
    "primePrivilegeDetail": {
      "accountId": "2129250963",
      "primeLevel": 1,
      "privilegeIdList": [16, 20]
    },
    "rank": 316,
    "rankingPoints": 2778,
    "region": "IND",
    "releaseVersion": "OB50",
    "seasonId": 47,
    "selectOccupations": [
      {
        "details": {
          "key1": 1,
          "key2": 7,
          "key3": 6,
          "key4": 1,
          "key5": 1
        },
        "modeId": 1,
        "seasonId": 47,
        "type": 2
      },
      {
        "details": {
          "key1": 3,
          "key2": 243,
          "key3": 154,
          "key4": 5,
          "key5": 1
        },
        "modeId": 15,
        "seasonId": 33,
        "type": 6
      }
    ],
    "showBrRank": true,
    "showCsRank": true,
    "showRank": true,
    "title": "904090025",
    "weaponSkinShows": [
      "907104303"
    ]
  },
  "captainBasicInfo": {
    "accountId": "2787909984",
    "accountPrefers": {
      "brPregameShowChoices": [1]
    },
    "accountType": 1,
    "badgeCnt": 45,
    "badgeId": "1001000088",
    "bannerId": "901026021",
    "createAt": "1612368377",
    "csMaxRank": 324,
    "csRank": 324,
    "csRankingPoints": 232,
    "exp": "4838515",
    "externalIconInfo": {
      "showType": 1,
      "status": 1
    },
    "extraField_77": 1399,
    "extraField_78": 1,
    "headPic": "902000192",
    "lastLoginAt": "1757428278",
    "level": 76,
    "liked": 33703,
    "maxRank": 324,
    "nickname": "ㅤGMㅤㅤVISHWA",
    "primePrivilegeDetail": {
      "accountId": "2787909984",
      "primeLevel": 5,
      "privilegeIdList": [8, 11, 19, 4, 12, 15, 17, 7, 16, 20, 10]
    },
    "rank": 324,
    "rankingPoints": 4975,
    "region": "IND",
    "releaseVersion": "OB50",
    "seasonId": 47,
    "selectOccupations": [
      {
        "details": {
          "key1": 3,
          "key2": 274,
          "key3": 163,
          "key4": 6,
          "key5": 1
        },
        "modeId": 1,
        "seasonId": 47,
        "type": 2
      },
      {
        "details": {
          "key1": 5,
          "key2": 606,
          "key3": 524,
          "key4": 13,
          "key5": 1
        },
        "modeId": 15,
        "seasonId": 33,
        "type": 6
      }
    ],
    "showBrRank": true,
    "showCsRank": true,
    "title": "904590059",
    "weaponSkinShows": [
      "907104418",
      "912044001",
      "914044001"
    ]
  },
  "clanBasicInfo": {
    "capacity": 55,
    "captainId": "2787909984",
    "clanId": "3012174478",
    "clanLevel": 7,
    "clanName": "GɅMEㅤMɅSTERS",
    "memberNum": 49
  },
  "creditScoreInfo": {
    "creditScore": 100,
    "rewardEndAt": "1757498835",
    "rewardStartAt": "1757239635",
    "rewardState": 1,
    "rewardType": 2
  },
  "diamondCostRes": {
    "diamondCost": 390
  },
  "petInfo": {
    "exp": 548,
    "id": "1300000120",
    "isSelected": true,
    "level": 4,
    "selectedSkillId": "1315000012",
    "skinId": "1310000201"
  },
  "profileInfo": {
    "avatarId": "101000001",
    "clothes": [
      "203043035",
      "205043004",
      "204043004",
      "211000733",
      "214000000",
      "211000124"
    ],
    "equipedSkills": [
      {
        "skillId": 5506
      },
      {
        "skillId": 501,
        "slotId": 1
      },
      {
        "skillId": 4806,
        "slotId": 2
      },
      {
        "skillId": 4901,
        "slotId": 3
      }
    ],
    "isSelected": true,
    "isSelectedAwaken": true
  },
  "socialInfo": {
    "accountId": "2129250963",
    "signature": "ya libliyu vsekh devushek na zemlya"
  }
}
```

##  Player Stats API
API Route = https://stats.ff.deaddos.online/api/{region}?uid={uid}&key={key}

**Endpoint:** `api/{region}`
**key:** `YOUR-KEY`
**Method:** `GET`  

This Endpoint Retrieves Player Information based on the Specified Region and User ID.

### 📨 Request Example
```http
GET https://stats.ff.deaddos.online/api/ind?uid=2129250963&key=KEY123
```

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `region`  | string | Yes      | The region code (`sg`, `ind`, `br`)|
| `uid`     | int    | Yes      | The user ID                   |
| `key`     | string | Yes      | Buy Key from https://t.me/TrueClasher4                  |

### ℹ️ Important Note

Query Parameter `SG` is for all regions that come under `clientbp.ggblueshark.com`
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Query Parameter `IND` is only for India and it comes under `client.ind.freefiremobile.com `
[`IND`]

Query Parameter `BR` is for all regions that come under `client.us.freefiremobile.com`
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Example of a Successful Reponse May Look Like this,
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

##  Likes API
API Route = https://free-fire-data.vercel.app/api/like?region={region}&uid={uid}&key={key}

**Endpoint:** `api/like`
**key:** `YOUR-KEY`
**Method:** `GET`  

This Endpoint Sends 100 Likes to the Player's Account based on the Specified Region and User ID.

### 📨 Request Example
```http
GET https://free-fire-data.vercel.app/api/like?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `region`  | string | Yes      | The region code (`sg`, `ind`, `br`)|
| `uid`     | int    | Yes      | The user ID                   |
| `key`     | string | Yes      | Buy Key from https://t.me/TrueClasher4                  |

### ℹ️ Important Note

Query Parameter `SG` is for all regions that come under `clientbp.ggblueshark.com`
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Query Parameter `IND` is only for India and it comes under `client.ind.freefiremobile.com `
[`IND`]

Query Parameter `BR` is for all regions that come under `client.us.freefiremobile.com`
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Example of a Successful Reponse May Look Like this,
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

##  Visits API
API Route = https://free-fire-data.vercel.app/api/visit?region={region}&uid={uid}&key={key}

**Endpoint:** `api/visit`
**key:** `YOUR-KEY`
**Method:** `GET`  

This Endpoint Sends 100 Visits to the Player's Account based on the Specified Region and User ID.

### 📨 Request Example
```http
GET https://free-fire-data.vercel.app/api/visit?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `region`  | string | Yes      | The region code (`sg`, `ind`, `br`)|
| `uid`     | int    | Yes      | The user ID                   |
| `key`     | string | Yes      | Buy Key from https://t.me/TrueClasher4                  |

### ℹ️ Important Note

Query Parameter `SG` is for all regions that come under `clientbp.ggblueshark.com`
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Query Parameter `IND` is only for India and it comes under `client.ind.freefiremobile.com `
[`IND`]

Query Parameter `BR` is for all regions that come under `client.us.freefiremobile.com`
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Example of a Successful Reponse May Look Like this,
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

##  Spam API
API Route = https://free-fire-data.vercel.app/api/spam?region={region}&uid={uid}&key={key}

**Endpoint:** `api/spam`
**key:** `YOUR-KEY`
**Method:** `GET`  

This Endpoint Spams 100 Friend Requests to the Player's Account based on the Specified Region and User ID.

### 📨 Request Example
```http
GET https://free-fire-data.vercel.app/api/spam?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `region`  | string | Yes      | The region code (`sg`, `ind`, `br`)|
| `uid`     | int    | Yes      | The user ID                   |
| `key`     | string | Yes      | Buy Key from https://t.me/TrueClasher4                  |

### ℹ️ Important Note

Query Parameter `SG` is for all regions that come under `clientbp.ggblueshark.com`
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Query Parameter `IND` is only for India and it comes under `client.ind.freefiremobile.com `
[`IND`]

Query Parameter `BR` is for all regions that come under `client.us.freefiremobile.com`
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Example of a Successful Reponse May Look Like this,
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

##  Images API
API Route = https://free-fire-data.vercel.app/api/images?iconName={iconName}&key={key}

**Endpoint:** `api/images`
**key:** `YOUR-KEY`
**Method:** `GET`  

This Endpoint Retrieves Player Information based on the Specified Region and User ID.

### 📨 Request Example
```http
GET https://free-fire-data.vercel.app/api/images?iconName=Icon_avatar_hair_cos_eggday2021_headwear_blue&key=KEY123
```

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `iconName`  | string | Yes      | The name of the Icon. |
| `key`     | string | Yes      | Buy Key from https://t.me/TrueClasher4 


### 💬 Example of a Successful Reponse May Look Like this,

![Icon_avatar_hair_cos_eggday2021_headwear_blue](https://github.com/realpega/free-fire-api/blob/main/images.png)

##  Craftland Map Info API
API Route = https://free-fire-data.vercel.app/api/maps?region={region}&code=%23{CODE}&key={key}

**Endpoint:** `api/maps`
**key:** `YOUR-KEY`
**Method:** `GET`  

This Endpoint Retrieves Player Information based on the Specified Region and User ID.

### 📨 Request Example
```http
GET https://free-fire-data.vercel.app/api/maps?region=sg&code=%23FREEFIREMAPCODE6969&key=KEY123
```

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `region`  | string | Yes      | The region code (`sg`, `ind`, `br`)|
| `uid`     | int    | Yes      | The user ID                   |
| `key`     | string | Yes      | Buy Key from https://t.me/TrueClasher4                  |

### ℹ️ Important Note

Query Parameter `SG` is for all regions that come under `clientbp.ggblueshark.com`
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Query Parameter `IND` is only for India and it comes under `client.ind.freefiremobile.com `
[`IND`]

Query Parameter `BR` is for all regions that come under `client.us.freefiremobile.com`
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Example of a Successful Reponse May Look Like this,
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
      "COMMON_ACCEPT": "ACCEPT",
      "COMMON_BACK": "Back",
      "COMMON_CANCEL": "Cancel",
      "COMMON_CONFIRM": "Confirm",
      "COMMON_CONTINUE_PURCHASE": "Continue to buy",
      "COMMON_COPY": "Copy",
      "COMMON_COPY_FAILED": "Copy Failed",
      "COMMON_COPY_SUCCESS": "copy successful",
      "COMMON_EXCHANGE": "redeem",
      "COMMON_EXCHANGED": "redeemed",
      "COMMON_FFTOKEN_HINT": "Converted to {num}{ff token icon}",
      "COMMON_FREE": "free",
      "COMMON_GEM_CONFIRM": "Spend {cost} gem(s) to purchase {NAME}?",
      "COMMON_GEM_CONFIRM2": "Spend {cost} gems for {num} spin(s)?",
      "COMMON_HISTORY_DRAW": "History",
      "COMMON_HISTORY_NORECORDS": "No records",
      "COMMON_HISTORY_PURCHASE": "Purchase history",
      "COMMON_HISTORY_REDEEM": "Redeem history",
      "COMMON_NO": "No",
      "COMMON_OWNED": "OWNED",
      "COMMON_PRIZEPOOL": "Rewards pool",
      "COMMON_PURCHASE": "Purchase",
      "COMMON_PURCHASED": "Purchased",
      "COMMON_QUANTITY_MAX": "max",
      "COMMON_REDEEM_CONFIRM": "Are you sure to redeem this item?",
      "COMMON_REJECT": "Decline",
      "COMMON_RULE": "Rules",
      "COMMON_SKIP": "Skip animation",
      "COMMON_SKIPANIMATION_TIP": "Tap anywhere to skip animation",
      "COMMON_SPIN_AGAIN": "Spin Again",
      "COMMON_TIPS_ITEM": "The rewards will be sent directly to your vault",
      "COMMON_TIPS_TOKEN": "tokens have been automatically accumulated",
      "COMMON_VISIT_GIFT": "Welcome gift",
      "COMMON_YES": "Yes",
      "POPUP_NO_REMIND": "Don't remind me again",
      "POPUP_TITLE_CONGRATULATIONS": "Congratulations!",
      "POPUP_TITLE_REDEEM": "Congratulation! You got",
      "POPUP_TITLE_UNIQUE": "The unique items you own",
      "UNIQUE_BUY_ALREADY_HAVE": "You already own this item, if you purchase it again, it will be converted to FF tokens",
      "UNIQUE_BUY_ALREADY_HAVE_PART": "You already own some of the item(s) you selected. If you receive again, it will be converted to FF tokens.",
      "UNIQUE_REDEEM_ALREADY_HAVE": "You already own this item, if you receive it again, it will be converted to FF tokens.",
      "TOAST_ERROR_CODE": "Unknown error, error code {code}",
      "TOAST_EVENTOVER": "Event ended",
      "TOAST_EVENT_CLOSED_AWHILE": "The event is closed temporarily. Please check again later.",
      "TOAST_EVENT_END": "Event ended",
      "TOAST_EVENT_NOTOPEN": "Event hasn't started",
      "TOAST_EXCHANGE_SUCCESS": "Successfully Redeemed",
      "TOAST_GEM_NOT_ENOUGH": "Insufficient diamonds, please top up and come back again",
      "TOAST_LOGIN_FAILED": "Login failed",
      "TOAST_NETWORK_BUSY": "Server busy, please try again later",
      "TOAST_NETWORK_ERROR": "Network connection error, please try again later",
      "TOAST_OPERATE_BUSY": "Too many requests, please try again later",
      "TOAST_PAY_FAILED": "Purchase failed",
      "TOAST_PURCHASE_SUCCESS": "Purchase Successful",
      "TOAST_SERVER_BUSY": "Server busy, please try again later",
      "TOAST_SERVER_NOTWORK": "Service unavailable",
      "TOAST_SERVER_TIMEOUT": "Service timeout",
      "TOAST_WRONG_REGION": "This event is not available for your region",
      "COMMON_CALLBACK": "Join the Fight!",
      "COMMON_JOIN": "Join",
      "COMMON_SHOOT": "Tap on the targets",
      "COMMON_SHOOT_2": "Good Job! To continue, please head to Free Fire!",
      "UGC_46_MAPSHARE_GOBUTTON": "EXPLORE MORE",
      "UGC_46_MAPSHARE_PLAYBUTTON": "PLAY NOW",
      "UGC_46_MAPSHARE_WRONGMESSAGE": "SORRY, THIS MAP IS NOT AVAILABLE AT THE MOMENT.",
      "UGC_47_MAPSHARE_MAPCODE": "Map Code",
      "UGC_47_MAPSHARE_NAME": "Creator Name",
      "UGC_47_MAPSHARE_TOAST1": "Copied successfully",
      "UGC_47_MAPSHARE_TOAST2": "Failed to copy"
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

##  Player Wishlist API
API Route = https://free-fire-data.vercel.app/api/wishlist?region={region}&uid={uid}&key={key}

**Endpoint:** `api/wishlist`
**key:** `YOUR-KEY`
**Method:** `GET`  

This Endpoint Retrieves Player Information based on the Specified Region and User ID.

### 📨 Request Example
```http
GET https://free-fire-data.vercel.app/api/wishlist?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| `region`  | string | Yes      | The region code (`sg`, `ind`, `br`)|
| `uid`     | int    | Yes      | The user ID                   |
| `key`     | string | Yes      | Buy Key from https://t.me/TrueClasher4                  |

### ℹ️ Important Note

Query Parameter `SG` is for all regions that come under `clientbp.ggblueshark.com`
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Query Parameter `IND` is only for India and it comes under `client.ind.freefiremobile.com `
[`IND`]

Query Parameter `BR` is for all regions that come under `client.us.freefiremobile.com`
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Example of a Successful Reponse May Look Like this,

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

📚 **Purpose of the API**  

The primary purpose of providing this free API is to enhance the Free Fire community experience. Garena Free Fire does not offer official account information APIs, so this custom solution aims to fill that gap, providing players and developers with valuable account data

🧩 **(Some of🤫) Frameworks and Libraries Used**  
- **Flask**: A micro web framework for Python to build the API endpoints.
- **Flask-CORS**: For handling Cross-Origin Resource Sharing (CORS).
- **PyCryptodome**: For implementing Decryption and Encryption.
- **Requests**: For making HTTP Requests to Server.

# 📁 Additional Information

- This API response Does not Represent the Actual Structure Received from the Official Garena Server.
- The Response structure is simplified in an User-Friendly Structure for the ease of understanding for Anyone at any level of Programming.

# 😵 Error Responses
API might Show Error Response Upon Users' Inaccurate Requests!

### Error Instances and Solutions

- **Error Code:** 400
  - **Message:** Invalid region.
  - **Solution:** Make sure you are using a valid region code.

- **Error Code:** 429
  - **Message:** Abnormal Requests Detected. Please Avoid Misusing Info API for Visits or Your IP may get Blocked!
  - **Solution:** Avoid excessive requests or contact the API provider for assistance.

- **Error Code:** 500
  - **Message:** An error occurred while processing your request. Please Recheck Your ID & Region.
  - **Solution:** Double-check the provided user ID and region, and retry the request. If the issue persists, contact the API provider for support.

---

API Made By Sounava777,
All Rights Reserved!
