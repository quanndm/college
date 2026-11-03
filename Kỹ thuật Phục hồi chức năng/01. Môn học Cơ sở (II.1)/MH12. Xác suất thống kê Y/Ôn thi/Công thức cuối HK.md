# BẢNG CÔNG THỨC XÁC SUẤT – THỐNG KÊ (CHƯƠNG 4–7)

---

# CHƯƠNG 4. LÝ THUYẾT MẪU

## 1. Các ký hiệu cơ bản

- N: Kích thước tổng thể.
    
- n: Kích thước mẫu.
    
- X̄: Trung bình mẫu.
    
- μ: Trung bình tổng thể.
    
- S²: Phương sai mẫu.
    
- S*: Độ lệch chuẩn mẫu hiệu chỉnh.
    
- σ²: Phương sai tổng thể.
    
- σ: Độ lệch chuẩn tổng thể.
    
- p̂: Tỷ lệ mẫu.
    

## 2. Trung bình mẫu

X̄ = (X₁ + X₂ + ... + Xₙ) / n

Hoặc:

X̄ = ΣXᵢ / n

## 3. Phương sai mẫu

Phương sai mẫu không hiệu chỉnh:

S² = Σ(Xᵢ − X̄)² / n

Công thức tính nhanh:

S² = ΣXᵢ² / n − X̄²

Phương sai mẫu hiệu chỉnh:

S*² = Σ(Xᵢ − X̄)² / (n − 1)

Mối liên hệ:

S*² = [n / (n − 1)] × S²

Độ lệch chuẩn mẫu hiệu chỉnh:

S* = √S*²

## 4. Tỷ lệ mẫu

p̂ = m / n

Trong đó:

- m: Số phần tử có tính chất cần xét.
    
- n: Kích thước mẫu.
    

## 5. Sai số chuẩn

Sai số chuẩn của trung bình mẫu:

SE(X̄) = σ / √n

Khi chưa biết σ, có thể ước lượng bằng:

SE(X̄) ≈ S* / √n

Sai số chuẩn của tỷ lệ mẫu:

SE(p̂) = √[p(1 − p) / n]

Khi chưa biết p, có thể thay bằng p̂:

SE(p̂) ≈ √[p̂(1 − p̂) / n]

---

# CHƯƠNG 5. ƯỚC LƯỢNG THAM SỐ

## 1. Ước lượng điểm

|Tham số tổng thể|Ước lượng điểm|
|---|---|
|Trung bình μ|X̄|
|Tỷ lệ p|p̂|
|Phương sai σ²|S*²|

## 2. Các giá trị tới hạn thường dùng

- Zα/2: Giá trị tới hạn của phân phối chuẩn tắc.
    
- tα/2(n−1): Giá trị tới hạn của phân phối Student với n−1 bậc tự do.
    
- χ²α/2(n−1): Giá trị tới hạn của phân phối Chi bình phương với n−1 bậc tự do.
    

**Lưu ý:** Trong phần công thức Chi bình phương dưới đây, χ²α(n−1) được hiểu là phân vị phía trái, tức P(χ² ≤ χ²α) = α.

## 3. Khoảng tin cậy cho trung bình μ

### Trường hợp 1: Biết phương sai tổng thể σ²

Khoảng tin cậy:

X̄ − Zα/2 × σ/√n < μ < X̄ + Zα/2 × σ/√n

### Trường hợp 2: Không biết phương sai tổng thể σ²

Sử dụng phân phối Student:

X̄ − tα/2(n−1) × S*/√n < μ < X̄ + tα/2(n−1) × S*/√n

## 4. Khoảng tin cậy cho tỷ lệ p

Khoảng tin cậy xấp xỉ:

p̂ − Zα/2 × √[p̂(1 − p̂)/n] < p < p̂ + Zα/2 × √[p̂(1 − p̂)/n]

## 5. Khoảng tin cậy cho phương sai σ²

Với tổng thể có phân phối chuẩn:

[(n−1)S_²] / χ²1−α/2(n−1) < σ² < [(n−1)S_²] / χ²α/2(n−1)

## 6. Xác định kích thước mẫu

### Ước lượng trung bình

Khi biết σ:

n ≥ (Zα/2 × σ / ε)²

Trong đó:

- ε: Sai số ước lượng cho phép.
    
- σ: Độ lệch chuẩn tổng thể.
    

### Ước lượng tỷ lệ

n ≥ Zα/2² × p(1 − p) / ε²

Nếu chưa biết p, thường lấy p = 0,5 để có kích thước mẫu lớn nhất:

n ≥ Zα/2² / (4ε²)

---

# CHƯƠNG 6. KIỂM ĐỊNH GIẢ THUYẾT

## 1. Các khái niệm cơ bản

- H₀: Giả thuyết không.
    
- H₁: Giả thuyết đối.
    
- α: Mức ý nghĩa.
    
- β: Xác suất mắc sai lầm loại II.
    
- 1 − β: Lực kiểm định.
    

Hai loại sai lầm:

- Sai lầm loại I: Bác bỏ H₀ khi H₀ đúng. Xác suất mắc sai lầm là α.
    
- Sai lầm loại II: Không bác bỏ H₀ khi H₀ sai. Xác suất mắc sai lầm là β.
    

## 2. Các dạng giả thuyết đối

|Dạng kiểm định|Giả thuyết đối H₁|
|---|---|
|Hai phía|μ ≠ μ₀|
|Phía phải|μ > μ₀|
|Phía trái|μ < μ₀|

## 3. Kiểm định trung bình tổng thể μ

### Trường hợp 1: Biết phương sai tổng thể σ²

Thống kê kiểm định:

Z = (X̄ − μ₀) / (σ/√n)

Miền bác bỏ H₀:

- Hai phía: |Z| > Zα/2
    
- Phía phải: Z > Zα
    
- Phía trái: Z < −Zα
    

### Trường hợp 2: Không biết phương sai tổng thể σ²

Thống kê kiểm định:

T = (X̄ − μ₀) / (S*/√n)

Miền bác bỏ H₀:

- Hai phía: |T| > tα/2(n−1)
    
- Phía phải: T > tα(n−1)
    
- Phía trái: T < −tα(n−1)
    

## 4. Kiểm định tỷ lệ tổng thể p

Giả thuyết:

H₀: p = p₀

Thống kê kiểm định:

Z = (p̂ − p₀) / √[p₀(1 − p₀)/n]

Miền bác bỏ H₀:

- Hai phía: |Z| > Zα/2
    
- Phía phải: Z > Zα
    
- Phía trái: Z < −Zα
    

## 5. Kiểm định hiệu hai trung bình μ₁ − μ₂

### Trường hợp 1: Biết phương sai hai tổng thể

Thống kê kiểm định:

Z = [ (X̄₁ − X̄₂) − (μ₁ − μ₂)₀ ] / √(σ₁²/n₁ + σ₂²/n₂)

Nếu H₀: μ₁ = μ₂ thì:

Z = (X̄₁ − X̄₂) / √(σ₁²/n₁ + σ₂²/n₂)

### Trường hợp 2: Không biết phương sai, giả sử hai phương sai bằng nhau

Phương sai gộp:

Sp² = [(n₁ − 1)S₁_² + (n₂ − 1)S₂_²] / (n₁ + n₂ − 2)

Thống kê kiểm định:

T = [ (X̄₁ − X̄₂) − (μ₁ − μ₂)₀ ] / [Sp × √(1/n₁ + 1/n₂)]

Bậc tự do:

df = n₁ + n₂ − 2

## 6. Kiểm định hiệu hai tỷ lệ p₁ − p₂

Khi kiểm định:

H₀: p₁ = p₂

Tỷ lệ gộp:

p̂ = (m₁ + m₂) / (n₁ + n₂)

Thống kê kiểm định:

Z = (p̂₁ − p̂₂) / √[p̂(1 − p̂)(1/n₁ + 1/n₂)]

Trong đó:

- p̂₁ = m₁/n₁
    
- p̂₂ = m₂/n₂
    

## 7. Phương pháp giá trị p-value

Quy tắc quyết định:

- Nếu p-value ≤ α: Bác bỏ H₀.
    
- Nếu p-value > α: Không bác bỏ H₀.
    

---

# CHƯƠNG 7. TƯƠNG QUAN VÀ HỒI QUY TUYẾN TÍNH

## 1. Hiệp phương sai mẫu

Cov(X,Y) = Σ[(Xᵢ − X̄)(Yᵢ − Ȳ)] / (n − 1)

## 2. Hệ số tương quan Pearson

r = Cov(X,Y) / (Sₓ × Sᵧ)

Trong đó:

- Sₓ: Độ lệch chuẩn mẫu của X.
    
- Sᵧ: Độ lệch chuẩn mẫu của Y.
    

Giá trị của hệ số tương quan:

−1 ≤ r ≤ 1

Ý nghĩa:

- r > 0: Tương quan thuận.
    
- r < 0: Tương quan nghịch.
    
- r ≈ 0: Tương quan tuyến tính yếu hoặc không có tương quan tuyến tính.
    
- |r| càng gần 1: Mối tương quan tuyến tính càng mạnh.
    

## 3. Phương trình hồi quy tuyến tính

Dạng phương trình:

Ŷ = aX + b

Trong đó:

- a: Hệ số góc.
    
- b: Hệ số chặn.
    
- Ŷ: Giá trị dự đoán của Y.
    

## 4. Phương pháp bình phương tối thiểu

Mục tiêu:

Σ(Yᵢ − Ŷᵢ)² → min

Hệ số góc:

a = Σ[(Xᵢ − X̄)(Yᵢ − Ȳ)] / Σ(Xᵢ − X̄)²

Hệ số chặn:

b = Ȳ − aX̄

Công thức tính nhanh:

a = [nΣXᵢYᵢ − ΣXᵢΣYᵢ] / [nΣXᵢ² − (ΣXᵢ)²]

b = Ȳ − aX̄

## 5. Hệ số xác định R²

R² = r²

Công thức tổng quát:

R² = 1 − [Σ(Yᵢ − Ŷᵢ)² / Σ(Yᵢ − Ȳ)²]

Ý nghĩa:

R² biểu thị tỷ lệ biến thiên của Y được giải thích bởi mô hình hồi quy tuyến tính.

---

# GHI NHỚ NHANH KHI LÀM BÀI

|Dạng bài|Công thức / Phân phối cần nhớ|
|---|---|
|Trung bình mẫu|X̄ = ΣXᵢ/n|
|Phương sai mẫu|S² = Σ(Xᵢ − X̄)²/n|
|Phương sai hiệu chỉnh|S*² = Σ(Xᵢ − X̄)²/(n−1)|
|Ước lượng trung bình, biết σ|Z|
|Ước lượng trung bình, không biết σ|Student t|
|Ước lượng tỷ lệ|Z|
|Ước lượng phương sai|Chi bình phương χ²|
|Kiểm định trung bình, biết σ|Z|
|Kiểm định trung bình, không biết σ|Student t|
|Kiểm định tỷ lệ|Z|
|So sánh hai trung bình|Z hoặc t tùy giả thiết|
|So sánh hai tỷ lệ|Z|
|Tương quan|Pearson r|
|Hồi quy tuyến tính|Ŷ = aX + b|

## Những điểm dễ nhầm

1. Phương sai mẫu S² chia cho n; phương sai mẫu hiệu chỉnh S*² chia cho n−1.
    
2. Khi kiểm định hoặc ước lượng trung bình mà không biết σ, thường dùng S* và phân phối Student t nếu các giả thiết phù hợp.
    
3. Ước lượng phương sai tổng thể sử dụng phân phối Chi bình phương khi tổng thể có phân phối chuẩn.
    
4. Kiểm định hai phía sử dụng α/2 ở mỗi phía; kiểm định một phía sử dụng α ở một phía.
    
5. Kiểm định hai mẫu độc lập khác với kiểm định mẫu ghép cặp.
    
6. Công thức t gộp ở Chương 6 giả định hai tổng thể độc lập, phân phối chuẩn và có phương sai bằng nhau. Nếu phương sai không bằng nhau, cần công thức Welch.
    
7. Tương quan không đồng nghĩa với quan hệ nhân quả.
    
8. R² = r² trong hồi quy tuyến tính đơn có hệ số chặn.