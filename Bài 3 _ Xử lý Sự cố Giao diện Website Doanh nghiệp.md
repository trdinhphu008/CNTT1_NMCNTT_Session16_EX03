### Phần 1: Báo cáo phân tích (I/O)

Em sử dụng F12, chọn Inspect Element và mở tab Computed để kiểm tra hai khung “Nội dung bài học” và “Danh sách video”.

Box Model gồm 4 lớp:

-   Content: Phần chứa nội dung chính.
    
-   Padding: Khoảng cách từ nội dung đến viền.
    
-   Border: Đường viền bao quanh phần tử.
    
-   Margin: Khoảng cách bên ngoài phần tử.
    

Nguyên nhân chồng lấn có thể do Margin, Padding quá lớn hoặc cách định vị phần tử chưa phù hợp. Em cần kiểm tra thông số thực tế để xác định chính xác lỗi.

Nếu chỉ tăng Margin mà không kiểm tra Padding, bố cục có thể bị lệch, xuất hiện thanh cuộn hoặc hai khung vẫn chồng lên nhau.

### Phần 2: Thiết kế giải pháp

Em mở tab Styles và điều chỉnh CSS như sau:

-   Padding: 12px để tạo khoảng cách bên trong.
    
-   Margin-bottom: 16px để tạo khoảng cách giữa hai khung.
    
-   Width: 100% để khung phù hợp với vùng chứa.
    
-   Box-sizing: border-box để kích thước bao gồm cả Padding và Border.
    
-   Kiểm tra Position để tránh định vị không phù hợp gây chồng lấn.
    

Sau khi sửa, em kiểm tra lại bằng tab Computed để đảm bảo hai khung không còn chồng lấn và giao diện vẫn cân đối.

- Kết luận: Em sử dụng Box Model để xác định nguyên nhân và điều chỉnh CSS phù hợp, giúp giao diện PTIT-LMS hiển thị rõ ràng, dễ sử dụng.
