---
layout: post
category: writing
date: 2020-05-11
title: Bạn cần Bandwidth và Disk Space bao nhiêu là đủ?
lede: Bạn có thể tự hỏi nếu 50 hoặc 100 GB băng thông là đủ cho trang web của bạn. Băng thông là tất cả về số lượng khách truy cập (lưu lượng truy cập) bạn có vào trang web của mình.
readingTime: 9
assets:
  cover: /images/psm_bandwidth.jpg
hero:
  showCover: true
  titleInvert: true
  imageBlend: 0.6
  ratio: 9/16
tags:
  - Psm
  - Web
---
**Psm thực hiện cập nhật nội dung mới nhất lúc 11/05/2020**

**99%** các trang web hiện có trên web sử dụng không quá **5 GB** băng thông mỗi tháng.

<Media ratio="844/1500" image="/images/psm_bandwidth.jpg"/>

- - -

| KÍCH THƯỚC TRANG TRUNG BÌNH | SỐ TRANG   | DUNG LƯỢNG ĐĨA CẦN THIẾT | SỐ LƯỢNG TẢI HÀNG NGÀY | SỐ LƯỢNG TẢI HÀNG THÁNG | BĂNG THÔNG CẦN THIẾT |
|-----------------------------|------------|--------------------------|------------------------|-------------------------|----------------------|
| 2 MB                        | 100        | 200 MB                   | 100                    | 3000                    | 6 GB                 |
| 2 MB                        | 500        | 1 GB                     | 500                    | 15000                   | 30 GB                |
| 2 MB                        | 1000       | 2 GB                     | 1000                   | 30000                   | 60 GB                |
| 2 MB                        | 2000       | 4 GB                     | 2000                   | 60000                   | 120 GB               |
> Psm (Phù sa mẹ) của Tiếp với địa chỉ https://phusa.me hiện tại vẫn chưa vượt qua được mốc đầu tiên 6GB dù cho đã phát triển được gần... 1 năm :D
> **Chuyện nhà Psm**.
- - -

## bảng tính toán dự phòng của Psm

Psm có phương án của riêng mình, chứ không phụ thuộc hoàn toàn vào cam kết của Nhà cung cấp Hosting. Trong đó, gói **mặc định** của Psm có Dung lượng đĩa lên tới 100 GB, và băng thông hàng tháng là 100 GB.

Dù còn sơ khai, nhưng Psm lại còn gói dự phòng cho bản thân khi gói mặc định hết băng thông, cụ thể trang Psm sẽ được chuyển manual bằng tay về gói dự phòng (Free Starter Team Plan) của Psm với dung lượng và băng thông tương đương như gói mặc định.

Và để đón trước tương lai, Psm còn chuẩn bị cho riêng mình với gói khá lớn lên đến 400 GB dung lượng và 400 GB băng thông (Open Source Plan) của mình. Đã nộp đơn đăng ký gói này kể từ 10/05/2020. Đây là bài tính đầy thận trọng cho tương lai của Psm.

| TÍNH TOÁN        | KÍCH THƯỚC TRANG | SỐ TRANG   | DUNG LƯỢNG ĐĨA | SỐ LƯỢNG TẢI HÀNG THÁNG | BĂNG THÔNG |
|------------------|------------------|------------|----------------|-------------------------|------------|
| HIỆN CÓ          | 2 MB             | 100        | 100 GB         | 30000                   | 100 GB     |
| PLAN DỰ PHÒNG    | 2 MB             | 100        | 100 GB         | 30000                   | 100 GB     |
| OPEN SOURCE PLAN | 2 MB             | 1000       | 400 GB         | 120000                  | 400 GB     |

với bài tính toán này của mình, Psm có thể **bao trọn gói** cho khách hàng thân thiết, và các bạn viếng thăm ngôi nhà Psm mà không cần lo lắng về việc Psm có thể bị tấn công hoặc hết sạch băng thông và làm gián đoạn sự yêu mến của các bạn khi viếng thăm Psm.

- - -


Băng thông không giới hạn?
Vì vậy, đừng phạm lỗi với những ưu đãi băng thông không giới hạn đó, đối với người mới bắt đầu, đó là một huyền thoại. Tất cả các nhà cung cấp dịch vụ lưu trữ web phải trả tiền cho băng thông của họ, vì vậy để cung cấp một dịch vụ không giới hạn chỉ là một cuộc nói chuyện điên rồ.

Không giới hạn, họ có nghĩa là đối với người dùng trung bình thì không giới hạn vì họ sẽ không bao giờ đạt đến giới hạn. Và đừng ngạc nhiên bởi các nhà cung cấp cung cấp tốc độ băng thông lớn, nhiều hơn không nhất thiết có nghĩa là tốt hơn. Bám sát những điều cơ bản trừ khi bạn biết trang web của bạn sẽ được hưởng nhiều lưu lượng truy cập.

Không gian đĩa không giới hạn?
Đối với không gian đĩa, điều đó thực sự phụ thuộc hoàn toàn vào nội dung trang web của bạn. Hầu hết các trang web trung bình khoảng 150 MB với một trang web chiếm khoảng 1-2 MB.

Tôi đặc biệt khuyên bạn nên chống lại các trang lớn hơn 2 MB. Chúng hoàn toàn không thực tế và do thời gian tải lâu, dẫn đến trải nghiệm người dùng xấu.

Nhiều nhà cung cấp Web Hosting sẽ cung cấp không gian đĩa không giới hạn. Theo tôi, 5 GB là quá đủ cho hầu hết các cá nhân và doanh nghiệp vừa và nhỏ.

Tuy nhiên, đáng để xem xét nội dung trang web của bạn sẽ là gì. Sẽ có quảng cáo banner, bạn sẽ có nhiều đồ họa, phương tiện video và hình ảnh? Trang web của bạn sẽ được điều khiển cơ sở dữ liệu , hoặc có phần mềm có thể tải xuống? Đối với người dùng cao cấp trung bình, 50GB thường là rất nhiều.

Trang web của bạn càng tinh vi và đa phương tiện, càng có nhiều dung lượng đĩa và có thể cần băng thông. Nhưng một lần nữa, một lời nhắc nhở, bạn không cần phải phát điên.

Tôi có thể kết hợp một máy tính trong tương lai có thể ước tính nhu cầu lưu lượng của bạn. Kiểm tra lại nếu bạn quan tâm!


Psm sẽ ghi chú lại nếu thêm nội dung được cập nhật và có ghi rõ ràng ngày giờ cập nhật {.Note}

Dữ liệu tài liệu này do Psm^1^ và KdO^2^ hợp tác trong bài viết, hỗ trợ thông tin dành cho người cùng lứa tuổi, hoàn cảnh, cùng các bạn đọc quan tâm tới Psm nội dung.^3^.

---

1. Nội dung được **Psm** chép lại khi trải đời, Kdo là tên viết tắt của Tiếp adsense và **Psm** là tên viết tắt của Psm (Phu sa me) Agency Advertising {.Note}

2. **Psm** là tên gọi Viết tắt của Phù sa mẹ. {.Note}

3. Muốn tìm bạn có cùng hoàn cảnh, lứa tuổi để học hỏi nhau trau dồi cuộc sống {.Note}

<script>
import Media from "../../src/components/Media";

export default {
  components: { Media }
}
</script>
