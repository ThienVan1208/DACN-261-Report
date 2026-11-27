# Quy tắc riêng của dự án

- Workspace này là dự án báo cáo cho dự án Convergence Chess của ConvergenceChess.
- Mọi nội dung trao đổi, phân tích, biên soạn và chỉnh sửa trong phạm vi workspace này phải tuân theo ngữ cảnh đây là báo cáo của dự án Convergence Chess thuộc ConvergenceChess.

## Phân biệt báo cáo đồ án và tài liệu mã nguồn (codebase document)

- Đây là **báo cáo đồ án**, tuyệt đối không viết theo văn phong tài liệu kỹ thuật mã nguồn (codebase document).
- Ngoại trừ các phần liên quan đến Multiplayer được giữ nguyên theo yêu cầu hiện hành, nghiêm cấm đưa các yếu tố đặc thù của tài liệu mã nguồn vào nội dung báo cáo:
  - Không ghi đường dẫn thư mục, tên tệp mã nguồn/cấu hình, tên lớp, tên hàm, tên biến, tên khóa/cờ cấu hình hay mã checkpoint nội bộ.
  - Không dùng tiếng lóng phát triển phần mềm (ví dụ: codebase, repo, HEAD, fallback, race condition, comment đóng băng, Inspector...).
  - Không nhồi nhét thuật ngữ kỹ thuật tiếng Anh dày đặc; mọi khái niệm kiến trúc, thuật toán và xử lý phải được trình bày bằng văn phong báo cáo tiếng Việt mạch lạc, dễ hiểu. Chỉ giữ tên riêng công nghệ hoặc tên ngắn gọn của phương pháp khoa học cần trích dẫn, kèm diễn giải tiếng Việt rõ nghĩa.

## Phạm vi tác nhân AI (Agent bot) trong báo cáo

- Về phần tác nhân AI (Agent bot), báo cáo chỉ sử dụng hai hướng tác nhân chính là **Hybrid Bot** và **LLM Bot** (không trình bày dàn trải các lớp bot nội bộ hay tác nhân thử nghiệm rời rạc ngoài hai hướng này).

## Phạm vi phụ trách và vùng bất khả xâm phạm (Multiplayer)

- Người dùng **Thiên Văn** chỉ phụ trách các phần ngoài Multiplayer của dự án và báo cáo.
- Tuyệt đối không chỉnh sửa, viết lại hoặc can thiệp vào bất kỳ tệp, mục hay đoạn nội dung nào liên quan đến **Multiplayer** (bao gồm `Content/Multiplayer/main.tex` và toàn bộ các mục/đoạn Multiplayer trong các chương khác) trừ khi có mệnh lệnh ngoại lệ rõ ràng từ người dùng.

## Định hướng thương mại hóa cho phân hệ Smart Customization (SC)

- Mục tiêu của dự án là hướng tới sản phẩm có thể thương mại hóa, do đó trong phân hệ **Smart Customization**, hệ thống chính thức **tắt và không sử dụng các mô hình/thành phần phi thương mại** (như **HRN**, **IC-Light**).
- Luồng sản phẩm chính thức chỉ sử dụng quy trình Smart Customization do nhóm tự xây dựng (tái tạo hình học khuôn mặt 25 thông số độc lập, chiếu ngược kết cấu và khử bóng đối xứng tự cài đặt, vật liệu mắt và hệ thống 6 kiểu tóc 3D).
- Các công trình nghiên cứu như **MeInGame**, **HRN**, **IC-Light** chỉ được trình bày ở vai trò **phương pháp tham khảo ngoài thực tế / nghiên cứu liên quan** hoặc các phương án đã khảo sát và loại bỏ vì ràng buộc bản quyền phi thương mại.
