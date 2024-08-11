






## 4.24.0811.0 [⬇️OneDrive](https://dh-hos-code.github.io/directTo/?&redirect_url=https%3A%2F%2Fo-dh-007-default-rtdb.asia-southeast1.firebasedatabase.app%2F%2FdirectTo%2FTreatmentexe%2F42408110-OneDrive.json) [⬇️GoogleStorage](https://dh-hos-code.github.io/directTo/?&redirect_url=https%3A%2F%2Fo-dh-007-default-rtdb.asia-southeast1.firebasedatabase.app%2F%2FdirectTo%2FTreatmentexe%2F42408110-GoogleStorage.json) [⬇️NasDHSolutions](https://dh-hos-code.github.io/directTo/?&redirect_url=https%3A%2F%2Fo-dh-007-default-rtdb.asia-southeast1.firebasedatabase.app%2F%2FdirectTo%2FTreatmentexe%2F42408110-NasDHSolutions.json)
- ✨: Yêu cầu - Hỗ trợ hàm kiểm tra thông tuyến theo Công văn 1923/BHXH-CNTT ngày 20/06/2024
- ✨: Mô tả thực hiện [Ham API tra cuu TT - theo CV 1923-BHXHVN.md
](https://github.com/dh-hos/Mo-ta-he-thong/blob/main/XML130/QD4570/Ham%20API%20tra%20cuu%20TT%20-%20theo%20CV%201923-BHXHVN.md)
- ✨:  + Chuyển hàm sử dụng thông tuyến KQNhanLichSuKCB2024 (Không theo cấu hình trên Admin)
- ✨:  + Sử dụng tài khoản kiểm tra theo tài khoản đăng nhập, điều kiện cụ thể để tài khoản có thể sử dụng tra cứu là có tài khoản BHXH cung cấp khác rỗng, có họ lót và Số CCCD
- ✨:  + Trường hợp tài khoản đăng nhập không hợp lệ, sẽ tìm theo tài khoản được cấu hình theo khoa, và theo bệnh viện trên Danh mục Nhân viên
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/565
## [v.4.24.0808.0]()
- 🐛: Fix Lỗi - Lỗi in phiếu tử vong thông tư 24 (BV Tim Mạch AG) #254
	- Fix lỗi khi in: lỗi khi lấy địa chỉ
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/254
## [v.4.24.0807.0]()
- ✨: Yêu cầu - BV Tim Mạch AG: Yêu cầu Tham số thời gian tối thiểu từ bắt đầu đến kết thúc phiếu PT-TT #568
	- Cập nhật yêu cầu: [Theo mô tả](https://github.com/dh-hos/Mo-ta-he-thong/blob/main/Mô%20tả%20Kiểm%20tra%20thời%20gian%20kết%20quả%20HA-CN-TT-PT.md)
	- Cảnh báo khi tham số ha.canhbaovuotthoigian = 0
		- Ngày bắt đầu phẫu thuật + số phút <= ngày chỉnh định cls
		![image](https://github.com/user-attachments/assets/dab426f4-e80e-44f3-9cfb-01e867199fe4)

		- Ngày kết thúc phẫu thuật + số phút <= ngày đầu phẫu thuật
		![image](https://github.com/user-attachments/assets/e822063e-c1f0-4f18-9468-2db5a9b93d30)

	- Cảnh báo khi tham số ha.canhbaovuotthoigian = 1
	  - Ngày bắt đầu phẫu thuật + số phút <= ngày chỉnh định cls
	  ![image](https://github.com/user-attachments/assets/7818eae5-5c72-44b6-b3b6-837e71b6b53d)

	  - Ngày kết thúc phẫu thuật + số phút <= ngày đầu phẫu thuật
	  ![image](https://github.com/user-attachments/assets/a96350ca-4694-4bf7-94e1-003142c55e4c)

	Lưu ý: Cập nhật script theo mô tả
	- sophutbatdau = (ưu tiên lấy tuần tự nếu khác 0 theo trình tự: dmcls.sophutthuchienylenh ⇒  dmloaicls.sophutthuchienylenh ⇒ [tham số ha.sophuttoithieu]).
	- sophutketthuc = (ưu tiên lấy tuần tự nếu khác 0 theo trình tự: dmcls.sophuttraketqua ⇒  dmloaicls.sophuttraketqua ⇒ [tham số ha.sophuttraketqua]).
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/568
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/570
## [v.4.24.0806.1]()
- 🐛: Fix Lỗi - LOAD THIẾU THÔNG TIN KHI MỞ FORM THÔNG TIN CON #253

- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/253
## [v.4.24.0806.0]()
- 🐛: Fix Lỗi - TRÙNG MÃ GIƯỜNG & MÃ GIƯỜNG KHÔNG CẢNH BÁO TRÙNG #252
		- Cập nhật: cảnh báo/ chặn theo tham số: nt.magiuong
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/252
## [v.4.24.0801.3]()
- 🐛: Fix lỗi - Không ghi nhận dữ liệu tiền ekip PT/TT #251
		- Fix lỗi sai tháng năm kế toán khi ngày bắt đầu phẫu thuật chưa có trong bảng danh mục ngày
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/251
## [v.4.24.0801.2]()
- 🐛: Fix lỗi - Không ghi nhận dữ liệu tiền ekip PT/TT #251
	- Fix lỗi tháng kết toán bị null
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/251
## [v.4.24.0801.1]()
- 🐛: Fix lỗi - Không ghi nhận dữ liệu tiền ekip PT/TT #251
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/251
## [v.4.24.0801.0]()
- ✨: Yêu cầu - BV Ung Bướu: Mẫu tóm tắt hồ sơ bệnh án theo thông tư 32/2023/TT-BYT #467
	 - Cập nhật tóm tắt bệnh án theo thông tư 32
		
		- Chạy cập nhật cấu trúc

		- Cập nhật tham số:
			- nt.tomtatba_tt32: Tóm tắt bệnh án theo TT32 (0: Không áp dụng, 1: Áp dụng)

		- Chổ nút tổng kết bệnh án sẽ hiện thị form theo tham số

		![image](https://github.com/user-attachments/assets/2d3c2101-641f-4602-886b-29a4bf2a8a87)

		Mô tả và hướng dẫn sử dụng [Mô tả bổ sung dữ liệu](https://github.com/dh-hos/Mo-ta-he-thong/blob/main/Vuong-mo-ta-tom-tat-BA-theo-tt32.md)
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/467
## [v.4.24.0731.0]()

- 🐛: Fix Lỗi - Khi bấm vào nút Phẫu Thuật #250
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/250
## [v.4.24.0730.1]()
- ✨: Fix chưa hỗ trợ TOA XUẤT VIỆN nội trú theo thứ tự nhập số lượng -> sáng -> trưa -> chiều -> tối . hiện tại nhập số lượng bấm enter (tab, mũi tên sang phải) thì tới chỉ định dùng thuốc
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/523
## [v.4.24.0730.0]()
- ✨: Fix chưa hỗ trợ thứ tự nhập số lượng -> sáng -> trưa -> chiều -> tối . hiện tại nhập số lượng bấm enter (tab, mũi tên sang phải) thì tới chỉ định dùng thuốc
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/523
## [v.4.24.0729.2]()
- ✨: Treatment thực hiện chức năng để lưu thêm thông tin, ttcon.lan_sinh,sinhcon_phauthuat,sinhcon_duoi32tuan#206
- ☑: https://github.com/dh-hos/Yeu_cau_ho_tro/issues/206
- ✨: Yêu cầu - Hoàn thiện XML9 #198
- ☑: https://github.com/dh-hos/Yeu_cau_ho_tro/issues/198
	- Cập nhật form thông tin con:
		- Bổ sung lần sinh: nhận giá trị số
		- Bổ sung Phẫu thuật khi sinh con: 0 (sinh con không phải phẫu thuật); 1 (sinh con phải phẫu thuật)
		- Bổ sung Sinh con dưới 32 tuần tuổi: 0 (Không sinh con dưới 32 tuần tuổi); 1 (sinh con dưới 32 tuần tuổi)
- ✨: Phần mềm Treatment, Prescription lỗi khi nhập liều dùng có 2 số lẻ thập phân #523
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/523
	- Cập nhật form ra toa:
		- Hiển thị 2 số lẻ (sáng, trưa, chiều, tối)
		- Nhập theo thứ tự: số lướng -> sáng -> trưa -> chiều -> tối
		![image](https://github.com/user-attachments/assets/18198044-fe2e-4f3c-8911-46595404e9c5)
## [v.4.24.0729.1]()
- 🐛: Lỗi - KHÔNG THÊM ĐƯỢC BUỒNG - MÃ GIƯỜNG KHI ĐỔI HAY CHỈNH DIỄN BIẾN #249
	- Cập nhật: buồng có thể trống hoặc nhập đúng theo danh mục buồng; giường không thể để trống --> phải nhập theo danh mục
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/249
## [v.4.24.0729.0]()

- 🐛: Fix LỖI HIỂN THỊ THIẾU TÊN XÃ 1 SỐ ĐỊA PHƯƠNG #247
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/247

- 🐛: Lỗi - KHÔNG THÊM ĐƯỢC BUỒNG - MÃ GIƯỜNG KHI ĐỔI HAY CHỈNH DIỄN BIẾN #249
	- Cập nhật: buồng, giường có thể trống hoặc nhập đúng theo danh mục buồng, giường 
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/249

## [v.4.24.0726.0]()
- 🐛: Fix lỗi thể hiện, và thêm yêu cầu ghi nhận nhật ký thay đổi lại ⌛Dự kiến: 2024-07-26 #534
	 - Cập nhật lỗi:
	 ![image](https://github.com/user-attachments/assets/f65b1ea5-f789-429e-84c1-492df65e18d2)
	 - Ghi nhật ký:
	 ![image](https://github.com/user-attachments/assets/352573f1-7324-4efb-86b5-9f2721a3c2ea)
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/534

- 🐛: Fix Lỗi - Hiển thị sai giờ bắt đầu và giờ kết thúc các phiếu TT/PT đã lập #248
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/248
## [v.4.24.0725.0]()
- 🐛: Fix lỗi - Treatment không hiển thị được nút Chuyển viện Lao khi Xử trí Không phải Chuyển viện (Đặc thù BV Phổi Đồng Tháp) #246
	- Cập nhật: nút chuyển viện lao không phụ thuộc xử trí
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/246
## [v.4.24.0724.0]()
- ✨: Thực hiện - Treatment hỗ trợ chức năng nhập Diễn biến, Tóm tắt KQ CLS các hồ sơ đã ra viện
	- Bổ sung chức năng:
	![image](https://github.com/user-attachments/assets/a4335cfb-d1be-4f4d-bb4f-d4730bce9c24)

	![image](https://github.com/user-attachments/assets/6cc42c9c-5f9a-468f-8b66-0ec0e9e8e0ac)

	Người dùng tự nhập vào hoặc nhấn nút (...) để hỗ trợ tóm tắt kết quả CLS
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/502
- ✨: Yêu cầu - BV QDY CT: Hỗ trợ chức năng nhập Diễn biến và tóm tắt kết quả CLS cho các bệnh án nội trú, BANT theo đợt cũ đã xuất viện để gửi dữ liệu XML8 QT_BENHLY và TOMTAT_KQ #501
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/501
- ✨: Yêu cầu: Treatment không kiểm tra độ dài tóm tắt kết quả CLS
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/517

## [v.4.24.0723.1]()
- ✨: Yêu cầu - QDY CT: Treatment bỏ giới hạn 400 ký tự tóm tắt kết quả CLS (QĐ 4750 không giới hạn số ký tự) #516
	- Bỏ giới hạn 400 ký tự
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/516
## [v.4.24.0723.0]()

- 🐛: FIx lỗi - Bệnh nhân chỉ có năm sinh khi in cấp lại giấy chứng sinh thì có ngày tháng sinh #243
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/243

- 🐛: FIx lỗi - IN PHIẾU CHỈ ĐỊNH CLS BÁO LỖI #244
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/244
## [v.4.24.0722.0]()
- ✨: Treatment - RÀNG BUỘC KHÔNG BỎ TRỐNG HƯỚNG ĐIỀU TRỊ CHO GIẤY CHUYỂN TUYẾN #506
- ✨: Yêu cầu - RÀNG BUỘC KHÔNG BỎ TRỐNG HƯỚNG ĐIỀU TRỊ CHO GIẤY CHUYỂN TUYẾN #504
	- Cập nhật không để trống hướng điều trị trên giấy chuyển tuyến
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/506
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/504

- ✨: Yêu cầu - Treatment - Ràng buộc không bỏ trống phương tiện vận chuyển khi lập phiếu chuyển tuyến
- ✨: Yêu cầu - Ràng buộc không bỏ trống phương tiện vận chuyển khi lập phiếu chuyển tuyến #510
	- Cập nhật không để trống phương tiện vận chuyển trên giấy chuyển tuyến
- ☑: https://github.com/dh-hos/THEO-DOI-THUC-HIEN-4750/issues/78
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/510
## [v.4.24.0720.0]()
- ✨: Treatment mới lỗi khi chỉnh diễn biến ở BV QDY CT #499
		- Fix lỗi khi sử dụng tham số nt.capnhat_dienbien > 0 và PostgreSQL phiên bản <= 9.5
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/499
- ✨: Yêu cầu - Hỗ trợ thao tác nhập Tóm tắt kết quả CLS #473
		- Fix lỗi lấy tóm tắt CLS
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/473
## [v.4.24.0719.0]()
- ✨: Yêu cầu: BV Nghĩa Hành - Treatment cho phép chọn ngày bắt đầu-kết thúc PT-TT và tháng kế toán cũ để lập phiếu PT-TT cho CLS PT-TT tháng cũ chưa lập phiếu #488
	- Bổ sung tham số: nt.lap_phieuttpt (Nội trú: lập phiếu thủ thuật - phẫu thuật theo:)
		- 0: Tháng hiện tại (mặc định) (giới hạn theo ngày bắt đầu và kế thúc trong tháng kế toán)
		- 1: Thời gian điều trị của bệnh nhân ( giới hạn từ ngày nhập viện và kết thúc tháng kế toán hiện tại)

- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/488
## [v.4.24.0718.2]()
- 🐛: Fix lỗi - Xem kết quả xét nghiệm Hóa sinh máu có cấu hình lên mẫu chuẩn #242 https://github.com/dh-hos/dhg.hosptaltreatment/issues/242
- ☑: 
## [v.4.24.0718.1]()
- 🐛: Fix lỗi: không load tình hình phẫu thuật (form lập phiếu phẫu thuật)

## [v.4.24.0718.0]()
- 🐛: Fix lỗi: không load tình hình phẫu thuật (form lập phiếu phẫu thuật)
## [v.4.24.0717.3]()
- ✨: Thực hiện [Treatment] kiểm tra số lượng ICD theo tham số khi thực hiện theo [Mô tả XML130 - Bổ sung QĐ 4750]
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/481

- ✨: Thực hiện gởi tối đa 12 ICD #479
	- Bổ sung tham số ma_benh_kt.soluong.
		- Treatment ⇒ Kiểm tra số lượng mã ICD10 khi sử dụng tham số ma_benh_kt.soluong để thay đổi diễn biến bệnh.
		- Nếu ma_benh_kt.soluong > 0
			- Kiểm tra Mã ICD phụ > ma_benh_kt.soluong ==> Cảnh báo và KHÔNG lưu diễn biến bệnh
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/479
- ☑: https://github.com/dh-hos/To_Ho_Tro/issues/20
- ☑: https://github.com/dh-hos/To_Trien_Khai/issues/57
## [v.4.24.0717.2]()
- ✨: Thực hiện - Treatment: Bổ sung chức năng hỗ trợ lấy dữ liệu [Tóm tắt kết quả CLS] ⏳Dự kiến : 2024-07-19 #475
	 - Bổ sung chức năng tóm tắt kế quả CLS khi ra viện
		- Khi ra viện: tự động load tóm tắt (1) khi tóm tắt chưa có hoặc tự load nút số (2)
		- Kiểm tra số ký tự tóm tắt: nếu vượt quá 400 sẽ không cho lưu
		- Chức năng đổi diễn biến: kiểm tra mã ICD có vượt quá 12 không? nếu vượt không cho lưu
		![image](https://github.com/user-attachments/assets/d44570da-c726-4086-b2ff-040deaac34e9)
		
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/475

- ✨: Yêu cầu - Hỗ trợ thao tác nhập Tóm tắt kết quả CLS #473
		
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/473
## [v.4.24.0717.1]()
- ✨: Thực hiện - Treatment: Bổ sung chức năng hỗ trợ lấy dữ liệu [Tóm tắt kết quả CLS] ⏳Dự kiến : 2024-07-19 #475
	 - Bổ sung chức năng tóm tắt kế quả CLS khi ra viện
		- Khi ra viện: tự động load tóm tắt (1) khi tóm tắt chưa có hoặc tự load nút số (2)
		- Kiểm tra số ký tự tóm tắt: nếu vượt quá 400 sẽ không cho lưu
		- Chức năng đổi diễn biến: kiểm tra mã ICD có vượt quá 12 không? nếu vượt không cho lưu
		![image](https://github.com/user-attachments/assets/d44570da-c726-4086-b2ff-040deaac34e9)
		
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/475

- ✨: Yêu cầu - Hỗ trợ thao tác nhập Tóm tắt kết quả CLS #473
		
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/473
## [v.4.24.0717.0]()
- 🐛: Fix lỗi - cân nặng ra viện không hiển thị được lên trang in.
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/482
![](https://i.imgur.com/KKNhyIp.png)

## [v.4.24.0716.0]()
- ✨: Yêu cầu - Treatment có tham số chặn khi diễn biến bị trống #466
		- Cập nhật: kiểm tra lưu diễn biến không được để trống hoặc nhập nhiều hơn 2000 ký tự
		![image](https://github.com/user-attachments/assets/d60694fb-f56a-4711-b2ee-0f68a8ee3e7a)
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/466
## [v.4.24.0715.0]()
- 🐛: Fix lỗi: Treatment 13/07 không tìm thấy CLS để lập phiếu phẫu thuật, thủ thuật #487
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/487
## [v.4.24.0713.0]()
- ✨: Yêu cầu - PK Medic Miền Đông: Không cấu hình loại PT trên danh mục CLS vẫn lập được phiếu PT-TT #435
	- Thực hiện theo mô tả: https://github.com/dh-hos/Mo-ta-he-thong/blob/main/Mô%20tả%20thực%20hiện%20Thủ%20thuật-Phẫu%20thuật%20đối%20với%20Cận%20lâm%20sàng.md
		--> Lập phiếu thủ thuật phẫu thuật: theo tham số phanloaipt.thuchien
		--> Sổ phẫu thuật thủ thuật: theo tham số phanloaipt.baocao
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/435

- ✨: Yêu cầu - BV QDY CT: thêm tham số ràng buộc thời gian bắt đầu và kết thúc phiếu thủ thuật phẫu thuật lớn hơn thời gian chỉ định #456
	--> Thêm: thời gian kết thúc phẫu thuật > thời gian bắt đầu phẫu thuật ít nhất 5 phút
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/456
## [v.4.24.0712.1]()
- 🐛: fix lỗi - Tính giá trị dinh dưỡng chưa đúng
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/482
## [v.4.24.0712.0]()
- ✨: Yêu cầu bổ sung chức năng nhập liều dùng đối với chức năng ra toa ngoại trú - BN nội trú #430
	- Fix lỗi khi vào xem lại không load được liều dùng đã nhập
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/430
## [v.4.24.0711.0]()
- 🐛: Fix Lỗi - CHỨC NĂNG QT ĐIỀU TRỊ VẪN CHỈNH ĐƯỢC SAU KHI ĐÃ KẾT THÚC BỆNH ÁN #237
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/237

- 🐛: Fix Lỗi - Trả toa thu phí bị lỗi #241
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/241

- 🐛: Fix Lỗi - Form khám và điều trị không hiển thị hết thông tin sinh hiêu (BV Thốt Nốt) #238
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/238


## [v.4.24.0710.1]()

- 🐛: Fix Lỗi - Không lưu được thông tin phường xã 4750 #240
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/240

- 🐛: Fix Lỗi - Treatment chỉnh thông tin bệnh nhân trường Phường xã không lấy theo địa chỉ 4750 #239
	  --> Đồng bộ 2 form sẽ cập nhật sau, đáp ứng chỉnh thông tin của bệnh viện trước
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/239
## [v.4.24.0710.0]()
- 🐛: Fix Lỗi - KHÔNG LOAD TÓM TẮT KẾT QUẢ CLS KHI VÀO LẠI FORM KẾT THÚC ĐIỀU TRỊ #236
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/236
## [v.4.24.0709.1]()

- 🐛: Fix Lỗi - BN CÓ MÃ ĐKBĐ ĐĂNG KÝ ĐÚNG NƠI ĐKBĐ PHIẾU 01 CHECK SAI THÔNG TUYẾN #235
	![image](https://github.com/dh-hos/dhg.hosptaltreatment/assets/32563776/d0d0c674-5d7a-4a91-8ac2-4618b0b93966)
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/235
## [v.4.24.0709.0]()
- ✨: XML14.ngay_hen_kl #48
	 - Phiếu hẹn tái khám: bổ sung cho người dùng điều chỉnh ngày giờ hẹn (mặc định 8:00 giờ)

	 ![image](https://github.com/dh-hos/THEO-DOI-THUC-HIEN-4750/assets/32563776/8f1095bf-06f2-4dc7-be53-50dc3b37e2fb)

- ☑: https://github.com/dh-hos/THEO-DOI-THUC-HIEN-4750/issues/48
## [v.4.24.0708.0]()

- 🐛: Fix lỗi: Form chỉnh thông tin chổ nút [...] enter lên danh sách thì load theo 4750 đã ok, nhưng khi gõ viết tắt thì giá trị gõ vào ko có trong 4750 nhưng phần mềm vẫn cho enter chọn và vẫn cho lưu
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/449

- 🐛: Fix lỗi: Lỗi - Khuất nội dung khi lập phiếu TT/PT #234
	- Setup form về chuẩn: 1024x768
- ☑: https://github.com/dh-hos/dhg.hosptaltreatment/issues/234
## [v.4.24.0707.0]()
- ✨: Treatment Chức năng hiệu chỉnh thông tin chưa chỉnh theo danh mục địa phương 4750 #449
	- Chức năng chỉnh thông tin: FIX lỗi chỉnh phường xã chưa lấy được danh mục địa phương 4750
	- Chỉnh thông tin tại Form khám và điều trị không chỉnh được Phường xã: Fix lỗi không load được danh được danh mục phường xã theo 4750
- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/449
## [v.4.24.0705.1]()
- ✨: Yêu cầu - Khi lập phiếu PT, TT tại Prescription và Treatment bắt buộc phải nhập Ekip mới cho lưu. #432
	- Fix lỗi không xóa được ekip

- ✨: Treatment bổ sung mamay khi thực hiện ghi nhận phiếu PT,TT #35
	- Bổ sung chức năng: ghi nhận mã máy vào phẫu thuật/thủ thuật
	- phauthuat.mamay = dmmamay.mamay
	![image](https://github.com/dh-hos/THEO-DOI-THUC-HIEN-4750/assets/32563776/19ef8506-4e51-4560-af50-bd4494843ac3)
	
	Hiện thị danh mục mã máy kho cận lâm sàng
	![image](https://github.com/dh-hos/THEO-DOI-THUC-HIEN-4750/assets/32563776/5d10bf03-078a-40c3-b32a-4cf7e281ea30)

	![image](https://github.com/dh-hos/THEO-DOI-THUC-HIEN-4750/assets/32563776/9452e9a0-4175-4db7-8071-5a18acff3752)

	- Bổ sung chức năng tóm tắt kết quả CLS có giá trị chẩn đoán vào form xuất viện (cột này là bắt buột nhập, hỗ trợ xuất xml8 )

	![image](https://github.com/dh-hos/THEO-DOI-THUC-HIEN-4750/assets/32563776/25861284-4410-48a5-a2bc-96023ab8f635)

- ☑: https://github.com/dh-hos/To_Lap_Trinh/issues/432
- ☑: https://github.com/dh-hos/THEO-DOI-THUC-HIEN-4750/issues/35
- ☑: https://github.com/dh-hos/To_Ho_Tro/issues/20
- ☑: https://github.com/dh-hos/To_Trien_Khai/issues/57
## [v.4.24.0705.0]()
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
