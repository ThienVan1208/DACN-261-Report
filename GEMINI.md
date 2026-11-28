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
- Không trình bày Behavioral Cloning, DAgger, NeuralMinimax và NNUE chuẩn; về mạng đánh giá nhanh chỉ dùng **Residual NNUE**.
- Phần thực nghiệm AI trình bày theo khung nghiên cứu cắt bỏ từng thành phần (mạng chính sách thuần, Minimax, Minimax kết hợp Residual NNUE, Hybrid Bot, LLM Bot), trong đó mạng tự quyết định nước đi và Minimax thuần là các mốc đối chứng truyền thống.
- Số liệu thực nghiệm phải lấy từ kết quả đo thực tế, ghi rõ số trận và khoảng tin cậy; không khẳng định vượt trội khi số liệu không chứng minh được (ví dụ không nêu LLM Bot hay Hybrid Bot mạnh hơn nhau khi chưa đối đầu trực tiếp).

## Phạm vi phụ trách và vùng bất khả xâm phạm (Multiplayer)

- Người dùng **Thiên Văn** chỉ phụ trách các phần ngoài Multiplayer của dự án và báo cáo.
- Tuyệt đối không chỉnh sửa, viết lại hoặc can thiệp vào bất kỳ tệp, mục hay đoạn nội dung nào liên quan đến **Multiplayer** (bao gồm `Content/Multiplayer/main.tex` và toàn bộ các mục/đoạn Multiplayer trong các chương khác) trừ khi có mệnh lệnh ngoại lệ rõ ràng từ người dùng.

## Định hướng thương mại hóa cho phân hệ Smart Customization (SC)

- Mục tiêu của dự án là hướng tới sản phẩm có thể thương mại hóa, do đó ở bản phát hành (khi chạy thực tế) phân hệ **Smart Customization** **không sử dụng các mô hình/thành phần phi thương mại**: **IC-Light** bị loại bỏ hoàn toàn; **HRN** không được gọi khi chạy.
- **HRN** chỉ được dùng ngoại tuyến làm giáo viên sinh nhãn huấn luyện cho mạng học sinh ở giai đoạn nghiên cứu. Báo cáo phải trình bày minh bạch điều này, kèm rủi ro pháp lý (dùng đầu ra của mô hình phi thương mại để huấn luyện) và kế hoạch thay bằng nguồn dữ liệu sạch bản quyền ở Giai đoạn 2; tuyệt đối không viết như thể quy trình không hề phụ thuộc HRN.
- Luồng sản phẩm chính thức chỉ sử dụng quy trình Smart Customization do nhóm tự xây dựng (mạng học sinh hai nhánh dự đoán 60 thông số hình thái 3D, chiếu ngược kết cấu và khử bóng đối xứng tự cài đặt, vật liệu mắt và hệ thống 14 kiểu tóc 3D dùng chung cho hai giới).
- Các công trình nghiên cứu như **MeInGame**, **HRN**, **IC-Light** chỉ được trình bày ở vai trò **phương pháp tham khảo ngoài thực tế / nghiên cứu liên quan** hoặc các phương án đã khảo sát và loại bỏ vì ràng buộc bản quyền phi thương mại.
