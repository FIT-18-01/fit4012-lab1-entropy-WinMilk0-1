# Report 1 Page – FIT4012 Lab 1

## 1. Mục tiêu
Tóm tắt ngắn gọn mục tiêu của bài lab.

## 2. Cách làm
- Đọc hiểu chương trình entropy mẫu.
- Bổ sung hàm tính redundancy.
- Hoàn thiện hàm mod_inverse().
- Chạy thử trên nhiều test case.

## 3. Kết quả chính
### 3.1 Entropy và redundancy
| Input | Entropy | Redundancy | Nhận xét |
|---|---:|---:|---|
| aaaa | 0 | 8 | Chuỗi chỉ có 1 ký tự duy nhất, entropy = 0, redundancy = log2(256) - 0 = 8 |
| abcd | 2 | 6 | 4 ký tự khác nhau, mỗi ký tự xuất hiện 1 lần, entropy = 2, redundancy = 8 - 2 = 6 |
| hello world | 2.844 | 5.156 | Chuỗi có 11 ký tự với các tần suất khác nhau, entropy ≈ 2.844, redundancy ≈ 5.156 |

### 3.2 Modulo inverse
| a | m | Kết quả mong đợi | Kết quả chương trình |
|---:|---:|---|---|
| 3 | 7 | 5 | 5 |
| 10 | 17 | 12 | 12 |
| 6 | 9 | Không tồn tại | -1 |

## 4. Kết luận
Từ bài lab này, em học được cách tính entropy của một chuỗi ký tự và độ dư thừa thông tin dựa trên entropy. Khó khăn lớn nhất là hiểu và cài đặt hàm mod_inverse sử dụng thuật toán Euclid mở rộng. Việc thực hành giúp em hiểu rõ hơn về entropy như một thước đo độ bất định của thông tin và ứng dụng của nghịch đảo modulo trong mật mã.
