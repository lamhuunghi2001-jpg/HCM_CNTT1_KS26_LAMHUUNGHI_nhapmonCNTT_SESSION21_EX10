## HỌ VÀ TÊN: **LÂM HỮU NGHỊ**
# LỚP: **HCM_KS26_CNTT1**
## Phần 1, câu 1: Bảng so sánh Trade-off
| Tiêu chí đánh giá | 	Phương án 1: Hỗ trợ cảm tính / Nhóm chat | Phương án 2: Troubleshooting 4 chặng chuẩn hóa |
|---|---|---|
| 1. Thời gian xử lý sự cố (Downtime) | Kéo dài, phụ thuộc Senior Dev có rảnh trả lời hay không. Mỗi giờ chết mất 500.000 VNĐ mỗi trụ. | Rút ngắn khoảng 80%, kỹ thuật viên tự giải quyết tại chỗ trong 5 đến 10 phút đầu. |
| 2. Áp lực và chi phí cho Senior Dev | Rất cao, bị phân tâm liên tục bởi các câu hỏi lỗi cơ bản lặp lại. | Tối ưu, chỉ nhận ca phức tạp đã có Bug Report chuẩn. |
| 3. Năng lực và tính tự chủ của KTV | Thụ động, sợ thông báo lỗi tiếng Anh, bó tay khi mất mạng nội bộ, không tiến bộ nghề nghiệp. | Chủ động, biết phân tích và tra cứu, làm chủ máy tính trạm. |
| 4. Khả năng lưu vết tri thức (Knowledge Base) | Thất thoát, tin nhắn trôi mất trên Zalo, người sau gặp lại lỗi cũ vẫn phải hỏi lại. | Lưu trữ tập trung qua phiếu Bug Report, tích lũy thành Wiki sửa lỗi nội bộ. |

## Phần 1, câu 2: Vì sao phải chọn Phương án 2 khi lên 1.000 trạm 
Ban Giám đốc nên chọn Phương án 2. 
Với Phương án 1, mọi lỗi đều đổ về một nhóm Senior Dev có hạn, nên khi số trạm tăng từ 10 lên 1.000 thì hàng đợi hỗ trợ dài ra, mỗi trụ chết thêm giờ là mất thêm 500.000 VNĐ và uy tín với khách đi xe điện giảm theo. Phương án 2 cho kỹ thuật viên tự xử lý phần lớn lỗi cơ bản ngay tại trạm, Senior Dev chỉ nhận những ca khó đã có Bug Report rõ ràng. Kỹ thuật viên cũng có kỹ năng tự gỡ lỗi khi mất mạng nội bộ, và mỗi phiếu sự cố được lưu lại thành tri thức cho người sau. Chỉ cách làm này mới mở rộng được mà không phải tuyển thêm Senior Dev theo từng trạm.
[Kiosk hiện Error Pop-up]
          |
          v
CHẶNG 1: Bóc tách từ khóa, tìm Google với toán tử
   - "cụm lỗi nguyên văn" (dấu ngoặc kép, khớp chính xác)
   - site:stackoverflow.com hoặc site:github.com (giới hạn trang)
   - -từ_khóa_nhiễu (loại kết quả không liên quan)
          |
          +-- Có kết quả StackOverflow/GitHub? --Không--> nhảy sang CHẶNG 3
          | Có
          v
CHẶNG 2: Thẩm định bài viết
   - Đọc lướt 30 giây: đúng lỗi, đúng HĐH/phiên bản không?
   - Kiểm tra tích xanh (✓) và số upvote
   - Chỉ thử cách phù hợp, không copy mù quáng lệnh phá hệ thống
          |
          +-- Giải quyết được? --Có--> XONG, ghi lại cách sửa
          | Chưa
          v
CHẶNG 3: Lỗi khó hiểu thì dùng AI
   - Gửi Prompt 3 thành phần: [Context] [Raw Error] [Instruction]
   - Che Secret/API Key trước khi dán
   - Thử tối đa 2 giải pháp AI đưa ra
          |
          +-- Giải quyết được? --Có--> XONG, ghi lại cách sửa
          | Chưa, đã quá 15 phút
          v
CHẶNG 4: Điền Bug Report chuẩn 4 bước
   - Gửi về IT Helpdesk (cấp 2), kèm log nguyên văn
     và những gì đã thử ở chặng 1 đến 3