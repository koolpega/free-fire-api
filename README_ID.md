# 📝 Dokumentasi API

## API Informasi Pemain
Rute API = https://free-fire-data.vercel.app/api/data?region={region}&uid={uid}&key={key}

**Endpoint:** `api/data`  
**Kunci:** `KUNCI-ANDA`  
**Metode:** `GET`  

Endpoint ini mengambil informasi pemain berdasarkan wilayah dan ID pengguna yang ditentukan.

### 📨 Contoh Permintaan
```http
GET https://free-fire-data.vercel.app/api/data?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parameter Kueri

| Parameter | Tipe   | Wajib | Deskripsi                            |
|-----------|--------|-------|--------------------------------------|
| `region`  | string | Ya    | Kode wilayah (`sg`, `ind`, `br`)     |
| `uid`     | int    | Ya    | ID pengguna                         |
| `key`     | string | Ya    | Beli kunci dari https://t.me/TrueClasher4 |

### ℹ️ Catatan Penting

Parameter kueri `SG` untuk semua wilayah yang berada di bawah `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parameter kueri `IND` hanya untuk India dan berada di bawah `client.ind.freefiremobile.com`  
[`IND`]

Parameter kueri `BR` untuk semua wilayah yang berada di bawah `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Contoh Respons Berhasil Mungkin Terlihat Seperti Ini,
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

## API Statistik Pemain
Rute API = https://free-fire-data.vercel.app/api/stats?region={region}&uid={uid}&key={key}

**Endpoint:** `api/stats`  
**Kunci:** `KUNCI-ANDA`  
**Metode:** `GET`  

Endpoint ini mengambil informasi statistik pemain berdasarkan wilayah dan ID pengguna yang ditentukan.

### 📨 Contoh Permintaan
```http
GET https://free-fire-data.vercel.app/api/stats?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parameter Kueri

| Parameter | Tipe   | Wajib | Deskripsi                            |
|-----------|--------|-------|--------------------------------------|
| `region`  | string | Ya    | Kode wilayah (`sg`, `ind`, `br`)     |
| `uid`     | int    | Ya    | ID pengguna                         |
| `key`     | string | Ya    | Beli kunci dari https://t.me/TrueClasher4 |

### ℹ️ Catatan Penting

Parameter kueri `SG` untuk semua wilayah yang berada di bawah `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parameter kueri `IND` hanya untuk India dan berada di bawah `client.ind.freefiremobile.com`  
[`IND`]

Parameter kueri `BR` untuk semua wilayah yang berada di bawah `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Contoh Respons Berhasil Mungkin Terlihat Seperti Ini,
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

## API Suka
Rute API = https://free-fire-data.vercel.app/api/like?region={region}&uid={uid}&key={key}

**Endpoint:** `api/like`  
**Kunci:** `KUNCI-ANDA`  
**Metode:** `GET`  

Endpoint ini mengirimkan 100 suka ke akun pemain berdasarkan wilayah dan ID pengguna yang ditentukan.

### 📨 Contoh Permintaan
```http
GET https://free-fire-data.vercel.app/api/like?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parameter Kueri

| Parameter | Tipe   | Wajib | Deskripsi                            |
|-----------|--------|-------|--------------------------------------|
| `region`  | string | Ya    | Kode wilayah (`sg`, `ind`, `br`)     |
| `uid`     | int    | Ya    | ID pengguna                         |
| `key`     | string | Ya    | Beli kunci dari https://t.me/TrueClasher4 |

### ℹ️ Catatan Penting

Parameter kueri `SG` untuk semua wilayah yang berada di bawah `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parameter kueri `IND` hanya untuk India dan berada di bawah `client.ind.freefiremobile.com`  
[`IND`]

Parameter kueri `BR` untuk semua wilayah yang berada di bawah `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Contoh Respons Berhasil Mungkin Terlihat Seperti Ini,
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

## API Kunjungan
Rute API = https://free-fire-data.vercel.app/api/visit?region={region}&uid={uid}&key={key}

**Endpoint:** `api/visit`  
**Kunci:** `KUNCI-ANDA`  
**Metode:** `GET`  

Endpoint ini mengirimkan 100 kunjungan ke akun pemain berdasarkan wilayah dan ID pengguna yang ditentukan.

### 📨 Contoh Permintaan
```http
GET https://free-fire-data.vercel.app/api/visit?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parameter Kueri

| Parameter | Tipe   | Wajib | Deskripsi                            |
|-----------|--------|-------|--------------------------------------|
| `region`  | string | Ya    | Kode wilayah (`sg`, `ind`, `br`)     |
| `uid`     | int    | Ya    | ID pengguna                         |
| `key`     | string | Ya    | Beli kunci dari https://t.me/TrueClasher4 |

### ℹ️ Catatan Penting

Parameter kueri `SG` untuk semua wilayah yang berada di bawah `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parameter kueri `IND` hanya untuk India dan berada di bawah `client.ind.freefiremobile.com`  
[`IND`]

Parameter kueri `BR` untuk semua wilayah yang berada di bawah `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Contoh Respons Berhasil Mungkin Terlihat Seperti Ini,
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

## API Spam
Rute API = https://free-fire-data.vercel.app/api/spam?region={region}&uid={uid}&key={key}

**Endpoint:** `api/spam`  
**Kunci:** `KUNCI-ANDA`  
**Metode:** `GET`  

Endpoint ini mengirimkan 100 permintaan pertemanan ke akun pemain berdasarkan wilayah dan ID pengguna yang ditentukan.

### 📨 Contoh Permintaan
```http
GET https://free-fire-data.vercel.app/api/spam?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parameter Kueri

| Parameter | Tipe   | Wajib | Deskripsi                            |
|-----------|--------|-------|--------------------------------------|
| `region`  | string | Ya    | Kode wilayah (`sg`, `ind`, `br`)     |
| `uid`     | int    | Ya    | ID pengguna                         |
| `key`     | string | Ya    | Beli kunci dari https://t.me/TrueClasher4 |

### ℹ️ Catatan Penting

Parameter kueri `SG` untuk semua wilayah yang berada di bawah `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parameter kueri `IND` hanya untuk India dan berada di bawah `client.ind.freefiremobile.com`  
[`IND`]

Parameter kueri `BR` untuk semua wilayah yang berada di bawah `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Contoh Respons Berhasil Mungkin Terlihat Seperti Ini,
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

## API Gambar
Rute API = https://free-fire-data.vercel.app/api/images?iconName={iconName}&key={key}

**Endpoint:** `api/images`  
**Kunci:** `KUNCI-ANDA`  
**Metode:** `GET`  

Endpoint ini mengambil informasi pemain berdasarkan wilayah dan ID pengguna yang ditentukan.

### 📨 Contoh Permintaan
```http
GET https://free-fire-data.vercel.app/api/images?iconName=Icon_avatar_hair_cos_eggday2021_headwear_blue&key=KEY123
```

### ☑️ Parameter Kueri

| Parameter  | Tipe   | Wajib | Deskripsi                            |
|------------|--------|-------|--------------------------------------|
| `iconName` | string | Ya    | Nama ikon.                          |
| `key`      | string | Ya    | Beli kunci dari https://t.me/TrueClasher4 |

### 💬 Contoh Respons Berhasil Mungkin Terlihat Seperti Ini,

![Icon_avatar_hair_cos_eggday2021_headwear_blue](https://github.com/realpega/free-fire-api/blob/main/images.png)

## API Informasi Peta Craftland
Rute API = https://free-fire-data.vercel.app/api/maps?region={region}&code=%23{CODE}&key={key}

**Endpoint:** `api/maps`  
**Kunci:** `KUNCI-ANDA`  
**Metode:** `GET`  

Endpoint ini mengambil informasi pemain berdasarkan wilayah dan ID pengguna yang ditentukan.

### 📨 Contoh Permintaan
```http
GET https://free-fire-data.vercel.app/api/maps?region=sg&code=%23FREEFIREMAPCODE6969&key=KEY123
```

### ☑️ Parameter Kueri

| Parameter | Tipe   | Wajib | Deskripsi                            |
|-----------|--------|-------|--------------------------------------|
| `region`  | string | Ya    | Kode wilayah (`sg`, `ind`, `br`)     |
| `uid`     | int    | Ya    | ID pengguna                         |
| `key`     | string | Ya    | Beli kunci dari https://t.me/TrueClasher4 |

### ℹ️ Catatan Penting

Parameter kueri `SG` untuk semua wilayah yang berada di bawah `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parameter kueri `IND` hanya untuk India dan berada di bawah `client.ind.freefiremobile.com`  
[`IND`]

Parameter kueri `BR` untuk semua wilayah yang berada di bawah `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Contoh Respons Berhasil Mungkin Terlihat Seperti Ini,
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
      "COMMON_ACCEPT": "TERIMA",
      "COMMON_BACK": "Kembali",
      "COMMON_CANCEL": "Batal",
      "COMMON_CONFIRM": "Konfirmasi",
      "COMMON_CONTINUE_PURCHASE": "Lanjutkan untuk membeli",
      "COMMON_COPY": "Salin",
      "COMMON_COPY_FAILED": "Gagal menyalin",
      "COMMON_COPY_SUCCESS": "berhasil disalin",
      "COMMON_EXCHANGE": "tukar",
      "COMMON_EXCHANGED": "ditukar",
      "COMMON_FFTOKEN_HINT": "Dikonversi ke {num}{ikon token ff}",
      "COMMON_FREE": "gratis",
      "COMMON_GEM_CONFIRM": "Habiskan {cost} permata untuk membeli {NAME}?",
      "COMMON_GEM_CONFIRM2": "Habiskan {cost} permata untuk {num} putaran?",
      "COMMON_HISTORY_DRAW": "Riwayat",
      "COMMON_HISTORY_NORECORDS": "Tidak ada catatan",
      "COMMON_HISTORY_PURCHASE": "Riwayat pembelian",
      "COMMON_HISTORY_REDEEM": "Riwayat penukaran",
      "COMMON_NO": "Tidak",
      "COMMON_OWNED": "DIMILIKI",
      "COMMON_PRIZEPOOL": "Kumpulan hadiah",
      "COMMON_PURCHASE": "Beli",
      "COMMON_PURCHASED": "Dibeli",
      "COMMON_QUANTITY_MAX": "maks",
      "COMMON_REDEEM_CONFIRM": "Apakah Anda yakin untuk menukar item ini?",
      "COMMON_REJECT": "Tolak",
      "COMMON_RULE": "Aturan",
      "COMMON_SKIP": "Lewati animasi",
      "COMMON_SKIPANIMATION_TIP": "Ketuk di mana saja untuk melewati animasi",
      "COMMON_SPIN_AGAIN": "Putar Lagi",
      "COMMON_TIPS_ITEM": "Hadiah akan dikirim langsung ke brankas Anda",
      "COMMON_TIPS_TOKEN": "token telah terakumulasi secara otomatis",
      "COMMON_VISIT_GIFT": "Hadiah selamat datang",
      "COMMON_YES": "Ya",
      "POPUP_NO_REMIND": "Jangan ingatkan saya lagi",
      "POPUP_TITLE_CONGRATULATIONS": "Selamat!",
      "POPUP_TITLE_REDEEM": "Selamat! Anda mendapatkan",
      "POPUP_TITLE_UNIQUE": "Item unik yang Anda miliki",
      "UNIQUE_BUY_ALREADY_HAVE": "Anda sudah memiliki item ini, jika Anda membelinya lagi, itu akan dikonversi ke token FF",
      "UNIQUE_BUY_ALREADY_HAVE_PART": "Anda sudah memiliki beberapa item yang Anda pilih. Jika Anda menerima lagi, itu akan dikonversi ke token FF.",
      "UNIQUE_REDEEM_ALREADY_HAVE": "Anda sudah memiliki item ini, jika Anda menerimanya lagi, itu akan dikonversi ke token FF.",
      "TOAST_ERROR_CODE": "Kesalahan tidak diketahui, kode kesalahan {code}",
      "TOAST_EVENTOVER": "Acara telah berakhir",
      "TOAST_EVENT_CLOSED_AWHILE": "Acara ditutup sementara. Silakan cek lagi nanti.",
      "TOAST_EVENT_END": "Acara telah berakhir",
      "TOAST_EVENT_NOTOPEN": "Acara belum dimulai",
      "TOAST_EXCHANGE_SUCCESS": "Berhasil Ditukar",
      "TOAST_GEM_NOT_ENOUGH": "Berlian tidak cukup, silakan isi ulang dan kembali lagi",
      "TOAST_LOGIN_FAILED": "Gagal masuk",
      "TOAST_NETWORK_BUSY": "Server sibuk, silakan coba lagi nanti",
      "TOAST_NETWORK_ERROR": "Kesalahan koneksi jaringan, silakan coba lagi nanti",
      "TOAST_OPERATE_BUSY": "Terlalu banyak permintaan, silakan coba lagi nanti",
      "TOAST_PAY_FAILED": "Pembelian gagal",
      "TOAST_PURCHASE_SUCCESS": "Pembelian Berhasil",
      "TOAST_SERVER_BUSY": "Server sibuk, silakan coba lagi nanti",
      "TOAST_SERVER_NOTWORK": "Layanan tidak tersedia",
      "TOAST_SERVER_TIMEOUT": "Waktu layanan hab जन",
      "TOAST_WRONG_REGION": "Acara ini tidak tersedia untuk wilayah Anda",
      "COMMON_CALLBACK": "Bergabunglah dalam Pertarungan!",
      "COMMON_JOIN": "Gabung",
      "COMMON_SHOOT": "Ketuk pada target",
      "COMMON_SHOOT_2": "Kerja bagus! Untuk melanjutkan, silakan menuju ke Free Fire!",
      "UGC_46_MAPSHARE_GOBUTTON": "JELAJAHI LEBIH BANYAK",
      "UGC_46_MAPSHARE_PLAYBUTTON": "MAIN SEKARANG",
      "UGC_46_MAPSHARE_WRONGMESSAGE": "MAAF, PETA INI TIDAK TERSEDIA SAAT INI.",
      "UGC_47_MAPSHARE_MAPCODE": "Kode Peta",
      "UGC_47_MAPSHARE_NAME": "Nama Pembuat",
      "UGC_47_MAPSHARE_TOAST1": "Berhasil disalin",
      "UGC_47_MAPSHARE_TOAST2": "Gagal menyalin"
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

## API Daftar Keinginan Pemain
Rute API = https://free-fire-data.vercel.app/api/wishlist?region={region}&uid={uid}&key={key}

**Endpoint:** `api/wishlist`  
**Kunci:** `KUNCI-ANDA`  
**Metode:** `GET`  

Endpoint ini mengambil informasi pemain berdasarkan wilayah dan ID pengguna yang ditentukan.

### 📨 Contoh Permintaan
```http
GET https://free-fire-data.vercel.app/api/wishlist?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Parameter Kueri

| Parameter | Tipe   | Wajib | Deskripsi                            |
|-----------|--------|-------|--------------------------------------|
| `region`  | string | Ya    | Kode wilayah (`sg`, `ind`, `br`)     |
| `uid`     | int    | Ya    | ID pengguna                         |
| `key`     | string | Ya    | Beli kunci dari https://t.me/TrueClasher4 |

### ℹ️ Catatan Penting

Parameter kueri `SG` untuk semua wilayah yang berada di bawah `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Parameter kueri `IND` hanya untuk India dan berada di bawah `client.ind.freefiremobile.com`  
[`IND`]

Parameter kueri `BR` untuk semua wilayah yang berada di bawah `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Contoh Respons Berhasil Mungkin Terlihat Seperti Ini,
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

📚 **Tujuan API**

Tujuan utama dari penyediaan API gratis ini adalah untuk meningkatkan pengalaman komunitas Free Fire. Garena Free Fire tidak menawarkan API informasi akun resmi, sehingga solusi kustom ini bertujuan untuk mengisi kesenjangan tersebut, memberikan data akun yang berharga kepada pemain dan pengembang.

🧩 **(Beberapa dari🤫) Framework dan Pustaka yang Digunakan**  
- **Flask**: Framework web mikro untuk Python untuk membangun endpoint API.  
- **Flask-CORS**: Untuk menangani Cross-Origin Resource Sharing (CORS).  
- **PyCryptodome**: Untuk mengimplementasikan dekripsi dan enkripsi.  
- **Requests**: Untuk membuat permintaan HTTP ke server.

# 📁 Informasi Tambahan

- Respons API ini tidak mewakili struktur sebenarnya yang diterima dari server resmi Garena.  
- Struktur respons disederhanakan dalam struktur yang ramah pengguna untuk memudahkan pemahaman bagi siapa saja pada tingkat pemrograman apa pun.

# 😵 Respons Kesalahan
API mungkin menampilkan respons kesalahan jika permintaan pengguna tidak akurat!

### Contoh Kesalahan dan Solusi

- **Kode Kesalahan:** 400
  - **Pesan:** Wilayah tidak valid.  
  - **Solusi:** Pastikan Anda menggunakan kode wilayah yang valid.

- **Kode Kesalahan:** 429
  - **Pesan:** Permintaan tidak normal terdeteksi. Harap hindari penyalahgunaan API informasi untuk kunjungan atau IP Anda mungkin diblokir!  
  - **Solusi:** Hindari permintaan berlebihan atau hubungi penyedia API untuk bantuan.

- **Kode Kesalahan:** 500
  - **Pesan:** Terjadi kesalahan saat memproses permintaan Anda. Harap periksa kembali ID dan wilayah Anda.  
  - **Solusi:** Periksa kembali ID pengguna dan wilayah yang diberikan, lalu coba lagi. Jika masalah berlanjut, hubungi penyedia API untuk dukungan.

---

API Dibuat Oleh Sounava777,  
Semua Hak Dilindungi!
