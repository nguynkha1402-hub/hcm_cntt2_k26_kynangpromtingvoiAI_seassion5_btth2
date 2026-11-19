-Tiêu đề (Headline - H1): Độ dài dưới 70 ký tự, chứa từ khóa chính, nêu bật giá trị cốt lõi của AI Chatbot cho doanh nghiệp (tránh giật tít sáo rỗng).

-Đoạn mở đầu (Lead): Dài 100 – 150 từ, đánh thẳng vào nỗi đau (pain points) lớn nhất từ <OUTPUT_1> (như quá tải CSKH, chi phí vận hành cao) và giới thiệu AI Chatbot như giải pháp tất yếu.

-Hệ thống tiêu đề con (H2, H3):

- Khớp 100% với dàn ý ở <OUTPUT_2>.

- Phân bổ từ khóa chính và từ khóa phụ tự nhiên trong các thẻ H2, H3.

- Triển khai sâu từng luận điểm (3 – 4 dòng/đoạn, có in đậm ý chính) để đạt tổng dung lượng 1.000 – 1.500 từ.

-Lời kêu gọi hành động (CTA): Nằm ở đoạn kết bài, nêu rõ hành động tiếp theo và lợi ích đi kèm (ví dụ: Đăng ký trải nghiệm Demo miễn phí 14 ngày hoặc Nhận tư vấn tích hợp 1-1).

#### Prompt 1: Phân tích khách hàng & Nỗi đau
```Plaintext
Vai trò: Chuyên gia Product Marketing B2B.
Sản phẩm: [Tên AI Chatbot] - [Tính năng cốt lõi].
Nhiệm vụ: Phân tích chân dung người ra quyết định (CEO, CMO, Giám đốc CSKH) và 4 nỗi đau (pain points) sản phẩm giải quyết.
Định dạng đầu ra (chỉ xuất nội dung trong thẻ):
<OUTPUT_1>
1. Chân dung khách hàng (KPIs, rào cản khi dùng AI): ...
2. 4 Nỗi đau -> Giải pháp của sản phẩm -> Lợi ích đo lường được: ...
3. Thông điệp cốt lõi (1 câu): ...
</OUTPUT_1>
```
#### Prompt 2: Lập dàn ý chuẩn SEO
```Plaintext
Vai trò: Senior SEO Content Strategist.
Đầu vào: [Dán toàn bộ <OUTPUT_1> vào đây]
Từ khóa SEO: Chính: [Từ khóa chính] | Phụ: [Từ khóa phụ].
Nhiệm vụ: Dựa trên <OUTPUT_1>, lập dàn ý bài PR 1.000 - 1.500 từ theo chuẩn SEO.
Định dạng đầu ra (chỉ xuất nội dung trong thẻ):
<OUTPUT_2>
1. Tiêu đề (H1): Dưới 70 ký tự, chứa từ khóa chính, mang tính chuyên gia.
2. Mở đầu (Lead - 120 từ): Đánh thẳng vào nỗi đau lớn nhất từ <OUTPUT_1>.
3. Thân bài (H2, H3): Chia rõ các mục H2/H3 giải quyết hết 4 nỗi đau, ghi rõ số từ dự kiến và từ khóa cần chèn.
4. Kết bài & CTA: Khẳng định thông điệp cốt lõi + Lời kêu gọi hành động cụ thể (VD: Đăng ký Demo miễn phí).
</OUTPUT_2>
```
#### Prompt 3: Viết bài chi tiết
```Plaintext
Vai trò: Senior Tech Copywriter.
Đầu vào:
- Insight: [Dán <OUTPUT_1>]
- Dàn ý: [Dán <OUTPUT_2>]

Nhiệm vụ: Viết hoàn chỉnh bài PR (1.000 - 1.500 từ) bám sát 100% <OUTPUT_2>.
Ràng buộc:
- Cấu trúc SEO: Đầy đủ H1, Lead, H2, H3 (định dạng Markdown) và CTA cuối bài; chèn từ khóa tự nhiên.
- Giọng điệu: Xuyên suốt là chuyên nghiệp, khách quan, tin cậy (không đổi giọng giữa chừng, không PR sáo rỗng).
- Trình bày: Đoạn ngắn 3-4 dòng, in đậm ý chính. Bắt đầu ngay từ H1.
```
Lệnh xử lý khi bị ngắt quãng (Max Token)
```Plaintext
Bài viết bị ngắt quãng. Viết tiếp ngay sau cụm từ cuối cùng này: "[Dán 10 từ cuối trước khi bị ngắt]".
Quy tắc: Nối khớp hoàn hảo về ngữ pháp, không lặp lại ý cũ, không thêm lời dẫn, giữ nguyên giọng điệu chuyên nghiệp và hoàn tất các mục H2, H3, CTA còn lại theo <OUTPUT_2>.
```