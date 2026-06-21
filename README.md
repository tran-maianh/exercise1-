# Bài 1: Thiết kế mạch lọc thông thấp tần số cắt 10 Khz sử dụng OP-AMP. Mô phỏng sử dụng LTSPICE 
Mạch lọc => sử dụng RC OPAmp

$$f_c = \frac{1}{2\pi \cdot R \cdot C}$$

C = 10nF

$$R = \frac{1}{2\pi \cdot f_c \cdot C} = \frac{1}{2\pi \cdot 10000 \cdot (10 \times 10^{-9})} \approx 1591.5\text{ }\Omega$$


<img width="725" height="649" alt="image" src="https://github.com/user-attachments/assets/21555ecc-46c9-4058-80f8-be1eb8d52764" />

<img width="955" height="862" alt="image" src="https://github.com/user-attachments/assets/acb0a3db-9a20-437e-bffd-39aa9e5e86be" />
Giải thích biểu đồ:

- Biên độ (đường nét liền):
  
Từ $10\text{ Hz}$ đến dưới $10\text{ kHz}$ (Dải thông - Passband): Đường nét liền này nằm phẳng lì ở mức $0\text{ dB}$ (tương đương Gain = 1, điện áp ra bằng điện áp vào). Điều này chứng minh mạch cho phép các tần số thấp đi qua nguyên vẹn mà không hề suy hao

Từ vùng $10\text{ kHz}$ trở đi: đường dốc xuống chứng tỏ các tần số cao bị nhiễu và triệt tiêu gần như hoàn toàn

# Bài 2: Thiết kế và mô phỏng một mạch đếm từ 0->99, hiển thị lên 2 LED 7 đoạn. Ngõ vào là 2 nút: PULSE, RESET. Cứ mỗi lần nhấn nút thì số đếm tăng 1, nhấn reset số đếm về 0. Mô phỏng sử dụng phần mềm Proteus. 

**Input:** 

  Pulse: mỗi lần nhấn tăng 1 -> tạo xung clk
  
  Reset
  
**Process:**: Sử dụng IC 74LS90 (đếm BCD)

  Tầng 1 (hàng đơn vị): Đếm từ 0-9. Khi chạm đến 10, nó tự reset về 0 và gửi 1 xung "Carry" sang tầng 2.

  Tầng 2 (Hàng chục): Đếm khi nhận xung từ tầng 1.

  Nút RESET sẽ nối chung vào chân Clear của cả 2 IC.
  
**Output:**

  2 LED 7 

