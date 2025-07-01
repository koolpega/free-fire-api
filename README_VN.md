# 📝 Tài liệu API

## API Thông tin Người chơi
Đường dẫn API = https://free-fire-data.vercel.app/api/data?region={region}&uid={uid}&key={key}

**Điểm cuối:** `api/data`  
**Khóa:** `KHÓA-CỦA-BẠN`  
**Phương thức:** `GET`  

Điểm cuối này lấy thông tin người chơi dựa trên khu vực và ID người dùng được chỉ định.

### 📨 Ví dụ Yêu cầu
```http
GET https://free-fire-data.vercel.app/api/data?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Tham số Truy vấn

| Tham số   | Kiểu   | Bắt buộc | Mô tả                                |
|-----------|--------|----------|--------------------------------------|
| `region`  | chuỗi  | Có       | Mã khu vực (`sg`, `ind`, `br`)       |
| `uid`     | số nguyên | Có     | ID người dùng                        |
| `key`     | chuỗi  | Có       | Mua khóa từ https://t.me/TrueClasher4 |

### ℹ️ Lưu ý Quan trọng

Tham số truy vấn `SG` dành cho tất cả các khu vực thuộc `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Tham số truy vấn `IND` chỉ dành cho Ấn Độ và thuộc `client.ind.freefiremobile.com`  
[`IND`]

Tham số truy vấn `BR` dành cho tất cả các khu vực thuộc `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Ví dụ về Phản hồi Thành công Có thể Trông Như Sau,
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

## API Thống kê Người chơi
Đường dẫn API = https://free-fire-data.vercel.app/api/stats?region={region}&uid={uid}&key={key}

**Điểm cuối:** `api/stats`  
**Khóa:** `KHÓA-CỦA-BẠN`  
**Phương thức:** `GET`  

Điểm cuối này lấy thông tin thống kê người chơi dựa trên khu vực và ID người dùng được chỉ định.

### 📨 Ví dụ Yêu cầu
```http
GET https://free-fire-data.vercel.app/api/stats?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Tham số Truy vấn

| Tham số   | Kiểu   | Bắt buộc | Mô tả                                |
|-----------|--------|----------|--------------------------------------|
| `region`  | chuỗi  | Có       | Mã khu vực (`sg`, `ind`, `br`)       |
| `uid`     | số nguyên | Có     | ID người dùng                        |
| `key`     | chuỗi  | Có       | Mua khóa từ https://t.me/TrueClasher4 |

### ℹ️ Lưu ý Quan trọng

Tham số truy vấn `SG` dành cho tất cả các khu vực thuộc `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Tham số truy vấn `IND` chỉ dành cho Ấn Độ và thuộc `client.ind.freefiremobile.com`  
[`IND`]

Tham số truy vấn `BR` dành cho tất cả các khu vực thuộc `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Ví dụ về Phản hồi Thành công Có thể Trông Như Sau,
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

## API Lượt thích
Đường dẫn API = https://free-fire-data.vercel.app/api/like?region={region}&uid={uid}&key={key}

**Điểm cuối:** `api/like`  
**Khóa:** `KHÓA-CỦA-BẠN`  
**Phương thức:** `GET`  

Điểm cuối này gửi 100 lượt thích đến tài khoản người chơi dựa trên khu vực và ID người dùng được chỉ định.

### 📨 Ví dụ Yêu cầu
```http
GET https://free-fire-data.vercel.app/api/like?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Tham số Truy vấn

| Tham số   | Kiểu   | Bắt buộc | Mô tả                                |
|-----------|--------|----------|--------------------------------------|
| `region`  | chuỗi  | Có       | Mã khu vực (`sg`, `ind`, `br`)       |
| `uid`     | số nguyên | Có     | ID người dùng                        |
| `key`     | chuỗi  | Có       | Mua khóa từ https://t.me/TrueClasher4 |

### ℹ️ Lưu ý Quan trọng

Tham số truy vấn `SG` dành cho tất cả các khu vực thuộc `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Tham số truy vấn `IND` chỉ dành cho Ấn Độ và thuộc `client.ind.freefiremobile.com`  
[`IND`]

Tham số truy vấn `BR` dành cho tất cả các khu vực thuộc `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Ví dụ về Phản hồi Thành công Có thể Trông Như Sau,
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

## API Lượt truy cập
Đường dẫn API = https://free-fire-data.vercel.app/api/visit?region={region}&uid={uid}&key={key}

**Điểm cuối:** `api/visit`  
**Khóa:** `KHÓA-CỦA-BẠN`  
**Phương thức:** `GET`  

Điểm cuối này gửi 100 lượt truy cập đến tài khoản người chơi dựa trên khu vực và ID người dùng được chỉ định.

### 📨 Ví dụ Yêu cầu
```http
GET https://free-fire-data.vercel.app/api/visit?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Tham số Truy vấn

| Tham số   | Kiểu   | Bắt buộc | Mô tả                                |
|-----------|--------|----------|--------------------------------------|
| `region`  | chuỗi  | Có       | Mã khu vực (`sg`, `ind`, `br`)       |
| `uid`     | số nguyên | Có     | ID người dùng                        |
| `key`     | chuỗi  | Có       | Mua khóa từ https://t.me/TrueClasher4 |

### ℹ️ Lưu ý Quan trọng

Tham số truy vấn `SG` dành cho tất cả các khu vực thuộc `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Tham số truy vấn `IND` chỉ dành cho Ấn Độ và thuộc `client.ind.freefiremobile.com`  
[`IND`]

Tham số truy vấn `BR` dành cho tất cả các khu vực thuộc `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Ví dụ về Phản hồi Thành công Có thể Trông Như Sau,
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
Đường dẫn API = https://free-fire-data.vercel.app/api/spam?region={region}&uid={uid}&key={key}

**Điểm cuối:** `api/spam`  
**Khóa:** `KHÓA-CỦA-BẠN`  
**Phương thức:** `GET`  

Điểm cuối này gửi 100 yêu cầu kết bạn đến tài khoản người chơi dựa trên khu vực và ID người dùng được chỉ định.

### 📨 Ví dụ Yêu cầu
```http
GET https://free-fire-data.vercel.app/api/spam?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Tham số Truy vấn

| Tham số   | Kiểu   | Bắt buộc | Mô tả                                |
|-----------|--------|----------|--------------------------------------|
| `region`  | chuỗi  | Có       | Mã khu vực (`sg`, `ind`, `br`)       |
| `uid`     | số nguyên | Có     | ID người dùng                        |
| `key`     | chuỗi  | Có       | Mua khóa từ https://t.me/TrueClasher4 |

### ℹ️ Lưu ý Quan trọng

Tham số truy vấn `SG` dành cho tất cả các khu vực thuộc `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Tham số truy vấn `IND` chỉ dành cho Ấn Độ và thuộc `client.ind.freefiremobile.com`  
[`IND`]

Tham số truy vấn `BR` dành cho tất cả các khu vực thuộc `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Ví dụ về Phản hồi Thành công Có thể Trông Như Sau,
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

## API Hình ảnh
Đường dẫn API = https://free-fire-data.vercel.app/api/images?iconName={iconName}&key={key}

**Điểm cuối:** `api/images`  
**Khóa:** `KHÓA-CỦA-BẠN`  
**Phương thức:** `GET`  

Điểm cuối này lấy thông tin người chơi dựa trên khu vực và ID người dùng được chỉ định.

### 📨 Ví dụ Yêu cầu
```http
GET https://free-fire-data.vercel.app/api/images?iconName=Icon_avatar_hair_cos_eggday2021_headwear_blue&key=KEY123
```

### ☑️ Tham số Truy vấn

| Tham số    | Kiểu   | Bắt buộc | Mô tả                                |
|------------|--------|----------|--------------------------------------|
| `iconName` | chuỗi  | Có       | Tên của biểu tượng.                  |
| `key`      | chuỗi  | Có       | Mua khóa từ https://t.me/TrueClasher4 |

### 💬 Ví dụ về Phản hồi Thành công Có thể Trông Như Sau,

![Icon_avatar_hair_cos_eggday2021_headwear_blue](https://github.com/realpega/free-fire-api/blob/main/images.png)

## API Thông tin Bản đồ Craftland
Đường dẫn API = https://free-fire-data.vercel.app/api/maps?region={region}&code=%23{CODE}&key={key}

**Điểm cuối:** `api/maps`  
**Khóa:** `KHÓA-CỦA-BẠN`  
**Phương thức:** `GET`  

Điểm cuối này lấy thông tin người chơi dựa trên khu vực và ID người dùng được chỉ định.

### 📨 Ví dụ Yêu cầu
```http
GET https://free-fire-data.vercel.app/api/maps?region=sg&code=%23FREEFIREMAPCODE6969&key=KEY123
```

### ☑️ Tham số Truy vấn

| Tham số   | Kiểu   | Bắt buộc | Mô tả                                |
|-----------|--------|----------|--------------------------------------|
| `region`  | chuỗi  | Có       | Mã khu vực (`sg`, `ind`, `br`)       |
| `uid`     | số nguyên | Có     | ID người dùng                        |
| `key`     | chuỗi  | Có       | Mua khóa từ https://t.me/TrueClasher4 |

### ℹ️ Lưu ý Quan trọng

Tham số truy vấn `SG` dành cho tất cả các khu vực thuộc `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Tham số truy vấn `IND` chỉ dành cho Ấn Độ và thuộc `client.ind.freefiremobile.com`  
[`IND`]

Tham số truy vấn `BR` dành cho tất cả các khu vực thuộc `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Ví dụ về Phản hồi Thành công Có thể Trông Như Sau,
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
      "COMMON_ACCEPT": "CHẤP NHẬN",
      "COMMON_BACK": "Quay lại",
      "COMMON_CANCEL": "Hủy",
      "COMMON_CONFIRM": "Xác nhận",
      "COMMON_CONTINUE_PURCHASE": "Tiếp tục mua",
      "COMMON_COPY": "Sao chép",
      "COMMON_COPY_FAILED": "Sao chép thất bại",
      "COMMON_COPY_SUCCESS": "sao chép thành công",
      "COMMON_EXCHANGE": "đổi",
      "COMMON_EXCHANGED": "đã đổi",
      "COMMON_FFTOKEN_HINT": "Đã chuyển đổi thành {num}{biểu tượng token ff}",
      "COMMON_FREE": "miễn phí",
      "COMMON_GEM_CONFIRM": "Chi tiêu {cost} viên ngọc để mua {NAME}?",
      "COMMON_GEM_CONFIRM2": "Chi tiêu {cost} viên ngọc cho {num} lần quay?",
      "COMMON_HISTORY_DRAW": "Lịch sử",
      "COMMON_HISTORY_NORECORDS": "Không có bản ghi",
      "COMMON_HISTORY_PURCHASE": "Lịch sử mua hàng",
      "COMMON_HISTORY_REDEEM": "Lịch sử đổi thưởng",
      "COMMON_NO": "Không",
      "COMMON_OWNED": "ĐÃ SỞ HỮU",
      "COMMON_PRIZEPOOL": "Nhóm phần thưởng",
      "COMMON_PURCHASE": "Mua",
      "COMMON_PURCHASED": "Đã mua",
      "COMMON_QUANTITY_MAX": "tối đa",
      "COMMON_REDEEM_CONFIRM": "Bạn có chắc chắn muốn đổi vật phẩm này không?",
      "COMMON_REJECT": "Từ chối",
      "COMMON_RULE": "Quy tắc",
      "COMMON_SKIP": "Bỏ qua hoạt ảnh",
      "COMMON_SKIPANIMATION_TIP": "Chạm vào bất kỳ đâu để bỏ qua hoạt ảnh",
      "COMMON_SPIN_AGAIN": "Quay lại",
      "COMMON_TIPS_ITEM": "Phần thưởng sẽ được gửi trực tiếp đến kho của bạn",
      "COMMON_TIPS_TOKEN": "token đã được tích lũy tự động",
      "COMMON_VISIT_GIFT": "Quà chào mừng",
      "COMMON_YES": "Có",
      "POPUP_NO_REMIND": "Đừng nhắc tôi lần nữa",
      "POPUP_TITLE_CONGRATULATIONS": "Chúc mừng!",
      "POPUP_TITLE_REDEEM": "Chúc mừng! Bạn đã nhận được",
      "POPUP_TITLE_UNIQUE": "Các vật phẩm độc đáo bạn sở hữu",
      "UNIQUE_BUY_ALREADY_HAVE": "Bạn đã sở hữu vật phẩm này, nếu mua lại, nó sẽ được chuyển đổi thành token FF",
      "UNIQUE_BUY_ALREADY_HAVE_PART": "Bạn đã sở hữu một số vật phẩm bạn đã chọn. Nếu nhận lại, nó sẽ được chuyển đổi thành token FF.",
      "UNIQUE_REDEEM_ALREADY_HAVE": "Bạn đã sở hữu vật phẩm này, nếu nhận lại, nó sẽ được chuyển đổi thành token FF.",
      "TOAST_ERROR_CODE": "Lỗi không xác định, mã lỗi {code}",
      "TOAST_EVENTOVER": "Sự kiện đã kết thúc",
      "TOAST_EVENT_CLOSED_AWHILE": "Sự kiện tạm thời đóng. Vui lòng kiểm tra lại sau.",
      "TOAST_EVENT_END": "Sự kiện đã kết thúc",
      "TOAST_EVENT_NOTOPEN": "Sự kiện chưa bắt đầu",
      "TOAST_EXCHANGE_SUCCESS": "Đổi thành công",
      "TOAST_GEM_NOT_ENOUGH": "Không đủ kim cương, vui lòng nạp thêm và quay lại",
      "TOAST_LOGIN_FAILED": "Đăng nhập thất bại",
      "TOAST_NETWORK_BUSY": "Máy chủ bận, vui lòng thử lại sau",
      "TOAST_NETWORK_ERROR": "Lỗi kết nối mạng, vui lòng thử lại sau",
      "TOAST_OPERATE_BUSY": "Quá nhiều yêu cầu, vui lòng thử lại sau",
      "TOAST_PAY_FAILED": "Mua hàng thất bại",
      "TOAST_PURCHASE_SUCCESS": "Mua hàng thành công",
      "TOAST_SERVER_BUSY": "Máy chủ bận, vui lòng thử lại sau",
      "TOAST_SERVER_NOTWORK": "Dịch vụ không khả dụng",
      "TOAST_SERVER_TIMEOUT": "Hết thời gian dịch vụ",
      "TOAST_WRONG_REGION": "Sự kiện này không khả dụng cho khu vực của bạn",
      "COMMON_CALLBACK": "Tham gia Chiến đấu!",
      "COMMON_JOIN": "Tham gia",
      "COMMON_SHOOT": "Chạm vào các mục tiêu",
      "COMMON_SHOOT_2": "Tốt lắm! Để tiếp tục, vui lòng đến với Free Fire!",
      "UGC_46_MAPSHARE_GOBUTTON": "KHÁM PHÁ THÊM",
      "UGC_46_MAPSHARE_PLAYBUTTON": "CHƠI NGAY",
      "UGC_46_MAPSHARE_WRONGMESSAGE": "XIN LỖI, BẢN ĐỒ NÀY HIỆN KHÔNG CÓ SẴN.",
      "UGC_47_MAPSHARE_MAPCODE": "Mã Bản đồ",
      "UGC_47_MAPSHARE_NAME": "Tên Người tạo",
      "UGC_47_MAPSHARE_TOAST1": "Sao chép thành công",
      "UGC_47_MAPSHARE_TOAST2": "Sao chép thất bại"
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

## API Danh sách Mong muốn Người chơi
Đường dẫn API = https://free-fire-data.vercel.app/api/wishlist?region={region}&uid={uid}&key={key}

**Điểm cuối:** `api/wishlist`  
**Khóa:** `KHÓA-CỦA-BẠN`  
**Phương thức:** `GET`  

Điểm cuối này lấy thông tin người chơi dựa trên khu vực và ID người dùng được chỉ định.

### 📨 Ví dụ Yêu cầu
```http
GET https://free-fire-data.vercel.app/api/wishlist?region=ind&uid=2180732447&key=KEY123
```

### ☑️ Tham số Truy vấn

| Tham số   | Kiểu   | Bắt buộc | Mô tả                                |
|-----------|--------|----------|--------------------------------------|
| `region`  | chuỗi  | Có       | Mã khu vực (`sg`, `ind`, `br`)       |
| `uid`     | số nguyên | Có     | ID người dùng                        |
| `key`     | chuỗi  | Có       | Mua khóa từ https://t.me/TrueClasher4 |

### ℹ️ Lưu ý Quan trọng

Tham số truy vấn `SG` dành cho tất cả các khu vực thuộc `clientbp.ggblueshark.com`  
[`SG`, `ID`, `ME`, `VN`, `TH`, `CIS`, `EU`, `TW`, `MY`, `PK`, `BD`]

Tham số truy vấn `IND` chỉ dành cho Ấn Độ và thuộc `client.ind.freefiremobile.com`  
[`IND`]

Tham số truy vấn `BR` dành cho tất cả các khu vực thuộc `client.us.freefiremobile.com`  
[`BR`, `US`, `NA`, `LATAM`]

### 💬 Ví dụ về Phản hồi Thành công Có thể Trông Như Sau,
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

📚 **Mục đích của API**

Mục đích chính của việc cung cấp API miễn phí này là để nâng cao trải nghiệm cộng đồng Free Fire. Garena Free Fire không cung cấp API thông tin tài khoản chính thức, vì vậy giải pháp tùy chỉnh này nhằm lấp đầy khoảng trống đó, cung cấp dữ liệu tài khoản có giá trị cho người chơi và nhà phát triển.

🧩 **(Một số🤫) Framework và Thư viện Được Sử dụng**  
- **Flask**: Một framework web nhỏ cho Python để xây dựng các điểm cuối API.  
- **Flask-CORS**: Để xử lý Chia sẻ Tài nguyên Chéo Nguồn (CORS).  
- **PyCryptodome**: Để triển khai giải mã và mã hóa.  
- **Requests**: Để thực hiện các yêu cầu HTTP đến máy chủ.

# 📁 Thông tin Bổ sung

- Phản hồi API này không đại diện cho cấu trúc thực tế nhận được từ máy chủ Garena chính thức.  
- Cấu trúc phản hồi được đơn giản hóa trong một cấu trúc thân thiện với người dùng để dễ hiểu cho bất kỳ ai ở bất kỳ cấp độ lập trình nào.

# 😵 Phản hồi Lỗi
API có thể hiển thị phản hồi lỗi nếu yêu cầu của người dùng không chính xác!

### Các Trường hợp Lỗi và Giải pháp

- **Mã Lỗi:** 400
  - **Thông báo:** Khu vực không hợp lệ.  
  - **Giải pháp:** Đảm bảo bạn đang sử dụng mã khu vực hợp lệ.

- **Mã Lỗi:** 429
  - **Thông báo:** Phát hiện yêu cầu bất thường. Vui lòng tránh lạm dụng API thông tin cho các lượt truy cập hoặc IP của bạn có thể bị chặn!  
  - **Giải pháp:** Tránh gửi quá nhiều yêu cầu hoặc liên hệ với nhà cung cấp API để được hỗ trợ.

- **Mã Lỗi:** 500
  - **Thông báo:** Đã xảy ra lỗi trong khi xử lý yêu cầu của bạn. Vui lòng kiểm tra lại ID và khu vực của bạn.  
  - **Giải pháp:** Kiểm tra kỹ lại ID người dùng và khu vực được cung cấp, sau đó thử lại yêu cầu. Nếu vấn đề vẫn tiếp diễn, liên hệ với nhà cung cấp API để được hỗ trợ.

---

API Được Tạo Bởi Sounava777,  
Mọi Quyền Được Bảo Lưu!
