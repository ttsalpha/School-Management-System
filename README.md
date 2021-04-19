# Website quản lý học đường

## Mục đích

Hỗ trợ giáo viên trong việc quản lý và lưu trữ thông tin của học sinh một cách dễ dàng, thuận tiện.

## Phạm vi và đối tượng

Trường Tiểu học (~500 học sinh).\
Dành cho giáo viên chủ nhiệm và ban giám hiệu nhà trường.

## Chức năng

- Đăng ký tài khoản cho giáo viên (chủ nhiệm) và ban giám hiệu.
- Đăng nhập, đăng xuất.
- Quản lý hồ sơ học sinh.
- Quản lý thông tin chung của lớp học.
- Quản lý điểm số, học lực các môn.
- Đánh giá học sinh, nhận xét.
- Khen thưởng, xếp loại.

## Công nghệ sử dụng

- Server Backend: Nodejs Express
- App Frontend: Reactjs
- Database: MySQL server

## Bản demo heroku

Truy cập: https://thaobone.herokuapp.com

|    role    |    username   |  password |
|:----------:|:-------------:|:---------:|
|   member   |      bone     |    jack   |
|   admin    |    president  | president |

## Các thư mục phát triển của Website

- Report repository: [SMS - Report](https://github.com/ttsalpha/school-management-system)
- Front end repository: [SMS - Client](https://github.com/ttsalpha/school-management-system-client)
- Back end repository: [SMS - Server](https://github.com/ttsalpha/school-management-system-server)

## Hướng dẫn cài đặt

- Back end: clone SMS - Server -> `yarn install` -> `yarn dev`
- Front end: clone SMS - Client -> `yarn install` -> `yarn start`

```js
// Đi đến file Misc.js trong src của front end, chọn server cần kết nối:
export const api = axios.create(({
// chọn một trong hai baseURL
  baseURL: 'http://localhost:3001/', // kết nối với sms server tại local
  baseURL: 'https://thaobone-server.herokuapp.com/' // mặc định kết nối heroku
}))
```

## Nhóm phát triển

- [Bùi Thị Phương Thảo](https://github.com/thaobone163)
- [Trần Thế Sơn](https://github.com/ttsalpha)

## Lược đồ quan hệ thực thể

![](./entity–relationship.png)