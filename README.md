# [IT-206-K25] Bài 2 - Session 6: Xây dựng Prioritized Product Backlog bằng kỹ thuật MoSCoW

> 👤 **Học viên:** Đỗ Hoàng Sơn | **Mã SV:** PTIT-HCM-066
> 🏫 **Môn học:** IT206-K25-Agile-va-Scrum

---

## Nhiệm vụ 1: Phân loại 12 hạng mục theo MoSCoW và giải thích lý do

Với vai trò là Product Owner của hệ thống mượn sách online (Release 1 - MVP), tôi đã phân loại 12 hạng mục backlog dựa trên giá trị cốt lõi, mức độ phụ thuộc kỹ thuật và năng lực của nhóm (20 điểm). Dưới đây là bảng phân loại chi tiết đi kèm lý do cho từng hạng mục:

- Đăng nhập/đăng ký tài khoản độc giả: Must have - Lý do: Là nền tảng bắt buộc để xác thực danh tính người dùng trước khi thực hiện bất kỳ giao dịch mượn sách nào.
- Tìm kiếm sách theo tên/tác giả: Must have - Lý do: Chức năng cốt lõi giúp độc giả tiếp cận danh mục tài nguyên của thư viện, thiếu nó thì hệ thống không có giá trị sử dụng.
- Mượn sách online (có giới hạn số sách mượn cùng lúc): Should have - Lý do: Rất quan trọng nhưng giai đoạn đầu có thể xử lý thủ công tại quầy hoặc giới hạn cứng, tuy nhiên vẫn đưa vào sát MVP nhờ điểm số vừa phải.
- Gia hạn mượn sách online: Could have - Lý do: Tiện ích gia tăng, nếu chưa kịp làm thì độc giả có thể đến trực tiếp thư viện hoặc gọi điện gia hạn.
- Đặt trước sách khi hết (kèm thông báo khi sách có sẵn): Must have - Lý do: Giải quyết bài toán nghiệp vụ thiết yếu khi sách phổ thông hết lượt, tạo trải nghiệm xuyên suốt cho độc giả.
- Đánh giá & bình luận sách sau khi đọc: Could have - Lý do: Tính năng cộng đồng mang tính chất bổ trợ, không ảnh hưởng trực tiếp đến luồng mượn/trả sách cốt lõi của MVP.
- Gợi ý sách theo sở thích cá nhân (recommendation): Won't have (this time) - Lý do: Thuộc về nâng cấp AI/Data ở các phiên bản sau, tốn nhiều công sức (3 điểm) và không cấp bách cho MVP.
- Thông báo email khi sắp đến hạn trả sách: Should have - Lý do: Giúp giảm tỷ lệ trả sách muộn, tuy nhiên có thể dùng hình thức nhắc nhở thủ công hoặc bỏ qua tạm thời ở tuần đầu phát hành.
- Xem lịch sử mượn sách của bản thân: Should have - Lý do: Mang lại giá trị minh bạch cho độc giả nhưng không chặn luồng mượn sách chính nếu chưa hoàn thiện.
- Thủ thư quản lý kho sách (thêm/sửa/xóa sách): Must have - Lý do: Thiếu giao diện quản trị kho của thủ thư thì hệ thống không có dữ liệu sách để độc giả tìm kiếm và mượn.
- Chat trực tiếp với thủ thư: Won't have (this time) - Lý do: Chi phí công sức cao (3 điểm) và đòi hỏi hạ tầng thời gian thực phức tạp, nên hoãn lại cho Release 2.
- Tích hợp đăng nhập bằng Google/Facebook: Could have - Lý do: Tiện ích đăng nhập nhanh, nhưng đăng nhập bằng tài khoản nội bộ (Mục 1) đã đủ đáp ứng cho MVP.

## Nhiệm vụ 2: Tính tổng điểm công sức nhóm Must và đánh giá ngưỡng năng lực

Dựa trên kích thước công sức đã quy ước (S = 1 điểm, M = 2 điểm, L = 3 điểm), ta tính tổng điểm cho nhóm Must have như sau:

- Tổng số lượng hạng mục nhóm Must: 4 mục (đáp ứng ràng buộc không vượt quá 5 hạng mục).
- Tổng điểm công sức nhóm Must: 2 + 2 + 2 + 3 = 9 điểm.
- Đánh giá so với ngưỡng: Năng lực của nhóm cho Release 1 là khoảng 20 điểm. Ngưỡng 60% năng lực tương đương 12 điểm. Tổng 9 điểm của nhóm Must nằm thấp hơn ngưỡng 60% một chút, cho thấy nhóm có độ an toàn cao, chừa dư địa lớn để xử lý rủi ro kỹ thuật hoặc gánh thêm các mục Should have trong sprint.

| Mã mục | Tên hạng mục | Kích thước công sức | Nhóm MoSCoW |
| --- | --- | --- | --- |
| 1 | Đăng nhập/đăng ký tài khoản độc giả | 2 điểm (M) | Must have |
| 2 | Tìm kiếm sách theo tên/tác giả | 2 điểm (M) | Must have |
| 5 | Đặt trước sách khi hết | 2 điểm (M) | Must have |
| 10 | Thủ thư quản lý kho sách | 3 điểm (L) | Must have |

## Nhiệm vụ 3: Sắp xếp Product Backlog có thứ tự từ 1 đến 12

Dựa trên nguyên tắc: Nhóm Must đứng đầu, tiếp theo là Should, Could, và cuối cùng là Won't; đồng thời tuân thủ các quy tắc phụ thuộc kỹ thuật (ví dụ: Quản lý kho sách và Đăng nhập phải làm trước Tìm kiếm và Đặt trước sách), danh sách 12 hạng mục được sắp xếp lại thành một Product Backlog duy nhất như sau:

| Thứ tự | Hạng mục Backlog | Nhóm MoSCoW | Điểm | Lý do sắp xếp thứ tự |
| --- | --- | --- | --- | --- |
| 1 | Đăng nhập/đăng ký tài khoản độc giả | Must have | 2 (M) | Nền tảng xác thực, bắt buộc đứng đầu để định danh người dùng. |
| 2 | Thủ thư quản lý kho sách (thêm/sửa/xóa sách) | Must have | 3 (L) | Phải có dữ liệu sách trong kho thì các tính năng tìm kiếm mới hoạt động được. |
| 3 | Tìm kiếm sách theo tên/tác giả | Must have | 2 (M) | Phụ thuộc vào kho sách (mục 2), giúp độc giả tra cứu tài nguyên. |
| 4 | Đặt trước sách khi hết (kèm thông báo) | Must have | 2 (M) | Tính năng nghiệp vụ cốt lõi xử lý khi sách hết, hoàn thiện bộ Must. |
| 5 | Mượn sách online (có giới hạn số sách) | Should have | 3 (L) | Nằm ở nhóm đệm số 1, là nghiệp vụ chính của Release 1 sau khi có kho và tài khoản. |
| 6 | Xem lịch sử mượn sách của bản thân | Should have | 2 (M) | Phụ thuộc vào việc đã có dữ liệu mượn sách (mục 5). |
| 7 | Thông báo email khi sắp đến hạn trả sách | Should have | 2 (M) | Hỗ trợ nghiệp vụ mượn trả, giảm tỷ lệ quá hạn. |
| 8 | Gia hạn mượn sách online | Could have | 2 (M) | Tiện ích gia tăng cho độc giả đang mượn sách. |
| 9 | Tích hợp đăng nhập bằng Google/Facebook | Could have | 2 (M) | Mở rộng phương thức đăng nhập sau khi hệ thống cơ bản ổn định. |
| 10 | Đánh giá & bình luận sách sau khi đọc | Could have | 2 (M) | Tính năng tương tác cộng đồng, đưa xuống nhóm Could. |
| 11 | Gợi ý sách theo sở thích cá nhân (recommendation) | Won't have | 3 (L) | Hoãn lại bản sau do thuật toán phức tạp và tốn tài nguyên. |
| 12 | Chat trực tiếp với thủ thư | Won't have | 3 (L) | Hoãn lại bản sau do đòi hỏi hạ tầng chat real-time ngoài luồng MVP. |

## Nhiệm vụ 4: Tự phản biện và bảo vệ quan điểm phân loại

Trong quá trình làm bài, nếu có Product Owner khác hoặc giảng viên tranh cãi về cách phân loại một số hạng mục nhạy cảm (như mục 7, 11, 12), họ và tôi có thể đưa ra các lập luận bảo vệ khác nhau như sau:

Thứ nhất, đối với hạng mục 'Gợi ý sách theo sở thích cá nhân' (mục 7): Một số người có thể muốn đẩy mục này lên nhóm Could have hoặc Should have vì cho rằng tính năng gợi ý giúp tăng trải nghiệm và giữ chân người dùng ngay từ phiên bản đầu. Tuy nhiên, lập luận của tôi là giữ nó ở nhóm Won't have vì MVP của thư viện chuẩn bị cho mượn sách giấy (độc giả đặt online rồi đến quầy nhận), thuật toán gợi ý đòi hỏi dữ liệu hành vi lớn vốn chưa tồn tại ở ngày đầu phát hành, việc cố đưa vào sẽ làm lãng phí 3 điểm công sức quý giá.

Thứ hai, đối với hạng mục 'Chat trực tiếp với thủ thư' (mục 11): Có ý kiến cho rằng đây là Must have hoặc Should have để giải đáp thắc mắc mượn sách tức thời cho độc giả. Tôi phản biện rằng trong giai đoạn MVP với quy mô thư viện vừa và nhỏ, việc hỗ trợ qua số điện thoại hoặc email tại quầy là đủ (workaround). Đưa chat real-time vào giai đoạn 1 tạo áp lực lớn về hạ tầng websocket và nhân sự trực ban, nên việc xếp vào Won't have là quyết định đánh đổi hợp lý.

Thứ ba, tổng công sức 4 mục Must của tôi là 9 điểm (chiếm 45% năng lực Release 1 thay vì sát mốc 60%). Một số ý kiến có thể cho rằng tôi đang quá an toàn và bỏ sót tính năng 'Mượn sách online' (mục 3) ra khỏi nhóm Must. Tôi bảo vệ quan điểm rằng 'Mượn sách online' được xếp vào Should have vì nhóm hoàn toàn có thể kết hợp quy trình đặt giữ chỗ qua mục 5 và chốt mượn thủ công tại quầy trong những ngày đầu chạy thử nghiệm, giúp giảm rủi ro trễ tiến độ sprint.

---

## 📁 Danh sách tệp tin nộp bài trong Repository
- 📝 `bt2.docx`: Báo cáo tài liệu phân tích nghiệp vụ hoàn chỉnh.
