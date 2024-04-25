<div align="center">
  <img src="./public/header.png" alt="onedrive-cf-index-ng" />
  <h3><a href="https://pan.lyc8503.site">onedrive-cf-index-ng</a></h3>
  <p><em>OneDrive public directory listing forked from <a href="https://github.com/spencerwooo/onedrive-vercel-index">onedrive-vercel-index</a>, powered by Cloudflare and Next.js</em></p>

  <img src="https://img.shields.io/badge/OneDrive-2C68C3?style=flat&logo=microsoft-onedrive&logoColor=white" alt="OneDrive" />
  <img src="https://img.shields.io/badge/Cloudflare-f38020?style=flat&logo=Cloudflare&logoColor=white" alt="Cloudflare" />
  <img src="https://img.shields.io/badge/Next.js-black?style=flat&logo=next.js&logoColor=white" alt="Next.js" />
  <a href="https://github.com/lyc8503/onedrive-cf-index-ng/wiki"><img src="https://img.shields.io/badge/Documentation-black?style=flat&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAABmJLR0QA/wD/AP+gvaeTAAABeUlEQVRIie2VwUrDQBCGZ5ZubNmS0Ba9tF6CUqTHpg+g+AhCn8R30DfpM3jRezdHoZJroaBJQ2qgsIEdD7YSsCtJVBTxP87u/t/u7M4swDcLTQNSSseyLFbERCmlPc9LCgF83z/jnE9s294vvk+AJEmesiwbe553awQEQbCXZVnY7/ebjBXa/Ju01jCbzVIA6AwGA7WN1/KT4jg+6vV6TcYYpGlKq9UKiQgAAOr1OnU6HWNKGWPQarWa8/n8GADudwIQ0UJ89QjDEKMoOiEitRm7tm37gnNuPAUiAiJa+VjNNJmIYDgcPiAiAQD4vh9tT1NG5RJdQT8PkFKak/5ZgJTyUgjxPJ1Ob4josArAeMmWZYHrulftdhvX6/X5YrEwPtFKgG63C7ApxEajga7rVvH/BZf8D/hjACJSVRpabj1su+9OgBAiiOM41VqXNtdaw3K5TIUQQT7+rjqllKec84njOAdlAEmSPCqlxqPR6O5DQA70JZ/+t+sFAb2R22dSZ7wAAAAASUVORK5CYII=" alt="Documentation" /></a>
</div>


## Demo

Live demo at [lyc8503's Fileshare](https://pan.lyc8503.site).

![demo](./public/demo.png)

---

> [!NOTE]
> Đây là hướng dẫn config và setup bằng tiếng việt bởi mod voz4rum
>
> This is configuration and setup instructions with Vietnamese by mod voz4rum 

> [!WARNING]
> Bài hướng dẫn dưới đây đã được viết khá lâu nên có thể hơi khác một chút để thực tế
>
> The instructions below were written a long time ago, so they may be a little different from reality

## Giới thiệu:
- Tính năng:
    - Direct link tất cả các file trong onedrive.
    - Xem trực tiếp tất cả các file video, nhạc, ảnh, ebook, pdf, office...
    - Có preview ảnh, video, pdf...
    - Tải nhiều file/thư một cùng lúc.
    - Có nút phát video thông qua VLC, Potplayer...
    - Có dark mode.
    - Các tính năng trên đều tương thích với điện thoại, tv...
    - Không cần tốn công đăng nhập khi vào trên thiết bị khác.
    - Hoàn toàn miễn phí.

Hướng dẫn bằng tiếng anh cho ai cần thêm thông tin chi tiết hơn:
https://github.com/lyc8503/onedrive-cf-index-ng/wiki

## Chuẩn bị
 
 Tài khoản onedrive: Nếu là tài khoản edu, E5 (dev), office 365 family... thì phải có tài khoản quyền admin của cái nhóm ấy, hoặc quen biết với admin của nhóm ấy nhờ họ giúp, kéo xuống mục E đăng nhập để xem thêm.
 Tài khoản E5 thì hoàn toàn miễn phí, lại có sẵn luôn quyền admin, có thể tham khảo thread này: [Đăng ký Microsoft 365 developer E5 miễn phí dùng thử 90 ngày tự động gia hạn khi còn kích hoạt](https://voz.vn/t/dang-ky-microsoft-365-developer-e5-mien-phi-dung-thu-90-ngay-tu-dong-gia-han-khi-con-kich-hoat.407602/)

 Đăng ký tài khoản cloudflare (nếu chưa có)
https://dash.cloudflare.com/

Fork lại project này trên github
https://github.com/lyc8503/onedrive-cf-index-ng

![img](https://voz.vn/proxy.php?image=https%3A%2F%2Fi.imgur.com%2FDj3x1P0.png&hash=e800cab4cad0dbab64787aba0f7ab5f2)

## Cài đặt trên github:
(Bước này để cá nhân hóa, nếu như thích để mặc định thì bỏ qua)

Vào project đã fork > Vào folder **Config** > **site.config.js** > bấm vào đây để edit file

![img](https://voz.vn/proxy.php?image=https%3A%2F%2Fi.imgur.com%2FrHJ4M3a.png&hash=6e10520682eb6607f8629f372a1ebcce)

Bây giờ chỉnh sửa file config này theo ý thích từng dòng sau, t chỉ hướng dẫn mấy cái nào cơ bản thôi, cái nào ko cần thiết quá thì đọc phần note englisk để tìm hiểu thêm:
`title: "Spencer's OneDrive"` Là tên website ở góc trái trên cùng vd: `title: "Fioren",`

![img](https://voz.vn/proxy.php?image=https%3A%2F%2Fi.imgur.com%2FNHvXLgO.png&hash=0d9de4671907f9c27bc6902e189d0523)

`baseDirectory: '/',` Là folder trong onedrive để đưa lên Web UI, nếu muốn đưa tất cả trong tài khoản thì giữ nguyên, không thì thêm vào vd như `/FolderA/FolderB`. Lưu ý phải là đường dẫn tới folder đã có sẵn trong onedrive, folder không nên có dấu tiếng việt, khoảng cách, kí tự đặc biệt...
`footer: 'Powered by <a href="https://github.com/spencerwooo/onedrive-vercel-index" target="_blank" ....` Dòng này là để quảng cáo, xóa đi cho đỡ tốn chỗ. bằng cách xóa toàn bộ 2 dòng này.

`protectedRoutes: ['/Private folder/u-need-a-password', '/Some test files/Protected route'],` Dùng để đặt password cho folder. VD: Folder cần đặt pass là: `/My` => code là

```
"protectedRoutes": [
  '/My',
],
```

Sau đó vào notepad tạo 1 file tên là `.password` nội dung là cái password cần đặt (lưu ý password 6 ký tự trở lên), sau đó upload vào trong cái folder `My` trên onedrive

`email: 'mailto:spencer.wushangbo@gmail.com',` xóa đi cho đỡ tốn chỗ sửa thành `email: '',`

 `datetimeFormat: 'YYYY-MM-DD HH:mm:ss',` sửa thành  `datetimeFormat: 'DD-MM-YYYY HH:mm:ss',` cho hợp định dạng thời gian ở VN

Sau khi sửa xong, kéo xuống dưới bấm nút **Commit changes**

## Deloy
Vào đây
https://dash.cloudflare.com/?to=/:account/workers

![img](https://voz.vn/proxy.php?image=https%3A%2F%2Fi.imgur.com%2FdiBJHxt.png&hash=dfda0a91eaf8c58b52f90bb81c82a87a)

Rồi đăng nhập vào tài khoản github, cấp quyền cho app cloudflare để đọc được các repo.
Sau khi cấp quyền xong thì chọn repo `onedrive-cf-index-ng` trong danh sách rồi bấm `Begin Setup`
Ở bước tiếp theo chọn `Framework preset` là `Next.js`:

![img](https://voz.vn/proxy.php?image=https%3A%2F%2Fi.imgur.com%2FTDqXQk1.png&hash=6e5ff14ab7fbcd82240f450aea120cc1)

Rối bấm `Save and Deploy` chờ cho khi nó Build xong, thì ấn **Continue to project**.

Rồi vào **Settings** > **Functions** > **Compatibility flags** điền vào `nodejs_compat` rồi bấm Save

Sau đó mở tab khác vào đây, tạo một cái KV với tên tùy thích:

![img](https://voz.vn/proxy.php?image=https%3A%2F%2Fi.imgur.com%2F0K1A94o.png&hash=ffdce5104da42eae4f99390db16eee76)

Quay trở lại mục **Settings** > **Functions** ở bước trên, kéo xuống mục `KV namespace bindings` bấm `Add binding`

`KV namespace` chọn cái KV vừa mới tạo `Variable name` điền `ONEDRIVE_CF_INDEX_KV` rồi bấm **Save**

![img](https://voz.vn/proxy.php?image=https%3A%2F%2Fi.imgur.com%2FXSSaqzc.png&hash=3ea5d23ab6bf70ed839837d2f84eb3fc)

Vào **Settings** > **Environment variables** > tạo **Variable name** là `USER_PRINCIPLE_NAME`, value địa chỉ Email account admin microsoft

![img](https://voz.vn/proxy.php?image=https%3A%2F%2Fi.imgur.com%2FJei1rP1.png&hash=eb341917cb2adf959df88f0f96b47726)

Sau đó chọn tab **Deployment** > **Retry Deployment** và chờ đến khi xong.

![img](https://voz.vn/proxy.php?image=https%3A%2F%2Fi.imgur.com%2Fpl4oSAW.png&hash=bb6706aa252932cc8740e971cbb93957)

## Đăng nhập
Vào domain này:

![img](https://voz.vn/proxy.php?image=https%3A%2F%2Fi.imgur.com%2Fs0IaCQI.png&hash=506625c6baa3a3f75d38f1288a81e4c9)

Rồi bấm **Proceed to OAuth**

![img](https://voz.vn/proxy.php?image=https%3A%2F%2Fi.imgur.com%2FNbO2DL9.png&hash=c5617035fc57cd59a9a5a1a74d95511a)

Sau đó bấm vào link này

![img](https://voz.vn/proxy.php?image=https%3A%2F%2Fi.imgur.com%2FoXN7Ynk.png&hash=e05e12b1e542ad65c53b909e1cd513c9)

Đăng nhập các kiểu, chấp nhận app các kiểu blabla. Lưu ý: Nếu như bạn chỉ là thành viên trong nhóm onedrive không phải là admin thì nhờ admin vào link đó, bấm đồng ý cho app đó và chọn **"Thay mặt cho tổ chức"**. Rồi vào account của mình kích hoạt bình thường các bước tiếp theo.

![img](https://voz.vn/proxy.php?image=https%3A%2F%2Fi.imgur.com%2FXfXEpz5.png&hash=e3351c0fe0bbe35d65d463abb7bea00a)

Sau khi đăng nhập xong nó sẽ mở ra 1 popup, copy link này ở thanh địa chỉ

![img](https://voz.vn/proxy.php?image=https%3A%2F%2Fi.imgur.com%2FbgZ50fF.png&hash=e1f262cb55b24111f7782cf5eefc37e3)

![img](https://voz.vn/proxy.php?image=https%3A%2F%2Fi.imgur.com%2FUOhMzKD.png&hash=fa10c0b6fe5d7c200c2e2254d0ead021)

Bấm **Get tokens** > **Store tokens**
Vậy là xong vào lại domain vừa tạo bước trên và thưởng thức.

Lâu lâu nhớ vào project github bấm vào nút này để update phiên bản mới nhé. Chỉ cần ấn là đủ, không cần làm gì hết vercel sẽ tự động deploy

![img](https://voz.vn/proxy.php?image=https%3A%2F%2Fi.imgur.com%2FhZdXRch.png&hash=94b86cd0cb595f0c0a94285bfb7589b9)



