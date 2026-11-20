# Phiếu QC 1 — Road v1.0

Lô được kiểm (học viên): Khưu Minh Phú       Người kiểm (học viên): Vũ Gia Khang  
Ngày: 2026-11-21                          Phiên bản guideline: Road v1.0  
File được kiểm (tên + `revision` trong manifest): khuuminhphu-front.zip, khuuminhphu-fisheye.zip (rev 1)  
Số ảnh kiểm: 6 (+ 0 ảnh thêm, ghi riêng)   Số nhãn đã kiểm (shape + tag): 65  

## Tổng hợp theo mã
| Mã | Loại lỗi | Số mục kiểm | Số lỗi | Mức |
| --- | --- | ---: | ---: | --- |
| QC1-01 tag camera | sai thuộc tính / bỏ sót | 6 | 0 | nặng |
| QC1-02 đủ L1, R1 | bỏ sót | 12 | 2 | nặng |
| QC1-03 position | sai thuộc tính / thừa | 16 | 0 | nặng |
| QC1-04 tâm vạch, chiều, điểm dừng | sai phạm vi / bỏ sót | 16 | 0 | chính |
| QC1-05 vạch đứt, che | sai phạm vi / sai thuộc tính | 16 | 2 | chính |
| QC1-06 style, color, kind | sai thuộc tính | 16 | 0 | chính |
| QC1-07 vùng lái | sai phạm vi / bỏ sót / thừa | 11 | 0 | chính |
| QC1-08 đèn, màu | bỏ sót / sai phạm vi / sai thuộc tính | 8 | 0 | nặng / chính |
| QC1-09 facing, type, group, biển phụ | sai thuộc tính | 8 | 0 | chính |
| QC1-10 hình in, đủ biển | bỏ sót / sai phạm vi | 8 | 0 | chính |
| QC1-11 fisheye | sai phạm vi / sai thuộc tính | 8 | 0 | chính |
| QC1-12 file | lỗi file | 2 | 0 | nhẹ / nặng |

## Danh sách lỗi (mỗi lỗi một dòng)
| # | Mã | Ảnh | Nhãn (label, id) | Mức | Mô tả ngắn |
| --- | --- | --- | --- | --- | --- |
| 1 | QC1-02 | A07 | lane | nặng | Thiếu vạch L1 (vạch biên bên trái của làn xe chạy) |
| 2 | QC1-02 | A09 | lane | nặng | Thiếu vạch R1 (vạch sơn trắng đứt phân làn bên phải xe chạy) |
| 3 | QC1-05 | A04 | lane | chính | Vạch đôi vàng phân làn xe chạy bị vẽ tách thành 2 polyline cùng mang position=L1 (theo Guideline phải gộp thành 1 polyline có kind="double") |
| 4 | QC1-05 | A09 | lane | chính | 2 polyline cùng mang position=L2 (gán nhầm thuộc tính làn) |

*Ghi chú ảnh kiểm không lỗi:*  
- Ảnh **A01** và **B01**: Đầy đủ các nhãn (lane, drivable, road_curb, crosswalk), thuộc tính chuẩn, đủ 4 tag ảnh, không có lỗi.

## Ca mơ hồ
| Ảnh | Câu hỏi cho lead | Lời đáp (nếu có) |
| --- | --- | --- |
| A05 | Không thấy vạch sơn L1 và R1 trên mặt đường | Xác nhận không vẽ L1/R1, chỉ vẽ drivable và road_curb theo ngoại lệ của Guideline |
| A06 | Mép phải đường là vỉa hè, không có sơn kẻ vạch R1 | Xác nhận miễn trừ R1, gán road_curb theo guideline |

## Quyết định
Lỗi nặng: 2   Lỗi chính: 2 / 65 nhãn = 3.08 %   Lỗi nhẹ: 0   Ca chờ lead: 0  
Quyết định (Release / Hold / Rework): Rework  
Lý do (theo luật của phiếu): Còn 2 lỗi nặng QC1-02 ở ảnh A07 (thiếu L1) và A09 (thiếu R1). Cần chuyển học viên Khưu Minh Phú sửa lại trong khung giờ buffer trước khi Release.

Loại lỗi: bỏ sót = thiếu nhãn phải có; thừa = gán cái không phải đối tượng; sai phạm vi = hình lệch, sai chiều, dừng sai chỗ, tràn vùng. Ba loại này theo cách chia lỗi gán nhãn của ISO/IEC 5259-4 (mục 8.4.2); "sai thuộc tính" và "lỗi file" là khóa học thêm. Cách xếp mức: [thang mức lỗi](../docs/qc_severity_road_v1.0.md).
