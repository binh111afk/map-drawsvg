# 🗺️ Map DrawSVG — Thiết kế bản đồ kéo–thả

Tool web **1 file HTML duy nhất** (vanilla JS + SVG, không dependency, không cần cài đặt) để vẽ bản đồ tưởng tượng kiểu Google Maps chỉ bằng kéo–thả, rồi xuất **SVG/PNG**.

## Chạy

Mở thẳng `index.html` bằng trình duyệt, hoặc (nếu bật GitHub Pages) truy cập:
`https://binh111afk.github.io/map-drawsvg/`

## Tính năng

- **Kéo–thả** từ khung nguyên liệu: đường, nhà ống, nhà chữ L/T/U, hình thang, nghiêng, tòa nhà, công viên (blob), hồ, sông, cây, đèn đường, xe, vạch sang đường, nhãn tên…
- **Đường & sông đa điểm uốn**: kéo dấu "+" trên thân để thêm chỗ uốn (spline Catmull-Rom mượt), nhấp đúp chấm cam để bỏ; chỉnh chiều dài/rộng/độ mềm bằng bảng chỉ số; sông nằm dưới đường → đường đi ngang thành cầu.
- **Hình khối kiểu Word (29 shape)**: menu xổ từ topbar; từng hình đổi được **màu nền, màu viền** (kèm màu tùy chọn + ống hút lấy màu màn hình) và **độ cong** bằng thanh trượt.
- **Địa danh (pin)**: 10 biểu tượng (nhà, bệnh viện, trường học, kho/giao hàng…), chọn màu Google, chỉnh cỡ 70%–300%.
- **Đổi màu nhà/tòa nhà**: xanh lá, xanh đậm hoặc màu tùy chọn.
- **Sửa hình dạng tự do**: chọn công viên/hồ/hình khối là có chấm cong trên viền — kéo để nắn hình bất kỳ; nhà nhấp đúp để sửa đỉnh.
- **Nhập SVG**: dán mã hoặc chọn file .svg, xem trước rồi đặt lên canvas như một vật thể.
- **2 giao diện màu**: Google Maps & Xám công nghiệp (nút Giao diện).
- Khung chọn kiểu Canva: 4 chấm góc resize, nút xoay ↻, mini-toolbar nhân đôi/xóa/định dạng nổi trên vùng chọn.
- **Tự lưu phiên làm việc** vào localStorage (mở lại là khôi phục nguyên trạng, kể cả theme và vị trí khung nhìn).
- Undo/redo 150 bước, snap lưới, zoom (lăn chuột hoặc nhập %), pan, phím tắt (Ctrl+Z/Y/D, Delete, mũi tên).
- **Xuất**: file SVG, file PNG (2x), hoặc **sao chép code SVG** vào clipboard.

## Ghi chú

- Tool chạy hoàn toàn offline, không gửi dữ liệu đi đâu.
- File xuất SVG là bản sạch: chỉ chứa bản đồ theo giao diện màu đang bật.
