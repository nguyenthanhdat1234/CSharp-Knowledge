# CSharp-Knowledge

# RESTful API 


## 1 - Giao thức giao tiếp
 Giao thức giao tiếp giữa API và người dùng luôn sử dụng giao thức HTTPs

## 2 - Tên miền 
*https://api.example.com

OR

* https:example.org/api/

# 3 - Phiên bản 
https://api.example.com/v1/
https://api.exaple.com/v2/


# 4 - Điểm cuối (Endpoint)

* https://api.example.com/v1/zoos

# 5 - Options HTTP

* GET (SELECT)
* CREATE (CREATE)
* PUT (UPDATE)
* PATCH (UPDATE) 
* DELETE (DELETE)

AND

* HEAD: Lấy siêu dữ liệu của tài nguyên

# 6 - Filtering

?limit=10: Chỉ đinh số lượng bản ghi được trả về 
?offset=10: chỉ định vị trí bắt đầu của bản ghi được trả về 
?page=2&per_page=100: chỉ định số trang và số lượng bản ghi trên mỗi trang
?sortby=name&order=asc: chỉ đinh thuộc tính naò để sắp xếp các kết quả trả về và thứ tự sắp xếp

# 7 - Return status 

200: Máy chỉ trả về thành công dữ liệu do người dùng yêu cầu
201 CREATE - [POST / PUT / PATCH]: Người dùng đã taoj hoăjc sửa đổi dữ liệu thành công.
202 Được chấp nhận. Cho biết một yêu câuf đã vào hàng đợi nền( tác vụ không đồng bộ)
204 KHÔNG CÓ NỌI DUNG - [XÓA: Người undgf đã xóa thành công dữ liệu
404 YÊU CẦU KHÔNG HỢP LỆ. Có lỗi trong yêu cầu do người dùng gửi và máy chủ chưa thực hiện thao tác tạo và sửa đổi dữ liệu