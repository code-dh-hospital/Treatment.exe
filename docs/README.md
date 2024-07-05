





## [v.4.24.0620.0]()
## 4.24.0705.0 [⬇️OneDrive](https://dh-hos-code.github.io/directTo/?&redirect_url=https%3A%2F%2Fo-dh-007-default-rtdb.asia-southeast1.firebasedatabase.app%2F%2FdirectTo%2FTreatmentexe%2F42407050-OneDrive.json) [⬇️GoogleStorage](https://dh-hos-code.github.io/directTo/?&redirect_url=https%3A%2F%2Fo-dh-007-default-rtdb.asia-southeast1.firebasedatabase.app%2F%2FdirectTo%2FTreatmentexe%2F42407050-GoogleStorage.json) [⬇️NasDHSolutions](https://dh-hos-code.github.io/directTo/?&redirect_url=https%3A%2F%2Fo-dh-007-default-rtdb.asia-southeast1.firebasedatabase.app%2F%2FdirectTo%2FTreatmentexe%2F42407050-NasDHSolutions.json)
- ✨: Treatment bổ sung mamay khi thực hiện ghi nhận phiếu PT,TT #35
	- Bổ sung chức năng: ghi nhận mã máy vào phẫu thuật/thủ thuật
	- phauthuat.mamay = dmmamay.mamay
	![image](https://github.com/dh-hos/THEO-DOI-THUC-HIEN-4750/assets/32563776/19ef8506-4e51-4560-af50-bd4494843ac3)
	
	Hiện thị danh mục mã máy kho cận lâm sàng
	![image](https://github.com/dh-hos/THEO-DOI-THUC-HIEN-4750/assets/32563776/5d10bf03-078a-40c3-b32a-4cf7e281ea30)

	![image](https://github.com/dh-hos/THEO-DOI-THUC-HIEN-4750/assets/32563776/9452e9a0-4175-4db7-8071-5a18acff3752)

	- Bổ sung chức năng tóm tắt kết quả CLS có giá trị chẩn đoán vào form xuất viện (cột này là bắt buột nhập, hỗ trợ xuất xml8 )

	![image](https://github.com/dh-hos/THEO-DOI-THUC-HIEN-4750/assets/32563776/25861284-4410-48a5-a2bc-96023ab8f635)

- ☑: https://github.com/dh-hos/THEO-DOI-THUC-HIEN-4750/issues/35
- ☑: https://github.com/dh-hos/To_Ho_Tro/issues/20
- ☑: https://github.com/dh-hos/To_Trien_Khai/issues/57
## [v.4.24.0704.0]()
- ✨: Update code
## [v.4.24.0702.1]()

- 🐛: Lỗi liều dung toa xuất viện - Treat #429
	--> Fix lỗi toa xuất viện (không kiểm tra số lượng tổng và các lần trong ngày)
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/429

- ✨: Yêu cầu bổ sung chức năng nhập liều dùng đối với chức năng ra toa ngoại trú - BN nội trú #430
	--> Bổ sung chức năng cập nhật liều dùng
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/430

## [v.4.24.0702.0]()
- ✨: Yêu cầu - Khi lập phiếu PT, TT tại Prescription và Treatment bắt buộc phải nhập Ekip mới cho lưu. #432
	- Thay đổi:
		- Cách cũ: nhập phiếu TT,PT --> Lưu --> nhập ekip
		- Cách mới: nhập phiếu TT, PT --> nhập ê kíp --> lưu
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/432
## [v.4.24.0701.1]()
- ✨: Yêu cầu - Treatment cho cập nhật lại chẩn đoán khi cận lâm sàng đã có kết quả #411
	- Bổ sung tham số: nt.capnhat_dienbien: Cập nhật lại diễn biến trên toa thuốc và cận lâm sàng (cùng diễn biến)
		- 0: Không áp dụng,
		- 1: Cập nhật lại diễn biến trên toa thuốc chưa tổng hợp, cls chưa thực hiện
		- 2: Cập nhật lại diễn biến tất cả toa thuốc, cls

	Câp nhật các bảng: bnnoitru, ttcon, chidinhcls, chungtu (khi có cùng idienbien cần cập nhật)

- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/411
## [v.4.24.0701.0]()
- ✨: Thêm chức năng tự động tính giá trị dinh dưỡng dựa vào dữ liệu có sẳn

- ✨: Chuyển đổi trang in tình trạng dinh dưỡng sang tự thiết kế

- ✨: thêm các para cannangtheotuoi, cannangtheochieucao, chieucaotheotuoi, bmitheotuoi

- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/410

![](https://i.imgur.com/Pk5P75I.png)

![](https://i.imgur.com/7AbOVdk.png)
## [v.4.24.0630.0]()
- ✨: Yêu cầu thực hiện Theo mô tả - QUY TRÌNH TRẢ THUỐC/VTYT NGƯỜI BỆNH ĐIỀU TRỊ NỘI TRÚ #404
QUI TRÌNH TRẢ THUỐC:
	- Cả toa: như cũ (ghi nhận thêm cột pshdx.sohdx = số chứng từ xuất)
	- Trả lẻ (trả thuốc, tủ trực, toa mổ):
		
		- Hiện thị danh mục thuốc đã xuất - trả (theo từng loại trả)
		![image](https://github.com/dh-hos/To_Lap_Trinh/assets/32563776/2d7f4da6-5756-458a-8477-207a5fac4c68)
		- Người có thể trả bằng hoặc ít hơn số lượng đã xuất


- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/404
## [v.4.24.0628.0]()
- ✨: Yêu cầu - Hỗ trợ cập nhật tự động giờ kết thúc giường bệnh theo ngày khám chữa bệnh #402
	Bổ sung tham số: nt.capnhat_ngaykq

	Diễn giải: Cập nhật tự động ngày kết quả giường bệnh (áp dụng cho giường bệnh chưa có ngày kq):

	0: Không áp dụng,

	1: Cập nhật khi lưu chỉ định CLS giường bệnh (ngày kết quả = ngày kcb + giờ (23:59))

	2: a. Cập nhật khi chuyển khoa:
	- Nếu ngày kcb != ngày chuyển khoa==> ngày kết quả = ngày kcb + giờ (23:59)
	- Ngày kcb = ngày chuyển khoa==> ngày kết quả = ngày giờ chuyển khoa
	b. Cập nhật khi xuất viện:
	- Nếu ngày kcb != ngày xuất viện ==> ngày kết quả = ngày kcb + giờ (23:59)
	- Ngày kcb = ngày xuất viên ==> ngày kết quả = ngày giờ xuất viện

- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/402
## [v.4.24.0627.0]()
- ✨: Yêu cầu - Bổ sung thêm trường phòng khám trên mẫu Phiếu nhập viện tự thiết kế (BV Thanh Bình) #379
- Cập nhật:
	buong: bnnoitru.buong
	tenphong = dmphong.tenphong
	
	Có cập nhật một phần, trả thuốc ghi nhận số ct trả, đề nghị chạy script tạo cột pshdxn.sohdx. Test trả thuốc (toa bình thường và toa tủ trực).

- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/379
## [v.4.24.0624.0]()
- ✨: Yêu cầu - Hỗ trợ cập nhật tự động giờ kết thúc giường bệnh theo ngày khám chữa bệnh #402
	- Bổ sung tham số: nt.capnhat_ngaykq
	- Diễn giải: Cập nhật tự động ngày kết quả giường bệnh (áp dụng cho giường bệnh chưa có ngày kq): 
		0: Không áp dụng,
		1: Cập nhật khi lưu chỉ định CLS giường bệnh (ngày kết quả = ngày kcb + giờ (23:59)
		2: Cập nhật khi chuyển khoa (ngày kq = ngày giờ chuyển khoa); cập nhật khi xuất viện (ngày kq = ngày giờ xuất viện)

	- Thêm CLS giường bệnh:
	![image](https://github.com/dh-hos/To_Lap_Trinh/assets/32563776/a7b86dcb-73ce-49be-81f0-168b3c468567)

	(1): Chỉnh ngày giờ chỉ định (ngaykcb)
	(3): Lưu
	(4) Xem danh sách giường bệnh
	Cập nhật từ tường bệnh được chọn:

	![image](https://github.com/dh-hos/To_Lap_Trinh/assets/32563776/49095406-41e3-4723-a566-392c94e8a044)

	Cập nhật cùng lúc nhiều giường bệnh cùng mã số:
	![image](https://github.com/dh-hos/To_Lap_Trinh/assets/32563776/947cc1cd-3250-48d5-b40a-ad1a9e0fbe7b)

	Chuyển khoa:
	![image](https://github.com/dh-hos/To_Lap_Trinh/assets/32563776/6191bd9e-51e8-43fb-b73e-2ffcda69b15b)

	Xuất viện: update ngày kết quả bằng ngày giờ xuất viện

- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/402
- ✨: Yêu cầu thực hiện 4750 - Cập nhật số liệu Liều dùng theo pshdxn #129
Cập nhật: 
- Bảng cũ chương trình tự chia đều các lần uống (nếu có)
- Bảng cập nhật (người dùng tự chia): 
	+ Không chia các lần uống (số lượng: sáng, trưa, chiếu, tối bằng 0)
	+ Nếu chia các lần các lần uống: tổng các lần uống phải bằng số lượng tổng 
	![image](https://github.com/dh-hos/Yeu_cau_ho_tro/assets/32563776/71b7ba5b-5217-4da4-a590-20166c59d922)
- ☑: https://github.com/dh-hos/Yeu_cau_ho_tro/issues/129

✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #20
☑: https://github.com/dh-hos/To_Ho_Tro/issues/20

✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #57
☑: https://github.com/dh-hos/To_Trien_Khai/issues/57
## [v.4.24.0619.0]()
- ✨: Yêu cầu thực hiện 4750 - Thay đổi cách ghi nhận maxa #401
	Form chỉnh thông tin bệnh nhân:
	![image](https://github.com/dh-hos/dhg.hosptaltreatment/assets/32563776/f4e64103-4399-4216-840c-695f8794aa06)
	Khi có dmxa4750 và có dữ liệu --> load dữ liệu từ dmxa4750 ngược lại load từ dmxa 
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/401

✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #20
☑: https://github.com/dh-hos/To_Ho_Tro/issues/20

✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #57
☑: https://github.com/dh-hos/To_Trien_Khai/issues/57
## [v.4.24.0617.0]()
- ✨: Yêu cầu thực hiện 4750 - Cập nhật nhóm máu và giai đoạn bệnh #396
Lưu ý: đô phân giải màn hình tối thiểu: 1152 x 864 (mới hiển thị đầy đủ)
![image](https://github.com/dh-hos/To_Lap_Trinh/assets/32563776/d58bbd97-ddca-4fba-9922-376453ace514)
![image](https://github.com/dh-hos/To_Lap_Trinh/assets/32563776/00668c89-0122-40fd-9fc7-4048c342afc9)
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/396


✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #20
☑: https://github.com/dh-hos/To_Ho_Tro/issues/20

✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #57
☑: https://github.com/dh-hos/To_Trien_Khai/issues/57
## [v.4.24.0613.0]()
- ✨: Yêu cầu - Bổ sung thêm trường phòng khám trên mẫu Phiếu nhập viện tự thiết kế (BV Thanh Bình) #379 (Treatment bổ sung mẫu tự thiết kế)
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/379
- ✨: Yêu cầu - Xác định mã lý do vào viện trên bảng kê 6556 và XML 4210 ( trường hợp bệnh nhân có giấy xác nhận cư trú)
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/389
## [v.4.24.0611.2]()
🐛: Lỗi - PHIẾU THỰC HIỆN KỸ THUẬT PHỤC HỒI CHỨC NĂNG không lấy được Phòng (BV YHCT CT) #230
	- Bổ sung para: tenphong
☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/230
## [v.4.24.0611.1]()
- ✨: Yêu cầu - Hỗ trợ cấp số chứng sinh theo đặc thù TTYT Thạnh Trị #367
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/367
## [v.4.24.0611.0]()
✨: Yêu cầu thực hiện 4750 - Thực hiện tích hợp DLL gửi checkIn, hồ sơ #380
☑: https://github.com/dh-hos/To_Lap_Trinh/issues/380
✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #57
☑: https://github.com/dh-hos/To_Trien_Khai/issues/57
✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #20
☑: https://github.com/dh-hos/To_Ho_Tro/issues/20
🐛: Lỗi - PHIẾU THỰC HIỆN KỸ THUẬT PHỤC HỒI CHỨC NĂNG không lấy được Phòng (BV YHCT CT) #230
☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/230

## [v.4.24.0607.1]()
✨: Yêu cầu thực hiện 4750 - Cập nhật số liệu Liều dùng theo pshdxn #371
☑: https://github.com/dh-hos/To_Lap_Trinh/issues/371
✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #57
☑: https://github.com/dh-hos/To_Trien_Khai/issues/57
✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #20
☑: https://github.com/dh-hos/To_Ho_Tro/issues/20
## [v.4.24.0607.0]()
- 🐛: Lỗi - Chỉnh thông tin bệnh nhân nội trú nút Lưu không lưu được #65
- ☑: https://github.com/dh-hos/dhg.hospitaladmin/issues/65
## [v.4.24.0606.2]()
✨: Yêu cầu - BV Phụ Sản Cần Thơ: Treatment cho phép nhập số hộ chiếu vào ô CMND (Form Thông tin bệnh nhân) #369
☑: https://github.com/dh-hos/To_Lap_Trinh/issues/369
✨: Yêu cầu thực hiện 4750 - Kiểm tra dữ liệu thông tin bệnh nhân kiểm tra ô [CMND] #370
☑: https://github.com/dh-hos/To_Lap_Trinh/issues/370
✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #57
☑: https://github.com/dh-hos/To_Trien_Khai/issues/57
✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #20
☑: https://github.com/dh-hos/To_Ho_Tro/issues/20
## [v.4.24.0606.1]()
✨: Yêu cầu - BV Phụ Sản Cần Thơ: Treatment cho phép nhập số hộ chiếu vào ô CMND (Form Thông tin bệnh nhân) #369
☑: https://github.com/dh-hos/To_Lap_Trinh/issues/369
✨: Yêu cầu thực hiện 4750 - Kiểm tra dữ liệu thông tin bệnh nhân kiểm tra ô [CMND] #370
☑: https://github.com/dh-hos/To_Lap_Trinh/issues/370
✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #57
☑: https://github.com/dh-hos/To_Trien_Khai/issues/57
✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #20
☑: https://github.com/dh-hos/To_Ho_Tro/issues/20
## [v.4.24.0606.0]()
- 🐛: Lỗi - Test_Mất Logo phần mềm #68
- ☑: https://github.com/dh-hos/dhg.hospitalregister/issues/68
## [v.4.24.0605.5]()
- ✨: Yêu cầu - Bổ sung tiêu chí thời gian xem báo cáo #373 --> bỏ giới hạn ngày thuộc tháng kế toán
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/373
## [v.4.24.0605.4]()
- ✨: Yêu cầu thực hiện 4750 - Kiểm tra dữ liệu thông tin bệnh nhân kiểm tra ô [CMND] #370
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/370
- ✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #57
- ☑: https://github.com/dh-hos/To_Trien_Khai/issues/57
- ✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #20
- ☑: https://github.com/dh-hos/To_Ho_Tro/issues/20
## [v.4.24.0605.3]()
- ✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #57
- ☑: https://github.com/dh-hos/To_Trien_Khai/issues/57
- ✨: Yêu cầu - Hỗ trợ test XML của quyết định 130 #20
- ☑: https://github.com/dh-hos/To_Ho_Tro/issues/20
## [v.4.24.0605.2]()
- 🐛: Lỗi - Toa Xuất viện thuốc Nghiện - HT không hiển thị số ngày uống #227
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/227
## [v.4.24.0605.1]()
- ✨: Yêu cầu - Bổ sung tiêu chí thời gian xem báo cáo #373
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/373
- ✨: Yêu cầu thực hiện 4750 - Kiểm tra dữ liệu thông tin bệnh nhân kiểm tra ô [CMND] #370
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/370
- ✨: Yêu cầu - BV Phụ Sản Cần Thơ: Treatment cho phép nhập số hộ chiếu vào ô CMND (Form Thông tin bệnh nhân) #369
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/369
## [v.4.24.0605.0]()
- ✨: Yêu cầu - Bổ sung tiêu chí thời gian xem báo cáo #373
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/373
- ✨: Yêu cầu thực hiện 4750 - Kiểm tra dữ liệu thông tin bệnh nhân kiểm tra ô [CMND] #370
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/370
- ✨: Yêu cầu - BV Phụ Sản Cần Thơ: Treatment cho phép nhập số hộ chiếu vào ô CMND (Form Thông tin bệnh nhân) #369
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/369

## [v.4.24.0603.0]()
- ✨: Yêu cầu - BV Phụ Sản Cần Thơ: Treatment cho phép nhập số hộ chiếu vào ô CMND (Form Thông tin bệnh nhân) #369
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/369
## [v.4.24.0531.0]()
- ✨: Yêu cầu - BV Phụ Sản CT: 1. Mẫu tự thiết kế Biên bản hội chẩn và Trích Biên bản hội chẩn trên Prescription và Treatment
	+ Chỉnh mẫu số 40/BV-01 --> 27/BV-02
	+ Chỉnh các trường rớt dòng
	+ Chuỗi: Tuổi: ...........; Nam hoặc nữ <= là đúng mẫu (Mẫu không có chữ giới tính)
	+ Chuỗi: Tuỗi: ............ ==> Ngày sinh: ......... là do yêu cầu làm riêng của BV PSCT (92118), các bệnh khác không ảnh hưởng
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/346
## [v.4.24.0527.1]()
- 🐛: Lỗi - Form Khám điều trị bệnh double tên bệnh nhân khi vừa có Thông tin thẻ thứ 2 và có thêm Thông tin con
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/228
- ✨: Yêu cầu - BV Phụ Sản CT: 1. Mẫu tự thiết kế Biên bản hội chẩn và Trích Biên bản hội chẩn trên Prescription và Treatment
		- Đổi chở chữ và margin
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/346
## [v.4.24.0527.0]()
- 🐛: Lỗi - Form Khám điều trị bệnh double tên bệnh nhân khi vừa có Thông tin thẻ thứ 2 và có thêm Thông tin con #228
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/228
## [v.4.24.0523.0]()
- ✨: BV Sa Đéc yêu cầu bỏ chức năng load danh sách bệnh nhân theo tài khoản đăng nhập
## [v.4.24.0520.0]()
- ✨: Mẫu biên bản hội chẩn tự thiết kế
	  Bật tham số nt.inbienbanhc = 3
	  --> fix lỗi thiếu para
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/346
## [v.4.24.0517.0]()
﻿- ✨: Yêu cầu - BV Phụ Sản CT: 1. Mẫu tự thiết kế Biên bản hội chẩn và Trích Biên bản hội chẩn trên Prescription và Treatment
	   Bật tham số: nt.inbienbanhc = 3
- ☑:https://github.com/dh-hos/To_Lap_Trinh/issues/346
- 🐛: Lỗi - Bệnh có nhập CN Miễn nhưng vẫn phát sinh thu 20% (BV Ung Bướu) #226
- ☑:https://github.com/dh-hos/dhg.hosptaltreatment/issues/226
