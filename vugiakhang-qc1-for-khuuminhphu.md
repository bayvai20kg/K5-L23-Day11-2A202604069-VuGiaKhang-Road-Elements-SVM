# Phiếu QC 1 — Road v1.0

Lô được kiểm (học viên): Khưu Minh Phú       Người kiểm (học viên): Vũ Gia Khang  
Ngày: 2026-11-21                          Phiên bản guideline: Road v1.0  
File được kiểm (tên + `revision` trong manifest): khuuminhphu-front.zip, khuuminhphu-fisheye.zip (rev 1)  
Số ảnh kiểm: 6 (+ 2 ảnh thêm, ghi riêng)   Số nhãn đã kiểm (shape + tag): 56  

## Tổng hợp theo mã
| Mã | Loại lỗi | Số mục kiểm | Số lỗi | Mức |
| --- | --- | ---: | ---: | --- |
| QC1-01 tag camera | sai thuộc tính / bỏ sót | 8 | 0 | nặng |
| QC1-02 đủ L1, R1 | bỏ sót | 6 | 0 | nặng |
| QC1-03 position | sai thuộc tính / thừa | 12 | 0 | nặng |
| QC1-04 tâm vạch, chiều, điểm dừng | sai phạm vi / bỏ sót | 12 | 0 | chính |
| QC1-05 vạch đứt, che | sai phạm vi / sai thuộc tính | 10 | 0 | chính |
| QC1-06 style, color, kind | sai thuộc tính | 10 | 0 | chính |
| QC1-07 vùng lái | sai phạm vi / bỏ sót / thừa | 8 | 0 | chính |
| QC1-08 đèn, màu | bỏ sót / sai phạm vi / sai thuộc tính | 14 | 0 | nặng / chính |
| QC1-09 facing, type, group, biển phụ | sai thuộc tính | 14 | 0 | chính |
| QC1-10 hình in, đủ biển | bỏ sót / sai phạm vi | 8 | 0 | chính |
| QC1-11 fisheye | sai phạm vi / sai thuộc tính | 10 | 0 | chính |
| QC1-12 file | lỗi file | 2 | 0 | nhẹ / nặng |

## Danh sách lỗi (mỗi lỗi một dòng)
| # | Mã | Ảnh | Nhãn (label, id) | Mức | Mô tả ngắn |
| --- | --- | --- | --- | --- | --- |
| 1 | - | - | - | - | Không phát hiện lỗi nghiêm trọng nào |

## Ca mơ hồ
| Ảnh | Câu hỏi cho lead | Lời đáp (nếu có) |
| --- | --- | --- |
| A05 | Đường không có vạch kẻ sơn mép phải (chỉ có vỉa hè) | Xác nhận không vẽ R1, chỉ gán road_curb theo guideline |

## Quyết định
Lỗi nặng: 0   Lỗi chính: 0 / 56 nhãn = 0.0 %   Lỗi nhẹ: 0   Ca chờ lead: 0  
Quyết định (Release / Hold / Rework): Release  
Lý do (theo luật của phiếu): Không có lỗi nặng, tỷ lệ lỗi chính 0.0% (< 5%), các nhãn tuân thủ đầy đủ Guideline Road v1.0.

Loại lỗi: bỏ sót = thiếu nhãn phải có; thừa = gán cái không phải đối tượng; sai phạm vi = hình lệch, sai chiều, dừng sai chỗ, tràn vùng. Ba loại này theo cách chia lỗi gán nhãn của ISO/IEC 5259-4 (mục 8.4.2); "sai thuộc tính" và "lỗi file" là khóa học thêm. Cách xếp mức: [thang mức lỗi](../docs/qc_severity_road_v1.0.md).
