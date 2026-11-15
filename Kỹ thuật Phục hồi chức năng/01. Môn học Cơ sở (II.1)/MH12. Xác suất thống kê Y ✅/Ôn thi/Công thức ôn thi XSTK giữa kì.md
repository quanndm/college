# 📑 CHƯƠNG 1: BIẾN CỐ NGẪU NHIÊN VÀ PHÉP TÍNH XÁC SUẤT

## 1. Định nghĩa xác suất cổ điển

$$  
P(A) = \frac{m}{n} = \frac{|A|}{|\Omega|}  
$$

- (m): Số kết quả thuận lợi cho biến cố (A).
    
- (n): Tổng số kết quả đồng khả năng trong không gian mẫu Ω.
    
## 2. Các công thức giải tích tổ hợp (Bấm máy tính)

- **Hoán vị** (Xếp (n) phần tử vào (n) vị trí có thứ tự):
    
    $$P_n = n!$$
    
- **Chỉnh hợp** (Chọn (k) từ (n) phần tử, **có** thứ tự):
    
    $$A_n^k = \frac{n!}{(n-k)!}$$
    
- **Tổ hợp** (Chọn (k) từ (n) phần tử, **không** thứ tự):
    
    $$C_n^k = \frac{n!}{k!(n-k)!}$$
    

## 3. Công thức cộng xác suất

- **Tổng quát:**
    
    $$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$
    
- **Nếu (A) và (B) xung khắc**:  **A∩B=∅**
    
    $$P(A \cup B) = P(A) + P(B)$$
    
- **Biến cố đối:**
    
    $$P(\overline{A}) = 1 - P(A)$$
    

## 4. Công thức nhân xác suất

- **Tổng quát (Xác suất có điều kiện):**
    
    $$P(A \cap B) = P(A) \cdot P(B|A) = P(B) \cdot P(A|B)$$
    
- **Nếu (A) và (B) độc lập:**
    
    $$P(A \cap B) = P(A) \cdot P(B)$$
    
- _Mẹo tính nhanh hệ độc lập:_
    
    $$P(A_1 \cup A_2 \cup \dots \cup A_n) = 1 - P(\overline{A_1} \cap \overline{A_2} \cap \dots \cap \overline{A_n})$$
    

## 5. Công thức xác suất đầy đủ và công thức Bayes

_Áp dụng khi bài toán chia làm 2 giai đoạn: Giai đoạn 1 là các giả thuyết (A_i), giai đoạn 2 là kết quả (B)._

- **Công thức xác suất đầy đủ:**
    
    $$P(B) = \sum_{i=1}^{n} P(A_i) \cdot P(B|A_i)$$
    
- **Công thức Bayes (Tính xác suất nguyên nhân):**
    
    $$P(A_k|B) = \frac{P(A_k) \cdot P(B|A_k)}{P(B)}$$
    

## 6. Công thức Bernoulli (Phép thử lặp)

Xác suất để trong (n) phép thử độc lập, biến cố (A) (có xác suất xảy ra cố định là (p)) xuất hiện đúng (k) lần:

$$  
P_n(k) = C_n^k \cdot p^k \cdot q^{n-k}  
\quad \text{(với } q = 1-p\text{)}  
$$

---

# 📊 CHƯƠNG 2: BIẾN NGẪU NHIÊN VÀ CÁC ĐẶC TRƯNG SỐ

## 1. Biến ngẫu nhiên rời rạc (Bảng phân phối xác suất)

- **Điều kiện bảng phân phối:**
    
    $$\sum_{i=1}^{n} p_i = 1$$
    
- **Kỳ vọng (Giá trị trung bình):**
    
    $$E(X) = \sum_{i=1}^{n} x_i p_i$$
    
- **Phương sai:**
    
    $$V(X) = E(X^2) - [E(X)]^2$$
    
    Trong đó:
    
    $$E(X^2) = \sum_{i=1}^{n} x_i^2 p_i$$
    

## 2. Biến ngẫu nhiên liên tục (Hàm mật độ (f(x)))

- **Điều kiện hàm mật độ:**
    
    $$\int_{-\infty}^{+\infty} f(x),dx = 1$$
    
- **Xác suất trên một khoảng:**
    
    $$P(a < X < b) = \int_a^b f(x),dx$$
    
- **Kỳ vọng:**
    
    $$E(X) = \int_{-\infty}^{+\infty} x \cdot f(x),dx$$
    
- **Phương sai:**
    
    $$V(X) = \int_{-\infty}^{+\infty} x^2 \cdot f(x),dx - [E(X)]^2$$
    

## 3. Tính chất của kỳ vọng và phương sai (Rất hay bẫy lý thuyết)

**Tính chất kỳ vọng:**
     
- $E(C) = C$
    
- $E(CX) = C \cdot E(X)$
    
- $E(X + Y) = E(X) + E(Y)$
    
- $E(X - Y) = E(X) - E(Y)$

**Tính chất phương sai:**
- $V(C) = 0$
    
- $V(CX) = C^2 \cdot V(X)$
    
- Nếu $X, Y$ độc lập:    
    $$V(X - Y) = V(X) + V(Y)$$
    _Lưu ý: Phương sai của tổng hoặc hiệu hai biến ngẫu nhiên độc lập đều là tổng hai phương sai._
- **Độ lệch chuẩn:**
    $$\sigma(X) = \sqrt{V(X)}$$
---

# 📉 CHƯƠNG 3: CÁC QUY LUẬT PHÂN PHỐI XÁC SUẤT THÔNG DỤNG

## 1. Phân phối nhị thức — X ~ B(n, p)

- **Công thức xác suất:**
    
    $$P(X = k) = C_n^k \cdot p^k \cdot q^{n-k}$$
    
- **Đặc trưng số:**
    
    $$E(X) = np \qquad V(X) = npq$$
    
- **Giá trị có khả năng xảy ra nhất (Mode):**
    
    $$np - q \leq \operatorname{Mode}(X) \leq np + p$$
    

## 2. Phân phối Poisson — X ~ P(λ)

- **Công thức xác suất:**
    
    $$P(X = k) = \frac{\lambda^k \cdot e^{-\lambda}}{k!}$$
    
- **Đặc trưng số:**
    
    $$E(X) = V(X) = \lambda$$
    
- _Xấp xỉ nhị thức sang Poisson:_
	Khi $n \geq 30$ và $p \leq 0.1$, có thể xấp xỉ phân phối nhị thức bằng phân phối Poisson với:
    
    $$\lambda = np$$
## 3. Phân phối chuẩn — X ~ N(μ, σ²)
- **Lưu ý quan trọng:**
    
    Khi đề bài cho $X \sim N(\mu, \sigma^2)$:
    
    - $\mu$: Kỳ vọng (giá trị trung bình).
        
    - $\sigma^2$: Phương sai.
        
    - $\sigma$: Độ lệch chuẩn.
        
    
    Do đó, mẫu số khi chuẩn hóa phải là độ lệch chuẩn $\sigma$, không phải phương sai $\sigma^2$.
    
- **Công thức chuẩn hóa:**
    
    $$Z = \frac{X-\mu}{\sigma}$$
    

### 🛑 Cách tính xác suất theo bảng tra phân phối chuẩn

Tùy thuộc vào loại bảng tra ở cuối sách của trường bạn:

**Trường hợp 1: Tính xác suất trong khoảng**

$$P(a < X < b)$$

- Theo bảng Laplace $\Phi(x)$:
    
    $$P(a < X < b) = \Phi\left(\frac{b-\mu}{\sigma}\right) - \Phi\left(\frac{a-\mu}{\sigma}\right)$$
    
- Theo bảng tích lũy $\Psi(x)$ hoặc $F(x)$:
    
    $$P(a < X < b) = \Psi\left(\frac{b-\mu}{\sigma}\right) - \Psi\left(\frac{a-\mu}{\sigma}\right)$$
    

**Trường hợp 2: Tính xác suất một phía - Nhỏ hơn**

$$P(X < b)$$

- Theo bảng Laplace $\Phi(x)$:
    
    $$P(X < b) = 0.5 + \Phi\left(\frac{b-\mu}{\sigma}\right)$$
    
- Theo bảng tích lũy $\Psi(x)$ hoặc $F(x)$:
    
    $$P(X < b) = \Psi\left(\frac{b-\mu}{\sigma}\right)$$
    

**Trường hợp 3: Tính xác suất một phía - Lớn hơn**

$$P(X > a)$$

- Theo bảng Laplace $\Phi(x)$:
    
    $$P(X > a) = 0.5 - \Phi\left(\frac{a-\mu}{\sigma}\right)$$
    
- Theo bảng tích lũy $\Psi(x)$ hoặc $F(x)$:
    
    $$P(X > a) = 1 - \Psi\left(\frac{a-\mu}{\sigma}\right)$$
    

### Mẹo tra bảng Laplace Φ(x)

- Nếu gặp giá trị âm, sử dụng tính chất đối xứng:
    
    $$\Phi(-x) = -\Phi(x)$$
    
- Nếu gặp giá trị chuẩn hóa lớn hơn 5, có thể lấy gần đúng giá trị bảng là 0.5.