# Bài 1: Thiết kế mạch lọc thông thấp tần số cắt 10 Khz sử dụng OP-AMP. Mô phỏng sử dụng LTSPICE 
Mạch lọc => sử dụng RC OPAmp
$$f_c = \frac{1}{2\pi \cdot R \cdot C}$$
C = 10nF
$$R = \frac{1}{2\pi \cdot f_c \cdot C} = \frac{1}{2\pi \cdot 10000 \cdot (10 \times 10^{-9})} \approx 1591.5\text{ }\Omega$$
<img width="847" height="690" alt="image" src="https://github.com/user-attachments/assets/bd1d70db-6251-4694-8819-0dd2033388cb" />

<img width="955" height="862" alt="image" src="https://github.com/user-attachments/assets/acb0a3db-9a20-437e-bffd-39aa9e5e86be" />
Giải thích biểu đồ:
- Biên độ (đường nét liền):
Từ $10\text{ Hz}$ đến dưới $10\text{ kHz}$ (Dải thông - Passband): Đường nét liền này nằm phẳng lì ở mức $0\text{ dB}$ (tương đương Gain = 1, điện áp ra bằng điện áp vào). Điều này chứng minh mạch cho phép các tần số thấp đi qua nguyên vẹn mà không hề suy hao
Từ vùng $10\text{ kHz}$ trở đi: đường dốc xuống chứng tỏ các tần số cao bị nhiễu và triệt tiêu gần như hoàn toàn

# Bài 2: Thiết kế và mô phỏng một mạch đếm từ 0->99, hiển thị lên 2 LED 7 đoạn. Ngõ vào là 2 nút: PULSE, RESET. Cứ mỗi lần nhấn nút thì số đếm tăng 1, nhấn reset số đếm về 0. Mô phỏng sử dụng phần mềm Proteus. 
