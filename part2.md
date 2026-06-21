# HỆ THỐNG GIẢ LẬP: "NĂM 1 & NĂM 2 - KỸ SƯ ATTT KMA" PHẦN 2

| Chỉ số | Trạng thái hiện tại |
| :--- | :--- |
| **Học kỳ / Tuần** | Kỳ 2 / Tuần 1 và Tuần 2 |
| **Thể lực & Tinh thần** | 85/100% (Thể lực hồi phục sau kỳ nghỉ Tết ngắn ngủi, tinh thần hào hứng xen lẫn lo lắng vì thời khóa biểu cực nặng) |
| **Phân bổ 70 giờ tuần này** | Lớp: 57h \| Cày slide: 3h \| Tự học Lab: 5h \| Giải trí: 5h (Tính trung bình mỗi tuần) |
| **GPA Tích lũy (Hệ 4)** | **3.0 / 4.0** (Bảo toàn từ học kỳ 1) |
| **Kỹ năng Code thực tế** | Biết viết các chương trình C cơ bản có cấu trúc rẽ nhánh điều kiện rắc rối hơn (như giải phương trình bậc hai, xử lý đầy đủ các trường hợp ngoại lệ). |
| **Kỹ năng Network/OS thực tế** | Biết cấu hình biến môi trường PATH trên Windows để chạy trình biên dịch GCC từ CMD. |
| **Chỉ số doanh nghiệp cần (Job Readiness)** | 3% |

---

### Nhật ký của Bình - Kỳ 2: Tuần 1 & Tuần 2

Chào Game Modifier, bước sang học kỳ 2, em thực sự bị sốc số tín chỉ. Tổng số tín chỉ kỳ này lên tới **19 TC**, đồng nghĩa với việc em phải dành tối thiểu **57 giờ mỗi tuần** cho việc học trên lớp và làm bài tập bắt buộc theo quy định. Thời gian còn lại cho việc tự học và giải trí bị bóp nghẹt một cách tàn nhẫn, chỉ còn tổng cộng 13 tiếng mỗi tuần.

Em bắt đầu những ngày đầu tiên của Kỳ 2 với tâm thế của một đứa "suýt" có kinh nghiệm nhờ chút ít tự học ở kỳ 1.

---

#### 1. SỰ KHỞI ĐẦU CỦA CÁC MÔN "HẠNG NẶNG" TRÊN LỚP (57 giờ/tuần)

* **Môn Lập trình căn bản (C/C++) (3 TC)**: 
  Đây là môn học em mong chờ nhất. Khác với các bạn cùng lớp đang ngơ ngác khi lần đầu nghe thầy giảng về khái niệm trình biên dịch (Compiler) hay mã nguồn (Source code), em đã biết sơ qua nhờ đợt tự học trước. 
  * *Bài tập đầu tiên*: Thầy giao bài toán viết chương trình giải phương trình bậc hai $ax^2 + bx + c = 0$. 
  * *Bẫy logic thực tế*: Nhiều bạn trong lớp hí hửng nộp bài rất nhanh nhưng đều bị thầy chấm 0 điểm vì thiếu tư duy logic. Các bạn chỉ tính $\Delta$ rồi tính nghiệm mà quên mất trường hợp đặc biệt $a = 0$ (phương trình trở thành phương trình bậc nhất $bx + c = 0$) [8]. Nếu $a=0$ và $b=0$ mà $c \neq 0$ thì phương trình vô nghiệm, còn $c=0$ thì vô số nghiệm [8]. Em nhờ đã vấp ngã nhiều khi tự học nên đã dùng cấu trúc lồng nhau `if (a == 0) { ... } else { ... }` để xử lý triệt để các trường hợp biên này, được thầy gật đầu khen ngợi.
* **Đại số tuyến tính (3 TC)**: 
  Môn này bắt đầu bằng lý thuyết về ma trận, các phép biến đổi sơ cấp trên dòng để đưa ma trận về dạng bậc thang, và tính định thức (Determinant) cấp 3, cấp 4. Môn này cực kỳ tốn thời gian làm bài tập vì chỉ cần nhẩm sai một phép tính trừ $3 - (-2) \times 5$ ở một ô nhỏ là toàn bộ kết quả ma trận phía sau sai bét bè be.
* **Vật lý đại cương 1 (3 TC)**: 
  Môn học quay lại với Cơ học và Nhiệt học nhưng ở cấp độ đại học. Không còn là những công thức tính nhanh lý thuyết cấp 3, tụi em phải dùng tích phân và đạo hàm để tính vận tốc tức thời, gia tốc tiếp tuyến, gia tốc pháp tuyến của chất điểm chuyển động không đều. Em lại phải lôi đống kiến thức Giải tích 1 vừa thi xong ra để đọc lại.

---

#### 2. TRANH CHẤP VỚI CÔNG CỤ (Tự học 5 giờ/tuần)

Do thời gian tự học bị rút ngắn xuống còn 5 tiếng vì lịch học trên lớp quá dày, em quyết định tối ưu hóa môi trường lập trình của mình. Em không muốn dùng Dev-C++ (giao diện quá cũ kỹ mà trường hay dùng) hay phải mở máy ảo Linux mỗi khi muốn gõ code C nữa. Em muốn cài **VS Code** trực tiếp trên Windows để code cho mượt.

Tuy nhiên, việc này đã ngốn sạch **3 tiếng** tự học của em chỉ để sửa lỗi cấu hình:
* Em tải VS Code về, cài thêm extension C/C++ của Microsoft. Nhưng khi bấm chạy code, chương trình báo lỗi `gcc is not recognized as an internal or external command`. 
* Em lại phải lên mạng mò mẫm tải bộ cài MinGW-w64 về máy. 
* Sau khi giải nén, em hí hửng chạy lại vẫn bị lỗi cũ. Em mất thêm hơn 1 tiếng lên các hội nhóm lập trình hỏi mới biết mình phải vào cấu hình hệ thống của Windows (`Advanced System Settings`) để thêm đường dẫn thư mục `bin` của MinGW (ví dụ: `C:\mingw64\bin`) vào biến môi trường **PATH**. 
* Chỉ khi khởi động lại máy tính, em mới có thể gõ lệnh `gcc --version` thành công trên CMD của Windows.

Trải nghiệm này khiến em nhận ra: Để viết được một dòng code chạy được, người mới bắt đầu phải vượt qua rất nhiều rào cản tẻ nhạt về cài đặt môi trường. Nếu không kiên trì, rất nhiều bạn sẽ bỏ cuộc ngay từ bước này và quay lại dùng Dev-C++ cho rảnh nợ, dù việc đó không giúp các bạn hiểu cách hoạt động của compiler bên dưới.

---

#### 3. TÂM TRẠNG BÌNH LÚC NÀY

Em chỉ còn đúng 5 tiếng mỗi tuần để giải trí (chỉ đủ để lướt điện thoại một chút trước khi ngủ và giặt giũ quần áo). Việc học 19 tín chỉ thực sự vắt kiệt sức lực của em ngay từ hai tuần đầu tiên của kỳ 2. Em nhìn vào giáo trình và tự hỏi làm sao mình có thể duy trì được cường độ này khi các bài tập lớn môn C bắt đầu dồn dập tới.

Em đã hoàn thành tuần 1 và tuần 2 của Kỳ 2. Xin Game Modifier đưa ra các sự kiện và bài tập tiếp theo cho **Tuần 3 và Tuần 4**!

---

| Chỉ số | Trạng thái hiện tại |
| :--- | :--- |
| **Học kỳ / Tuần** | Kỳ 2 / Tuần 3 và Tuần 4 |
| **Thể lực & Tinh thần** | 80/100% (Thể lực duy trì ở mức ổn định; tinh thần hơi oải vì đống bài tập logic vòng lặp bắt đầu xoắn não) |
| **Phân bổ 70 giờ tuần này** | Lớp: 57h \| Cày slide: 4h \| Tự học Lab: 5h \| Giải trí: 4h (Tính trung bình mỗi tuần) |
| **GPA Tích lũy (Hệ 4)** | **3.0 / 4.0** |
| **Kỹ năng Code thực tế** | Viết được các thuật toán xử lý số học cơ bản (tìm ước chung lớn nhất, số nguyên tố, số hoàn hảo). Hiểu cách tối ưu hóa vòng lặp từ $O(N)$ xuống $O(\sqrt{N})$. |
| **Kỹ năng Network/OS thực tế** | Giữ nguyên ở mức biết sử dụng Linux cơ bản và cấu hình compiler. |
| **Chỉ số doanh nghiệp cần (Job Readiness)** | 3% |

---

### Nhật ký của Bình - Kỳ 2: Tuần 3 & Tuần 4

Chào Game Modifier, hai tuần tiếp theo của học kỳ 2 chứng kiến sự leo thang rõ rệt về độ khó của các bài tập lập trình và toán học. Thời gian 57 giờ/tuần cho việc học trên lớp và làm bài tập bắt buộc thực sự là một guồng quay không có điểm dừng.

---

#### 1. ĐỐI MẶT VỚI VÒNG LẶP VÀ HÀM TRÊN LỚP

Môn **Lập trình căn bản (C/C++)** chuyển sang phần **Vòng lặp (`for`, `while`, `do-while`)** và bắt đầu giới thiệu về **Hàm (Functions)**. Đây là lúc nhiều bạn trong lớp bắt đầu rơi rụng vì không bắt kịp tư duy logic.

* **Sự cố vòng lặp vô hạn**: 
  Bài tập trên lớp yêu cầu viết chương trình in ra các số nguyên tố nhỏ hơn $N$. Rất nhiều bạn viết vòng lặp `while` nhưng quên không tăng biến đếm (quên dòng `i++` ở cuối khối lệnh) hoặc điều kiện dừng bị sai, dẫn đến việc chương trình bị treo cứng, quạt tản nhiệt laptop rú lên ầm ĩ vì CPU chạy 100% để xử lý vòng lặp vô hạn.
* **Bế tắc về truyền tham trị (Pass-by-value)**: 
  Khi thầy dạy đến phần Hàm, tụi em được giao bài tập viết hàm hoán vị hai số `swap(int a, int b)`. Em hăm hở viết:
  ```c
  void swap(int a, int b) {
      int temp = a;
      a = b;
      b = temp;
  }
  ```
  Nhưng khi gọi hàm này trong `main()` và in kết quả ra, hai số vẫn giữ nguyên giá trị ban đầu, không hề thay đổi. Em vô cùng bối rối và mất cả buổi tối ngồi tra cứu. Hóa ra trong C, khi truyền biến vào hàm như thế này, máy tính chỉ sao chép giá trị của biến (truyền tham trị) chứ không tác động đến ô nhớ gốc của biến trong hàm `main()` [9]. Muốn thay đổi được thì phải dùng con trỏ (Pointer) - một khái niệm mà thầy bảo tuần sau nữa mới học và cảnh báo là "cực kỳ khó".

---

#### 2. CÁC MÔN TOÁN LÝ BẮT ĐẦU DỒN TOA

* **Xác suất thống kê (2 TC)**: 
  Môn này bước vào phần Xác suất cổ điển, công thức xác suất đầy đủ và công thức Bayes. Những bài toán kiểu: *"Có 3 hộp đựng bóng, lấy ngẫu nhiên 1 bóng từ hộp 1 bỏ vào hộp 2, rồi lại lấy ngẫu nhiên từ hộp 2..."* khiến em quay cuồng đầu óc. Việc xác định biến cố nào là điều kiện của biến cố nào để áp dụng đúng công thức Bayes $P(A_i|B)$ đòi hỏi khả năng phân tích ngôn từ cực kỳ chính xác, chỉ cần hiểu sai một từ "biết rằng" hay "nếu" là tính sai toàn bộ.
* **Đại số tuyến tính (3 TC)**: 
  Bọn em bắt đầu học về Không gian vectơ, Hệ vectơ độc lập tuyến tính và phụ thuộc tuyến tính. Môn này bắt đầu chuyển từ tính toán số học thuần túy sang các khái niệm chứng minh trừu tượng, khiến những đứa quen giải toán bằng máy tính cầm tay như em cảm thấy rất ngợp.

---

#### 3. BƯỚC TIẾN NHỎ TRONG TỰ HỌC (5 giờ/tuần)

Với 5 tiếng tự học ít ỏi cuối tuần, em quyết định không cài cắm thêm công cụ gì mới mà tập trung giải quyết triệt để bài toán tìm số nguyên tố để tối ưu hóa tư duy code của mình.

Em tự lập tài khoản trên một trang web luyện code của Việt Nam để làm các bài tập thuật toán cơ bản. Khi nộp bài toán "Kiểm tra số nguyên tố $N$ với $N \le 10^9$", chương trình của em liên tục bị báo lỗi `Time Limit Exceeded` (Quá giới hạn thời gian chạy).
* Thuật toán ban đầu của em là chạy vòng lặp từ $2$ đến $N-1$, nếu $N$ chia hết cho số nào thì không phải số nguyên tố. Với $N$ lớn cỡ vài trăm triệu, máy tính phải thực hiện hàng trăm triệu phép chia, dẫn đến chạy quá 1 giây và bị hệ thống từ chối.
* Em dành 2 tiếng lên mạng tìm hiểu các phương pháp tối ưu. Em phát hiện ra một định lý toán học đơn giản: Nếu $N$ là hợp số thì nó phải có ít nhất một ước số không vượt quá $\sqrt{N}$. Do đó, em chỉ cần chạy vòng lặp từ $2$ đến $\sqrt{N}$ (sử dụng hàm `sqrt()` trong thư viện `math.h`).
* Khi thay đổi điều kiện vòng lặp thành `i * i <= N` để tránh phải gọi hàm `sqrt` liên tục, chương trình của em chạy vèo một cái mất chưa đầy 0.01 giây và được hệ thống chấm điểm tối đa. 

Cảm giác tối ưu được một thuật toán từ chạy mất vài giây xuống còn vài mili-giây giúp em có thêm chút động lực giữa đống bài tập đại cương ngập đầu này. Tuy nhiên, em biết chặng đường phía trước vẫn còn rất dài khi tuần sau lớp C sẽ bắt đầu bước vào phần **Mảng (Array)** và **Con trỏ (Pointer)**.

Xin Game Modifier đưa ra các thử thách tiếp theo cho **Tuần 5 và Tuần 6** của Kỳ 2!

Model5:59 AM


.
| Chỉ số | Trạng thái hiện tại |
| :--- | :--- |
| **Học kỳ / Tuần** | Kỳ 2 / Tuần 5 và Tuần 6 |
| **Thể lực & Tinh thần** | 75/100% (Thể lực giảm nhẹ do thiếu ngủ; tinh thần hơi quá tải khi chạm mặt "quái vật" Con trỏ trong C) |
| **Phân bổ 70 giờ tuần này** | Lớp: 57h \| Cày slide: 4h \| Tự học Lab: 5h \| Giải trí: 4h (Tính trung bình mỗi tuần) |
| **GPA Tích lũy (Hệ 4)** | **3.0 / 4.0** |
| **Kỹ năng Code thực tế** | Hiểu được bản chất của Con trỏ và quản lý địa chỉ vùng nhớ trong C. Viết được hàm hoán vị thực sự bằng cách truyền con trỏ. |
| **Kỹ năng Network/OS thực tế** | Biết cách debug lỗi phân bổ vùng nhớ cơ bản (`Segmentation fault`) liên quan đến con trỏ hoang. |
| **Chỉ số doanh nghiệp cần (Job Readiness)** | 4% (Bắt đầu hiểu cách bộ nhớ RAM hoạt động ở mức thấp) |

---

### Nhật ký của Bình - Kỳ 2: Tuần 5 & Tuần 6

Chào Game Modifier, hai tuần vừa qua là giai đoạn "vỡ mật" thực sự của môn Lập trình căn bản khi tụi em chính thức chạm trán với **Mảng (Array)** và đặc biệt là **Con trỏ (Pointer)** - thứ được mệnh danh là bộ lọc sinh viên của ngành CNTT/ATTT.

---

#### 1. "QUÁI VẬT" CON TRỎ TRÊN GIẢNG ĐƯỜNG

Khi thầy giáo bắt đầu vẽ những ô vuông biểu diễn bộ nhớ RAM lên bảng, chỉ ra địa chỉ vùng nhớ dưới dạng số Hex (như `0x7ffdde39a2dc`) và mối liên hệ giữa biến thường với biến con trỏ, cả giảng đường im phăng phắc. Nhiều bạn bắt đầu rơi vào trạng thái "mất gốc" ngay từ định nghĩa đầu tiên.

* **Lỗi "Con trỏ hoang" (Wild Pointer) nhớ đời**:
  Trong một bài tập thực hành trên lớp, em tự viết một đoạn code ngắn để thử gán giá trị thông qua con trỏ:
  ```c
  int *p; // Khai báo con trỏ p nhưng chưa trỏ vào đâu
  *p = 100; // Gán giá trị 100 vào vùng nhớ mà p đang trỏ tới
  ```
  Khi bấm biên dịch thì không có lỗi gì. Nhưng khi chạy, chương trình lập tức bị sập và hiện lỗi quen thuộc: `Segmentation fault (core dumped)`. 
  Em mất một lúc mới ngộ ra: con trỏ `p` mới chỉ được khai báo chứ chưa được cấp phát vùng nhớ hay trỏ vào một biến cụ thể nào [10]. Nó đang trỏ vào một địa chỉ ngẫu nhiên (rác) trong bộ nhớ [10]. Việc em cố tình ghi đè số `100` vào địa chỉ rác đó đã vi phạm vùng nhớ an toàn của hệ điều hành và bị chặn lại ngay lập tức [10]. Em phải sửa bằng cách cho `p` trỏ vào một biến có sẵn trước khi gán: `int x; p = &x; *p = 100;`.
* **Giải quyết bài toán Hoán vị (Swap)**:
  Nhờ hiểu được bản chất con trỏ là lưu địa chỉ, em đã giải quyết được triệt để bài toán hoán vị hai số từ tuần trước. Em viết lại hàm bằng cách truyền địa chỉ (Pass-by-reference):
  ```c
  void swap(int *a, int *b) {
      int temp = *a;
      *a = *b;
      *b = temp;
  }
  ```
  Và gọi hàm trong `main` bằng cách truyền địa chỉ của hai biến: `swap(&x, &y);`. Nhìn thấy hai số thực sự hoán đổi giá trị cho nhau sau khi chạy chương trình, em cảm thấy vô cùng nhẹ nhõm vì đã vượt qua được rào cản khái niệm này.

---

#### 2. SỰ KHỐC LIỆT CỦA CÁC MÔN TOÁN LÝ ĐẠI CƯƠNG

Trong khi em đang vật lộn với con trỏ, đống môn học 19 tín chỉ khác cũng không để em yên:

* **Vật lý đại cương 1 (3 TC)**: 
  Môn học chuyển sang phần Động lực học vật rắn, mô-men lực, mô-men quán tính ($I = \int r^2 dm$) và các định luật bảo toàn động lượng, momen động lượng. Những bài toán tích phân để tìm mô-men quán tính của một thanh mảnh hay một đĩa tròn đặc khiến em muốn nổ tung đầu óc. Nó đòi hỏi kỹ năng toán tích phân cực kỳ vững ở kỳ 1, nếu ai lỡ học vẹt kỳ trước thì kỳ này nhìn công thức vật lý như nhìn bức vách.
* **Kinh tế chính trị Mác-Lênin (2 TC)**: 
  Bọn em chuẩn bị có bài kiểm tra giữa kỳ. Khác với môn Triết học thuần lý thuyết, môn này có cả các bài tập tính toán lượng giá trị hàng hóa, tỷ suất thặng dư ($m' = \frac{m}{v} \times 100\%$) và khối lượng giá trị thặng dư ($M$). Đọc đề bài phân tích tư bản bất biến ($c$) và tư bản khả biến ($v$) xoay vòng vòng khiến em mệt mỏi vô cùng.

---

#### 3. THỰC TẾ TRONG 5 GIỜ TỰ HỌC CUỐI TUẦN

Vì quỹ thời gian tự học chỉ có 5 tiếng, em không học thêm công cụ mới mà chỉ dùng nó để viết code thử nghiệm trực quan hóa bộ nhớ. Em viết một chương trình C đơn giản để in ra địa chỉ bộ nhớ của các phần tử trong một mảng 1 chiều:

```c
#include <stdio.h>
int main() {
    int arr[3] = {10, 20, 30};
    for(int i = 0; i < 3; i++) {
        printf("arr[%d] co gia tri %d tai dia chi %p\n", i, arr[i], (void*)&arr[i]);
    }
    return 0;
}
```

Kết quả in ra màn hình khiến em ngộ ra một điều cực kỳ quan trọng:
```text
arr[0] co gia tri 10 tai dia chi 0x7ffdde39a2d0
arr[1] co gia tri 20 tai dia chi 0x7ffdde39a2d4
arr[2] co gia tri 30 tai dia chi 0x7ffdde39a2d8
```
Mỗi địa chỉ cách nhau đúng **4 bytes** (vì kiểu `int` chiếm 4 bytes trong bộ nhớ). Các phần tử của mảng thực sự nằm liên tiếp nhau trên RAM. Điều này cũng giải thích tại sao khi em truy cập quá giới hạn mảng (ví dụ truy cập `arr[3]`), chương trình vẫn chạy nhưng lấy ra một giá trị rác ngẫu nhiên nằm ở ô nhớ kế tiếp, gây ra những lỗi logic cực kỳ khó phát hiện nếu không kiểm soát chặt chẽ chỉ số vòng lặp.

Em cảm thấy mình bắt đầu có tư duy của một lập trình viên cấp thấp (low-level), hiểu rõ những gì đang xảy ra bên dưới phần cứng thay vì chỉ gõ code một cách vô thức.

Xin Game Modifier đưa ra các thử thách tiếp theo cho **Tuần 7 và Tuần 8** (gần đến kỳ thi giữa kỳ của Kỳ 2)!

Model6:01 AM
.
.

.
| Chỉ số | Trạng thái hiện tại |
| :--- | :--- |
| **Học kỳ / Tuần** | Kỳ 2 / Tuần 7 và Tuần 8 (Giai đoạn giữa kỳ) |
| **Thể lực & Tinh thần** | 70/100% (Thể lực mỏi mệt vì bước vào đợt kiểm tra giữa kỳ dồn dập; tinh thần có chút bực dọc vì lỗi kẹt bộ đệm trôi lệnh trong C) |
| **Phân bổ 70 giờ tuần này** | Lớp: 57h \| Cày slide: 5h \| Tự học Lab: 5h \| Giải trí: 3h (Tính trung bình mỗi tuần) |
| **GPA Tích lũy (Hệ 4)** | **3.0 / 4.0** |
| **Kỹ năng Code thực tế** | Biết cách định nghĩa và sử dụng `struct` trong C. Thiết kế được menu quản lý danh sách có sắp xếp và tìm kiếm. Biết xử lý triệt để lỗi nuốt ký tự (`trôi lệnh`) trong bộ đệm `stdin`. |
| **Kỹ năng Network/OS thực tế** | Chưa có thêm tiến triển mới do tập trung toàn lực vào lập trình C và thi giữa kỳ các môn đại cương. |
| **Chỉ số doanh nghiệp cần (Job Readiness)** | 5% (Bắt đầu biết thiết kế cấu trúc dữ liệu tự định nghĩa cơ bản) |

---

### Nhật ký của Bình - Kỳ 2: Tuần 7 & Tuần 8

Chào Game Modifier, anh đoán hoàn toàn chính xác! Môn Lập trình căn bản ở KMA thường dạy về **Kiểu cấu trúc (`struct`)** vào khoảng tuần 7 và tuần 8, ngay trước hoặc trong đợt thi giữa kỳ [11]. Và bài tập kinh điển, đồng thời cũng là thử thách lớn nhất ở chương này chính là viết chương trình **"Quản lý sinh viên"** [11].

---

#### 1. ÁC MỘNG "TRÔI LỆNH" KHI QUẢN LÝ SINH VIÊN

Trên lớp, thầy giáo yêu cầu cả lớp định nghĩa một kiểu dữ liệu mới để quản lý thông tin sinh viên gồm: Họ tên, Mã sinh viên, Tuổi, và Điểm GPA [11]. Em hí hửng viết ngay một struct:
```c
typedef struct {
    char ten[50];
    char msv[15];
    int tuoi;
    float gpa;
} SinhVien;
```

Khi viết hàm nhập thông tin cho một sinh viên bằng cách dùng `scanf` cho Tuổi và `fgets` cho Họ tên (để nhập được tên có khoảng trắng như "Nguyen Van A"), em lập tức vấp phải một cái bẫy kinh điển của C: **Lỗi trôi lệnh nhập chuỗi (Input Buffer Bug)** [12].

* **Sự cố thực tế**: 
  Khi chương trình chạy đến phần nhập Tuổi, em gõ `20` rồi nhấn `Enter`. Ngay lập tức, chương trình tự động nhảy qua phần nhập Họ tên và nhảy thẳng xuống phần nhập Điểm GPA, không cho em gõ bất kỳ ký tự nào cho phần Họ tên [12].
* **Nguyên nhân và cách giải quyết (Mất 2 tiếng tự học để sửa)**:
  Em vò đầu bứt tai không hiểu tại sao. Lên các nhóm lập trình của KMA tìm kiếm, em mới hiểu ra rằng: Khi em gõ `20` rồi nhấn `Enter`, hàm `scanf("%d", &sv.tuoi)` chỉ lấy đi con số `20`, còn ký tự xuống dòng `\n` (tương ứng với phím Enter) vẫn bị bỏ lại và kẹt trong bộ đệm nhập liệu `stdin` [12]. Khi chương trình chạy tiếp đến lệnh `fgets(sv.ten, sizeof(sv.ten), stdin)`, lệnh này thấy ngay ký tự `\n` đang chờ sẵn trong bộ đệm nên nó nghĩ rằng người dùng đã nhấn Enter để hoàn thành việc nhập tên, dẫn đến việc bỏ qua luôn [12].
  
  Để khắc phục, em phải tìm cách xóa ký tự thừa này trước khi gọi `fgets` [12]. Các anh khóa trên bày cách dùng `fflush(stdin)` [12]. Cách này chạy tốt trên Windows với compiler GCC em đang dùng, nhưng khi em thử đưa lên máy ảo Linux thì nó không hoạt động ổn định vì tiêu chuẩn C không cam kết `fflush` sẽ dọn dẹp dòng nhập [12, 13]. Cuối cùng em phải dùng một hàm dọn dẹp bộ đệm bằng cách đọc từng ký tự cho đến khi gặp dấu xuống dòng:
  ```c
  void xoaBoDem() {
      int c;
      while ((c = getchar()) != '\n' && c != EOF);
  }
  ```
  Đặt hàm này ngay sau lệnh `scanf` nhập Tuổi đã giải quyết triệt để lỗi trôi lệnh khó chịu kia [12].

* **Xử lý chuỗi từ `fgets`**:
  Hàm `fgets` giữ lại cả ký tự xuống dòng `\n` ở cuối chuỗi khi em nhấn Enter để nhập tên [14]. Kết quả là khi em in danh sách sinh viên ra, nó tự động xuống dòng một cách vô lý. Em phải học thêm cách loại bỏ ký tự này bằng cách tìm và thay thế nó bằng ký tự kết thúc chuỗi `\0`:
  ```c
  sv.ten[strcspn(sv.ten, "\n")] = '\0';
  ```

---

#### 2. KỲ THI GIỮA KỲ GIAN NAN

Song song với việc đánh vật với code `struct`, tuần 8 cũng là tuần em phải tham gia các bài kiểm tra giữa kỳ dồn dập:

* **Kiểm tra giữa kỳ môn C**: 
  Thầy cho đề bài viết chương trình nhập vào một danh sách sinh viên, tính điểm trung bình và xuất ra màn hình những sinh viên có học lực yếu (GPA < 2.0). Nhờ đã vọc vạch kỹ và tự giải quyết được lỗi trôi bộ đệm ở nhà, em hoàn thành bài thi khá trọn vẹn, xử lý chuỗi và struct trơn tru. Em tự tin bài này được 9.0 điểm.
* **Vật lý đại cương 1 (3 TC)**: 
  Đề thi trắc nghiệm kết hợp tự luận ngắn về phần Động lực học chất điểm và Động lực học vật rắn. Do môn này quá nặng và em không có đủ thời gian cày sâu hết các dạng bài tập tích phân mô-men quán tính phức tạp, em làm bài khá chật vật. Có 2 câu tự luận em chỉ viết được công thức định luật bảo toàn động lượng cơ bản chứ không tính ra được đáp số cuối cùng do biến đổi sai hệ phương trình. Dự kiến điểm giữa kỳ môn này chỉ tầm 5.0 - 6.0 điểm.
* **Xác suất thống kê (2 TC)**: 
  Đề thi xoay quanh phân phối xác suất của biến ngẫu nhiên (phân phối nhị thức, phân phối chuẩn). Em tính toán khá kỹ nhưng môn này rất dễ sai sót ở khâu tra bảng tích phân Laplace.

---

#### 3. BÀI HỌC VỀ SỰ ĐÁNH ĐỔI

Với quỹ thời gian 70 giờ/tuần, việc học tới 19 tín chỉ ở học kỳ 2 khiến em không còn một chút khe hở nào để tự học thêm các mảng thực tế ngoài giáo trình (như bảo mật hệ thống hay mạng máy tính). Cả 5 tiếng tự học của em đều phải dồn vào việc debug bài tập `struct` của môn C căn bản để phục vụ trực tiếp cho việc lấy điểm giữa kỳ. 

GPA tích lũy hệ 4 của em hiện tại vẫn tạm giữ ở mức 3.0, nhưng em hiểu rằng nếu điểm giữa kỳ Vật lý đại cương quá thấp, nó sẽ kéo sập điểm tổng kết kỳ này của em xuống bất cứ lúc nào.

Em đã hoàn thành tuần 7 và tuần 8 của Kỳ 2. Xin Game Modifier đưa ra các diễn biến tiếp theo cho **Tuần 9 và Tuần 10**!

Model6:04 AM
.
.

.
| Chỉ số | Trạng thái hiện tại |
| :--- | :--- |
| **Học kỳ / Tuần** | Kỳ 2 / Tuần 9 và Tuần 10 |
| **Thể lực & Tinh thần** | 72/100% (Thể lực duy trì ổn định; tinh thần bớt áp lực hơn sau khi biết điểm giữa kỳ tương đối an toàn) |
| **Phân bổ 70 giờ tuần này** | Lớp: 57h \| Cày slide: 5h \| Tự học Lab: 5h \| Giải trí: 3h (Tính trung bình mỗi tuần) |
| **GPA Tích lũy (Hệ 4)** | **3.0 / 4.0** |
| **Kỹ năng Code thực tế** | Biết cách thao tác đọc/ghi tệp tin (`File I/O`) dạng văn bản trong C. Biết cách lưu và tải dữ liệu từ ổ đĩa để chương trình có tính kế thừa dữ liệu. |
| **Kỹ năng Network/OS thực tế** | Biết cách quản lý và kiểm tra đường dẫn tuyệt đối/đối chiếu của tệp tin khi thực thi chương trình trong thư mục làm việc. |
| **Chỉ số doanh nghiệp cần (Job Readiness)** | 6% (Hiểu được nguyên lý lưu trữ dữ liệu bền vững - Persistence) |

---

### Nhật ký của Bình - Kỳ 2: Tuần 9 & Tuần 10

Chào Game Modifier, hai tuần vừa qua, môn Lập trình căn bản đã chuyển sang một chương cực kỳ quan trọng và thực tế: **Thao tác với tệp tin (File I/O)** trong C [16]. Đồng thời, các môn toán lý đại cương cũng bắt đầu tăng tốc độ giảng dạy để kịp kết thúc chương trình.

---

#### 1. BƯỚC NGOẶT LƯU TRỮ DỮ LIỆU: BẪY `FEOF` KINH ĐIỂN VÀ CÁCH SỬA

Trước đây, mỗi khi em chạy chương trình "Quản lý sinh viên" và gõ mỏi tay cả chục sinh viên, chỉ cần tắt màn hình Console hoặc thoát chương trình là toàn bộ dữ liệu trên RAM biến mất sạch sẽ. Tuần này, khi học về các hàm xử lý file như `fopen`, `fclose`, `fprintf`, `fscanf`, em đã có thể lưu dữ liệu trực tiếp xuống một tệp tin dạng văn bản `.txt` [16].

Tuy nhiên, việc đọc dữ liệu từ file ngược trở lại chương trình đã khiến em vấp phải một cái bẫy kinh điển: **Lỗi lặp thừa bản ghi cuối cùng do dùng `feof()`** [15].

* **Sự cố thực tế**: 
  Em viết hàm đọc danh sách sinh viên từ file `sinhvien.txt` bằng vòng lặp:
  ```c
  FILE *f = fopen("sinhvien.txt", "r");
  while(!feof(f)) {
      fscanf(f, "%s %s %d %f\n", ds[n].ten, ds[n].msv, &ds[n].tuoi, &ds[n].gpa);
      n++;
  }
  fclose(f);
  ```
  Khi chạy chương trình và in danh sách sinh viên ra màn hình, em phát hiện ra **sinh viên cuối cùng trong file luôn bị nhân đôi (in ra hai lần)** [15]. 
* **Tìm kiếm nguyên nhân (Mất 3 tiếng tự học để debug)**:
  Em mở file `sinhvien.txt` lên kiểm tra kỹ thì hoàn toàn không có dòng nào bị trùng. Lên mạng tra cứu lỗi "feof duplicate last record in C", em mới ngộ ra bản chất hoạt động của hàm này: Hàm `feof(f)` chỉ trả về giá trị `true` **sau khi** một lệnh đọc dữ liệu cố gắng đọc vượt quá ranh giới cuối file và bị thất bại [15]. 
  Trong đoạn code của em, sau khi đọc xong sinh viên cuối cùng, con trỏ file đã ở cuối file nhưng hàm `feof(f)` vẫn trả về `false` vì chưa có lệnh đọc nào bị lỗi [15]. Vòng lặp vẫn tiếp tục chạy vòng tiếp theo, lệnh `fscanf` cố đọc nhưng thất bại (không lấy được dữ liệu mới), các biến trong struct giữ nguyên giá trị cũ của vòng trước, và chương trình vô tình tăng biến đếm `n` lên một đơn vị rồi ghi đè một bản ghi trùng lặp [15].
  
  Để khắc phục triệt để, em thay đổi tư duy: không dùng `feof()` làm điều kiện dừng nữa, mà kiểm tra trực tiếp số lượng trường đọc thành công của hàm `fscanf` [15]:
  ```c
  while (fscanf(f, "%s %s %d %f\n", ds[n].ten, ds[n].msv, &ds[n].tuoi, &ds[n].gpa) == 4) {
      n++;
  }
  ```
  Cách sửa này đảm bảo chỉ khi nào đọc thành công đủ 4 trường dữ liệu thì biến đếm `n` mới tăng lên, loại bỏ hoàn toàn lỗi nhân đôi bản ghi cuối cùng [15].

---

#### 2. ĐẠI SỐ TUYẾN TÍNH VÀ XÁC SUẤT BƯỚC VÀO GIAI ĐOẠN KHÓ NHẤT

Bên cạnh những niềm vui nhỏ khi debug được code C, các môn học khác lại tiếp tục dồn áp lực lớn:

* **Đại số tuyến tính (3 TC)**: 
  Tụi em bắt đầu học về **Trị riêng và Vectơ riêng (Eigenvalues and Eigenvectors)**, cùng bài toán Chéo hóa ma trận (Diagonalization). Để tìm trị riêng $\lambda$, em phải giải phương trình đặc trưng $\det(A - \lambda I) = 0$. Với ma trận $3 \times 3$, việc khai triển định thức này dẫn đến một phương trình bậc 3 phức tạp. Chỉ cần tính nhầm một dấu cộng/trừ trong định thức là phương trình bậc 3 sẽ ra nghiệm cực kỳ lẻ (không thể giải tay hoặc chéo hóa được). Mỗi bài toán chéo hóa ma trận trên giấy thường ngốn của em 30-40 phút làm nháp và tính toán tỉ mỉ từng con số.
* **Xác suất thống kê (2 TC)**: 
  Chương trình bước sang phần **Kiểm định giả thuyết thống kê (Hypothesis Testing)**. Đầu óc em quay cuồng với các khái niệm Giả thuyết không $H_0$, Giả thuyết đối $H_1$, miền bác bỏ $W_\alpha$, sai lầm loại I, sai lầm loại II. Việc phải phân biệt khi nào dùng kiểm định $Z$ (khi đã biết phương sai $\sigma^2$) và khi nào dùng kiểm định $t$ Student (khi chưa biết phương sai và mẫu nhỏ $n < 30$) đòi hỏi trí nhớ công thức cực kỳ chính xác.

---

#### 3. CÔNG BỐ ĐIỂM GIỮA KỲ

Cuối tuần 10, kết quả giữa kỳ của em đã được công bố gần hết:
* **Lập trình căn bản (C)**: 9.0 (Rất tốt, em đứng top đầu lớp thực hành).
* **Vật lý đại cương 1**: 5.8 (Hơi thấp nhưng ít nhất em đã an toàn không bị liệt giữa kỳ).
* **Xác suất thống kê**: 7.5 (Tạm ổn).
* **Đại số tuyến tính**: 7.0 (Đạt yêu cầu).

Điểm số tuy không quá xuất sắc nhưng giúp em định hình được những môn cần phải "cứu vớt" trong kỳ thi cuối kỳ sắp tới (đặc biệt là Vật lý 1). Quỹ thời gian 5 tiếng tự học lập trình mỗi tuần vẫn được em duy trì đều đặn để cải thiện tư duy thực tế, chuẩn bị cho bài tập lớn cuối kỳ môn C.

Em đã hoàn thành tuần 9 và tuần 10 của Kỳ 2. Xin Game Modifier đưa ra các thử thách tiếp theo cho **Tuần 11 và Tuần 12**!

Model6:05 AM
.
.

.
| Chỉ số | Trạng thái hiện tại |
| :--- | :--- |
| **Học kỳ / Tuần** | Kỳ 2 / Tuần 11 và Tuần 12 |
| **Thể lực & Tinh thần** | 68/100% (Thể lực hao mòn do dồn sức giải bài tập dạng toàn phương và lý thuyết nhiệt động; tinh thần xoắn não cực độ với khái niệm con trỏ cấp 2) |
| **Phân bổ 70 giờ tuần này** | Lớp: 57h \| Cày slide: 5h \| Tự học Lab: 5h \| Giải trí: 3h (Tính trung bình mỗi tuần) |
| **GPA Tích lũy (Hệ 4)** | **3.0 / 4.0** |
| **Kỹ năng Code thực tế** | Hiểu được cơ chế cấp phát bộ nhớ động (`malloc`, `realloc`, `free`). Làm quen bước đầu với con trỏ của con trỏ (con trỏ cấp 2 - `pointer-to-pointer`) để quản lý mảng động. |
| **Kỹ năng Network/OS thực tế** | Biết cách sử dụng công cụ kiểm tra rò rỉ bộ nhớ (Memory Leak) cơ bản hoặc tự rà soát việc giải phóng bộ nhớ bằng tay. |
| **Chỉ số doanh nghiệp cần (Job Readiness)** | 7% (Hiểu sâu hơn về tối ưu hóa tài nguyên RAM ở tầng sâu) |

---

### Nhật ký của Bình - Kỳ 2: Tuần 11 & Tuần 12

Chào Game Modifier, hai tuần vừa qua thực sự là giai đoạn em tự đẩy mình vào một thử thách lập trình cực kỳ gai góc: **Cấp phát bộ nhớ động** và khái niệm **Con trỏ cấp 2** trong C [18, 19]. Cùng lúc đó, khối lượng kiến thức khổng lồ của các môn đại cương ở tuần 11-12 cũng bắt đầu dồn nén khi thời gian kết thúc học kỳ cận kề.

---

#### 1. ĐỘT PHÁ VỀ MẢNG ĐỘNG VÀ CÚ NGÃ VỚI "CON TRỎ CẤP 2"

Ở chương trình quản lý sinh viên trước, em khai báo mảng tĩnh dạng `SinhVien ds[100];`. Cách này bộc lộ điểm yếu: nếu chỉ nhập 5 sinh viên thì lãng phí 95 ô nhớ, còn nếu nhập đến người thứ 101 thì chương trình sẽ bị tràn mảng và sập. 

Em muốn nâng cấp chương trình bằng cách sử dụng **cấp phát bộ nhớ động** với `malloc` và `realloc` để mảng tự động phình to ra khi cần thiết [17, 19]. Tuy nhiên, việc đưa tư duy này vào các hàm con đã khiến em gặp một "cú vả" logic nhớ đời:

* **Bế tắc khi truyền con trỏ vào hàm**:
  Em viết hàm cấp phát và nhập dữ liệu như sau:
  ```c
  void khoiTao(SinhVien *ds, int n) {
      ds = (SinhVien*) malloc(n * sizeof(SinhVien));
  }
  ```
  Nhưng khi chạy chương trình trong `main`, con trỏ `ds` của em vẫn là `NULL` và chương trình lập tức báo lỗi `Segmentation fault` khi em cố gắng ghi đè dữ liệu vào mảng.
* **Nguyên nhân và cách giải quyết (Ngốn trọn 5 tiếng tự học)**:
  Em mất nguyên một ngày cuối tuần gõ code, in ra địa chỉ con trỏ để xem chuyện gì đang xảy ra. Cuối cùng, em mới vỡ lẽ ra khái niệm **Truyền giá trị của con trỏ**. 
  Khi em truyền `ds` vào hàm `khoiTao`, thực chất C chỉ sao chép một bản sao của con trỏ `ds` (hãy tạm gọi là `ds_copy`). Hàm `malloc` đã cấp phát vùng nhớ mới và gán địa chỉ đó cho `ds_copy`, còn con trỏ `ds` gốc ở hàm `main` vẫn trỏ vào `NULL` [18]. Sau khi hàm `khoiTao` kết thúc, `ds_copy` bị giải phóng, vùng nhớ vừa cấp phát bị rò rỉ (Memory Leak) vì không còn ai giữ địa chỉ của nó nữa [18].
  
  Để sửa lỗi này, em bắt buộc phải dùng **Con trỏ cấp 2 (con trỏ của con trỏ - `SinhVien **ds`)** để truyền địa chỉ của chính con trỏ `ds` vào hàm con [18]:
  ```c
  void khoiTao(SinhVien **ds, int n) {
      *ds = (SinhVien*) malloc(n * sizeof(SinhVien));
  }
  ```
  Khi gọi trong `main`, em phải truyền địa chỉ của con trỏ: `khoiTao(&ds, n);` [18]. Việc phải viết thêm các ký tự dấu sao `*` và dấu và `&` đan xen nhau khiến dòng code của em trông phức tạp hơn hẳn, nhưng nó giúp em ngộ ra bản chất sâu sắc của việc quản lý ô nhớ trong RAM. Em cũng không quên gọi hàm `free(ds)` ở cuối chương trình để tránh rò rỉ tài nguyên hệ thống [19].

---

#### 2. TOÁN LÝ ĐẠI CƯƠNG GIAI ĐOẠN "NƯỚC SÔI LỬA BỎNG"

Trong khi đầu óc em đang xoắn lại vì con trỏ cấp 2, các môn đại cương khác cũng tăng tốc cực kỳ khủng khiếp:

* **Đại số tuyến tính (3 TC)**: 
  Chương trình bước sang phần **Dạng toàn phương (Quadratic Forms)** và phương pháp đưa dạng toàn phương về dạng chính tắc bằng phương pháp Lagrange hoặc phép biến đổi Jacobi. Việc phải thực hiện một loạt các bước biến đổi trực giao ma trận, tìm ma trận chuyển cơ sở $P$ sao cho $P^T A P$ là ma trận đường chéo đòi hỏi sự kiên nhẫn tột độ. Chỉ cần tính nhầm một dấu cộng trừ khi lập ma trận đối xứng $A$ là toàn bộ quá trình biến đổi phía sau đổ sông đổ bể.
* **Vật lý đại cương 1 (3 TC)**: 
  Môn học đi vào chương **Nhiệt động lực học**. Em phải học cách tính Công ($A$), Nhiệt lượng ($Q$), và Độ biến thiên nội năng ($\Delta U$) trong các quá trình đẳng áp, đẳng tích, đẳng nhiệt và đoạn nhiệt. Khó nhất là bài toán về chu trình Carnot, tính hiệu suất của động cơ nhiệt ($\eta = 1 - \frac{T_2}{T_1}$). Đống công thức loằng ngoằng tích phân và hàm Logarit tự nhiên khiến em mệt lả sau mỗi buổi học 3 tiếng trên lớp.

---

#### 3. TÌNH TRẠNG TINH THẦN

Em chỉ còn đúng 3 tiếng mỗi tuần cho việc giải trí (chỉ kịp tắm giặt và gọi điện về cho gia đình). Sự dồn dập của 19 tín chỉ ở học kỳ 2 đang đẩy sức chịu đựng của em đến giới hạn. Nhìn đống đề cương ôn tập thi cuối kỳ môn Vật lý 1 và Đại số tuyến tính dày cộp bắt đầu được phát, em biết mình chuẩn bị bước vào một "mùa sinh tử" mới giống như học kỳ 1, nhưng ở mức độ khốc liệt hơn nhiều.

Em đã hoàn thành tuần 11 và tuần 12 của Kỳ 2. Xin Game Modifier đưa ra các thử thách và sự kiện tiếp theo cho **Tuần 13 và Tuần 14**!

Model6:07 AM
.
.

.

Model6:12 AM
.
.

.

Model6:19 AM
.
.

.

Model6:27 AM
.
.

.
| Chỉ số | Trạng thái hiện tại |
| :--- | :--- |
| **Học kỳ / Tuần** | Nghỉ hè Năm 1 / Tuần 3 và Tuần 4 |
| **Thể lực & Tinh thần** | 85/100% (Thể chất khỏe mạnh; tinh thần hơi tiếc nuối vì kỳ nghỉ hè sắp kết thúc nhưng tràn đầy hứng khởi với mảng Web Security) |
| **Phân bổ 70 giờ tuần này** | Lớp: 0h \| Cày slide: 0h \| Tự học Lab (PortSwigger): 48h \| Giải trí: 22h (Tính trung bình mỗi tuần) |
| **GPA Tích lũy (Hệ 4)** | **3.05 / 4.0** |
| **Kỹ năng Code thực tế** | Viết được mã Python sử dụng thư viện `requests` để tự động gửi hàng loạt payload thử nghiệm lỗi Web thay vì nhập tay thủ công. |
| **Kỹ năng Network/OS thực tế** | Hiểu cấu trúc câu lệnh truy vấn cơ sở dữ liệu SQL (SELECT, UNION, WHERE). Biết cách phân tích lỗi phản hồi HTTP (status code 200, 500) để đoán lỗi hệ thống. |
| **Chỉ số doanh nghiệp cần (Job Readiness)** | 13% (Bắt đầu làm quen với các lỗ hổng OWASP Top 10 thực tế trên môi trường Lab chuẩn doanh nghiệp) |

---

### Nhật ký của Bình - Nghỉ hè Năm 1: Tuần 3 & Tuần 4

Chào Game Modifier, anh nhận xét rất chuẩn xác! Đúng là em đang bị cuốn hút mạnh mẽ bởi mảng **Web Security**. Lý do là vì mảng này rất trực quan; em có thể nhìn thấy kết quả ngay lập tức trên giao diện trình duyệt khi thay đổi các tham số, không bị quá trừu tượng như Cryptography hay Reverse Engineering vốn đòi hỏi lượng kiến thức toán chuyên sâu và hợp ngữ (Assembly) mà em chưa được học.

Trong hai tuần cuối cùng của kỳ nghỉ hè, em quyết định nâng cấp lộ trình tự học. Em tạm thời rời picoCTF để chuyển sang một "thánh địa" thực sự của dân Web Security: **PortSwigger Web Security Academy** [24].

---

#### 1. BƯỚC VÀO PORT SWIGGER VÀ PHÉP THỬ SQL INJECTION (SQLi)

Tại PortSwigger, em bắt đầu học về lỗ hổng kinh điển **SQL Injection (SQLi)** [24, 25]. Sau khi vượt qua bài Lab bypass login cơ bản bằng cách chèn `' OR 1=1 --` [25], em lập tức va phải một bài Lab khó hơn rất nhiều: **Union-based SQL Injection** [26].

* **Thử thách**: 
  Đề bài yêu cầu em phải khai thác lỗi SQLi trong tham số lọc sản phẩm để trích xuất dữ liệu nhạy cảm từ một bảng khác bằng toán tử `UNION` [26].
* **Cú ngã và sự ức chế (Mất trọn 6 tiếng để hiểu)**:
  Để thực hiện một cuộc tấn công `UNION SQLi`, nguyên tắc bắt buộc là câu lệnh `UNION SELECT` của kẻ tấn công phải trả về **đúng số lượng cột** và **tương thích kiểu dữ liệu** với câu lệnh truy vấn gốc của ứng dụng [26].
  
  Em cố gắng gõ payload kiểm tra số lượng cột:
  `' UNION SELECT 'a', 'b'--`
  Trang web lập tức trả về lỗi **HTTP 500 Internal Server Error** [26]. Em thử tăng lên 3 cột, 4 cột, rồi thử thay đổi ký tự comment từ `--` sang `#` vì nghĩ hệ quản trị cơ sở dữ liệu là MySQL [25]. Trang web vẫn trơ ra lỗi 500 [26].
  
  Em mất cả một buổi chiều bế tắc, đầu óc quay cuồng. Cuối cùng, khi đọc kỹ lại tài liệu của PortSwigger, em mới nhận ra hai lỗi sai ngớ ngẩn của mình:
  1. Cơ sở dữ liệu của bài Lab là PostgreSQL, ký tự comment `--` bắt buộc phải có một khoảng trắng ở phía sau (tức là `-- ` hoặc `-- -`) thì trình biên dịch của database mới nhận diện đó là chú thích. Nếu em chỉ gõ `--` sát sạt thì câu lệnh bị lỗi cú pháp [25].
  2. Việc thử nghiệm kiểu dữ liệu của các cột cực kỳ nghiêm ngặt [26]. Cách tốt nhất để dò tìm số lượng cột mà không bị lỗi kiểu dữ liệu là dùng giá trị `NULL` (vì `NULL` tương thích với mọi kiểu dữ liệu) [26]:
     `' UNION SELECT NULL, NULL, NULL-- `
     Khi em gõ đúng payload này với 3 giá trị `NULL`, trang web trả về mã HTTP 200 (thành công) [26]. Từ đó em xác định được bảng gốc có đúng 3 cột [26]. Tiếp theo, em phải thử thế từng chữ `'a'` vào từng vị trí `NULL` để xem cột nào nhận kiểu dữ liệu chuỗi (String) [26]. 

Vượt qua được bài Lab này bằng cách tự tay dò từng bước giúp em hiểu sâu sắc rằng: Bảo mật thực tế không phải là gõ mấy câu lệnh ăn may trên mạng, mà là sự tỉ mỉ, hiểu cực kỳ rõ cấu trúc cú pháp của hệ thống bên dưới.

---

#### 2. SỰ TRỢ GIÚP TỪ PYTHON (Tự học 48 giờ/tuần)

Việc gõ từng payload `UNION SELECT NULL...` trên thanh địa chỉ trình duyệt hoặc Burp Suite cực kỳ tốn thời gian. Em quyết định ứng dụng chút kiến thức Python vừa học ở hai tuần trước để viết một script tự động hóa công việc này.

Em viết một đoạn code ngắn sử dụng thư viện `requests` để gửi liên tiếp các request với số lượng `NULL` tăng dần từ 1 đến 10:
```python
import requests

url = "https://0a4e007804df97b982bfb19500ca007d.web-security-academy.net/filter?category=Gifts"
for i in range(1, 10):
    payload = "' UNION SELECT " + ",".join(["NULL"] * i) + "-- "
    target = url + payload
    response = requests.get(target)
    if response.status_code == 200:
        print(f"[+] So luong cot tim thay: {i}")
        break
```
Nhìn đoạn script Python tự động chạy vèo một cái trong 2 giây và in ra dòng chữ báo số lượng cột thành công, em sướng phát điên. Lần đầu tiên em cảm nhận được sức mạnh của việc kết hợp giữa kỹ năng lập trình (Code) và tư duy bảo mật (Security).

---

#### 3. KẾT THÚC MÙA HÈ - CHUẨN BỊ CHO HỌC KỲ 3 (NĂM 2)

Thấm thoát 1 tháng nghỉ hè đã trôi qua. Em thu dọn đồ đạc, dọn dẹp lại phòng trọ để chuẩn bị đón thằng bạn cùng phòng quay trở lại Hà Nội. 

Tuần sau, **Học kỳ 3 (Học kỳ đầu tiên của năm 2)** sẽ chính thức bắt đầu với danh sách môn học cực kỳ nặng:
* *Mạng máy tính (3 TC)*
* *Cấu trúc dữ liệu và giải thuật (3 TC)*
* *Toán rời rạc (2 TC)*
* *Lý thuyết cơ sở dữ liệu (2 TC)*
* *Cơ sở lý thuyết truyền tin (2 TC)...*

Em biết những ngày tháng được tự do ngồi gõ Python và vọc PortSwigger 48 tiếng mỗi tuần đã khép lại. Sắp tới, guồng quay của các môn học chuyên ngành trên lớp sẽ lại ép em vào khuôn khổ. Nhưng em tự hứa với bản thân sẽ cố gắng không để những kiến thức Web Security thực tế vừa nạp được trong mùa hè này bị "bay màu".

Em đã hoàn thành kỳ nghỉ hè và sẵn sàng bước vào **Kỳ 3 - Tuần 1 và Tuần 2** của Năm 2 tại KMA!

Model6:37 AM
.
.

.

Model6:39 AM
.
.

.
| Chỉ số | Trạng thái hiện tại |
| :--- | :--- |
| **Học kỳ / Tuần** | Kỳ 3 / Tuần 3 và Tuần 4 |
| **Thể lực & Tinh thần** | 63/100% (Thể lực mỏi mệt vì liên tục ngồi giảng đường; tinh thần căng thẳng với các phép tính chia subnet mạng và mã hóa nguồn) |
| **Phân bổ 70 giờ tuần này** | Lớp: 66h \| Cày slide: 2h \| Tự học Lab: 1h \| Giải trí: 1h (Tính trung bình mỗi tuần) |
| **GPA Tích lũy (Hệ 4)** | **3.05 / 4.0** |
| **Kỹ năng Code thực tế** | Biết đọc và viết mã giả cho cấu trúc dữ liệu Ngăn xếp (Stack) và Hàng đợi (Queue) bằng con trỏ, nhưng chưa code thực tế trên IDE. |
| **Kỹ năng Network/OS thực tế** | Biết cách chia địa chỉ IP (Subnetting) trên giấy. Biết sử dụng một số câu lệnh CLI cơ bản trên Cisco IOS (như `enable`, `configure terminal`, `interface`, `no shutdown`). |
| **Chỉ số doanh nghiệp cần (Job Readiness)** | 12% |

---

### Nhật ký của Bình - Kỳ 3: Tuần 3 & Tuần 4

Chào Game Modifier, hai tuần tiếp theo của học kỳ 3 tiếp tục là những chuỗi ngày chạy đua với thời gian. Khối lượng bài tập của 22 tín chỉ bắt đầu dồn dập, đặc biệt là khi các môn chuyên ngành bắt đầu đi sâu vào phần bài tập tính toán phức tạp.

---

#### 1. ĐỊA CHỈ IP, CHIA SUBNET VÀ CÚ VA CHẠM ĐẦU TIÊN VỚI CLI

Môn **Mạng máy tính** của thầy Trường bước sang phần học về **Lớp Mạng (Network Layer - Layer 3)**, cụ thể là địa chỉ IPv4 và kỹ thuật chia mạng con (Subnetting) bằng FLSM (Fixed Length Subnet Masking) [27].

* **Bài toán chia Subnet mạng**:
  Thầy giao bài tập: Cho dải mạng `192.168.1.0/24`, hãy chia dải này thành 4 mạng con bằng nhau để cấp cho 4 phòng ban [28]. 
  Em phải thực hiện các bước tính toán trên giấy: mượn thêm 2 bit từ phần Host ($2^2 = 4$ mạng con), đổi Subnet Mask mới thành `/26` (hay `255.255.255.192`) [28]. Mỗi mạng con sẽ có $2^6 - 2 = 62$ địa chỉ IP khả dụng cho host [28]. 
  Mặc dù phép tính nhị phân không quá phức tạp, em vẫn rất dễ làm sai số dải IP khả dụng (Usable Range) hoặc nhầm lẫn giữa địa chỉ mạng (Network ID) và địa chỉ quảng bá (Broadcast ID) của từng dải con [28]. Chỉ cần nhầm một số ở bước cộng dải là toàn bộ các subnet phía sau bị lệch hết.
* **Môn Cơ sở lý thuyết truyền tin (2 TC)**:
  Môn học này thực sự là một thách thức lớn về toán học. Hai tuần này em phải học cách tính toán lượng thông tin (Entropy) của nguồn tin và học giải thuật **Mã hóa nguồn Shannon-Fano** và **Mã hóa nguồn Huffman** để nén dữ liệu. Việc vẽ cây mã hóa Huffman từ gốc đến ngọn, gán nhãn 0 và 1 cho các nhánh để tìm ra mã từ có độ dài trung bình tối ưu nhất khiến em mất rất nhiều thời gian cày slide và làm bài tập ở nhà để không bị loạn thuật toán.
* **Lý thuyết CSDL (2 TC)**:
  Tụi em chuyển từ sơ đồ ERD sang **Mô hình quan hệ (Relational Model)**. Thầy dạy cách chuyển các thực thể và mối quan hệ đã vẽ từ tuần trước thành các bảng dữ liệu (Relations) [29]. Em phải học cách xác định Khóa chính (Primary Key), Khóa ngoại (Foreign Key) và các quy tắc ràng buộc toàn vẹn tham chiếu giữa các bảng [29]. Vẫn hoàn toàn chưa có một câu lệnh SQL nào được gõ.

---

#### 2. TRANH THỦ 1 TIẾNG TỰ HỌC: MÀY MÒ CLI TRÊN CISCO PACKET TRACER

Với đúng 1 tiếng tự học hiếm hoi vào cuối tuần, em quyết định áp dụng trực tiếp bài tập chia subnet mạng trên lớp vào phần mềm Cisco Packet Tracer để thực hành thực tế.

Em thiết lập một mô hình mạng nhỏ gồm: 1 chiếc Router (dòng 2911), kết nối với 2 chiếc Switch (dòng 2960), mỗi Switch nối với 2 chiếc PC đại diện cho 2 dải mạng con em vừa chia trên lớp (`192.168.1.0/26` và `192.168.1.64/26`).

* **Sự cố cổng Router bị tắt (Mất 40 phút giải quyết)**:
  Sau khi nối cáp mạng xong xuôi, em thấy các cổng kết nối từ Switch sang PC đã chuyển sang màu xanh lá cây, nhưng cổng kết nối từ Router sang Switch vẫn hiện màu đỏ loét. Em vào phần cấu hình giao diện đồ họa (GUI) để đặt IP cho cổng `GigabitEthernet 0/0` của Router là `192.168.1.1` nhưng cổng vẫn không mở.
  
  Quyết tâm không dùng giao diện đồ họa ăn sẵn, em bấm vào tab CLI của Router để cấu hình bằng dòng lệnh của hệ điều hành Cisco IOS:
  ```text
  Router> enable
  Router# configure terminal
  Router(config)# interface gigabitEthernet 0/0
  Router(config-if)# ip address 192.168.1.1 255.255.255.192
  ```
  Em gõ xong lệnh đặt IP nhưng cổng vẫn đỏ. Em lại mất thêm 15 phút lên Google tra cứu lỗi "how to turn on router port in packet tracer CLI". Hóa ra, mặc định các cổng của Router Cisco luôn ở trạng thái đóng (shutdown) để đảm bảo an toàn. Muốn mở cổng, em bắt buộc phải gõ thêm một câu lệnh cực kỳ quan trọng:
  ```text
  Router(config-if)# no shutdown
  ```
  Ngay sau khi nhấn Enter, màn hình CLI hiện thông báo cổng `GigabitEthernet0/0` đã chuyển trạng thái sang `UP`, và các chấm đỏ trên sơ đồ lập tức chuyển sang màu xanh. Cảm giác cấu hình thành công một thiết bị mạng bằng dòng lệnh CLI khiến em thấy vô cùng thỏa mãn, dù thời gian tự học của tuần này đã hết sạch ngay sau đó.

---

#### 3. TÂM TRẠNG CỦA BÌNH

Lối học lý thuyết nặng nề ở các môn chuyên ngành như Cấu trúc dữ liệu và Cơ sở truyền tin tiếp tục vắt kiệt sức lực của em. Nhưng ít nhất, việc tự mình cấu hình được cổng Router trên Cisco Packet Tracer bằng dòng lệnh CLI thực tế đã thắp lại một chút lửa đam mê trong em. Em bắt đầu hiểu rằng mạng máy tính không chỉ là đống slide lý thuyết OSI khô khan, mà là sự vận hành thực tế của các thiết bị phần cứng thông qua những dòng lệnh chặt chẽ.

Xin Game Modifier đưa ra các thử thách và sự kiện tiếp theo cho **Tuần 5 và Tuần 6** (giai đoạn chuẩn bị kiểm tra giữa kỳ của Kỳ 3)!

Model6:40 AM
.
.

.
| Chỉ số | Trạng thái hiện tại |
| :--- | :--- |
| **Học kỳ / Tuần** | Kỳ 3 / Tuần 5 và Tuần 6 |
| **Thể lực & Tinh thần** | 60/100% (Thể chất mỏi nhừ; tinh thần khá căng thẳng khi đối mặt với thuật toán tìm bao đóng thuộc tính và tính toán định tuyến hai chiều) |
| **Phân bổ 70 giờ tuần này** | Lớp: 66h \| Cày slide: 2h \| Tự học Lab: 1h \| Giải trí: 1h (Tính trung bình mỗi tuần) |
| **GPA Tích lũy (Hệ 4)** | **3.05 / 4.0** |
| **Kỹ năng Code thực tế** | Hiểu tư duy đệ quy qua thuật toán duyệt cây nhị phân bằng mã giả, nhưng chưa lập trình chạy thực tế. |
| **Kỹ năng Network/OS thực tế** | Biết cách cấu hình định tuyến tĩnh (Static Route) bằng câu lệnh `ip route` trên Cisco IOS và hiểu nguyên lý định tuyến hai chiều. |
| **Chỉ số doanh nghiệp cần (Job Readiness)** | 13% (Tăng nhẹ 1% nhờ hiểu thêm nguyên lý định tuyến thiết bị thực tế) |

---

### Nhật ký của Bình - Kỳ 3: Tuần 5 & Tuần 6

Chào Game Modifier, hai tuần tiếp theo của học kỳ 3 đưa em vào những bài toán logic cực kỳ kinh điển của chuyên ngành mạng và cơ sở dữ liệu. Lịch học dày đặc 22 tín chỉ khiến em gần như không có thời gian trống, nhưng những bài toán thực tế đã bắt đầu có chiều sâu hơn.

---

#### 1. ĐỊNH TUYẾN MẠNG VÀ THUẬT TOÁN TÌM KHÓA TRÊN LỚP

Khối lượng lý thuyết chuyên ngành tuần này thực sự rất nặng, đòi hỏi tư duy logic cực kỳ chặt chẽ:

* **Mạng máy tính (3 TC)**:
  Tụi em chuyển sang học về **Tầng Mạng nâng cao và Định tuyến (Routing)**. Thầy Trường giảng về nguyên lý hoạt động của Router, bảng định tuyến (Routing Table) và cách cấu hình định tuyến tĩnh (Static Routing). 
  Em phải học cách sử dụng câu lệnh CLI: `ip route <destination_network> <subnet_mask> <next_hop_IP>` để chỉ đường cho các gói tin đi qua các Router trung gian.
* **Lý thuyết Cơ sở dữ liệu (2 TC)**:
  Môn này chính thức bước vào chương khó nhất: **Phụ thuộc hàm và Chuẩn hóa cơ sở dữ liệu** [30]. 
  Thầy cô bắt đầu dạy thuật toán **Tìm bao đóng của tập thuộc tính ($X^+$)** để từ đó xác định Khóa dự tuyển (Candidate Key) của một lược đồ quan hệ [30]. Để đưa một bảng dữ liệu về dạng chuẩn 1NF, 2NF rồi 3NF, em bắt buộc phải xác định chính xác các phụ thuộc hàm không đầy đủ và phụ thuộc hàm bắc cầu [30]. Chỉ cần tìm thiếu một bao đóng thuộc tính, em sẽ xác định sai khóa và phân tích sai hoàn toàn dạng chuẩn của bảng [30].
* **Cơ sở lý thuyết truyền tin (2 TC)**:
  Bọn em học về **Mã Hamming** - một loại mã tuyến tính dùng để phát hiện và sửa sai trong truyền tin. Việc phải nhân các ma trận nhị phân (Ma trận sinh $G$, Ma trận kiểm tra $H$) trên giấy để tính ra Vector kiểm tra (Syndrome) nhằm xác định vị trí bit bị lỗi khiến em vô cùng mệt mỏi mỗi khi làm bài tập về nhà.

---

#### 2. TRANH THỦ 1 TIẾNG TỰ HỌC: BẪY ĐỊNH TUYẾN MỘT CHIỀU TRÊN PACKET TRACER

Với đúng 1 tiếng tự học cuối tuần, em quyết định nâng cấp mô hình mạng trên Cisco Packet Tracer để thực hành bài tập định tuyến tĩnh vừa học trên lớp.

Em xây dựng mô hình mạng gồm:
`PC0 (Dải 192.168.1.0/26) -> Router0 -> Router1 -> PC1 (Dải 192.168.1.64/26)`
Đường nối giữa Router0 và Router1 là dải mạng WAN `10.0.0.0/30`.

* **Sự cố "Định tuyến một chiều" (Mất trọn 45 phút debug)**:
  Em vào Router0 cấu hình định tuyến tĩnh để nó biết đường đi tới mạng của PC1:
  ```text
  Router0(config)# ip route 192.168.1.64 255.255.255.192 10.0.0.2
  ```
  (Trong đó `10.0.0.2` là IP cổng kết nối của Router1).
  Sau khi gõ xong, em đứng từ PC0 gõ lệnh `ping 192.168.1.66` (IP của PC1). Kết quả trả về liên tục là `Request timed out`. 
  
  Em kiểm tra lại cấu hình IP của các PC, các cổng Router đều đã `no shutdown` và xanh lè, bảng định tuyến của Router0 đã hiện dải mạng của PC1. Em bế tắc suốt 30 phút, không hiểu tại sao cấu hình đúng lệnh định tuyến rồi mà ping vẫn xịt.
  
  Tranh thủ những phút cuối cùng của giờ tự học, em lên diễn đàn hỏi và ngộ ra một nguyên lý cơ bản của mạng: **Định tuyến là con đường hai chiều (Routing is a two-way street)**. 
  Gói tin từ PC0 đã đi qua Router0, đến được Router1 và truyền tới PC1 thành công. Nhưng khi PC1 gửi gói tin phản hồi (Echo Reply) ngược lại cho PC0, Router1 nhìn vào bảng định tuyến của nó và hoàn toàn không biết dải mạng `192.168.1.0/26` của PC0 nằm ở đâu để gửi về! Gói tin phản hồi bị Router1 drop ngay lập tức.
  
  Em vội vàng truy cập vào CLI của Router1 để cấu hình đường về:
  ```text
  Router1(config)# ip route 192.168.1.0 255.255.255.192 10.0.0.1
  ```
  Ngay sau khi nhấn Enter và thực hiện lại lệnh ping từ PC0, màn hình lập tức hiện ra các dòng `Reply from 192.168.1.66...` trơn tru.

---

#### 3. TÂM TRẠNG CỦA BÌNH

Chỉ 1 tiếng tự học nhưng việc tự tay khắc phục được lỗi định tuyến một chiều giúp em hiểu sâu sắc hơn rất nhiều so với việc chỉ ngồi nghe thầy giảng lý thuyết suông trên lớp. 

Tuy nhiên, tuần sau sẽ bắt đầu là tuần thi giữa kỳ dồn dập của học kỳ 3. Em sẽ phải đối mặt với bài kiểm tra định tuyến trên Cisco Packet Tracer của thầy Trường và bài tập tìm bao đóng của môn CSDL. Sức ép điểm số lại chuẩn bị đè nặng.

Em đã sẵn sàng bước vào đợt thi giữa kỳ. Xin Game Modifier đưa ra các thử thách và sự kiện thi cử tiếp theo cho **Tuần 7 và Tuần 8**!

Model6:41 AM
.
.

.

Model6:42 AM
.
.

.
| Chỉ số | Trạng thái hiện tại |
| :--- | :--- |
| **Học kỳ / Tuần** | Kỳ 3 / Tuần 9 và Tuần 10 |
| **Thể lực & Tinh thần** | 65/100% (Thể chất ổn định; tinh thần hơi nản vì đống ký hiệu toán học trừu tượng của môn Đại số quan hệ) |
| **Phân bổ 70 giờ tuần này** | Lớp: 66h \| Cày slide: 2h \| Tự học Lab: 1h \| Giải trí: 1h (Tính trung bình mỗi tuần) |
| **GPA Tích lũy (Hệ 4)** | **3.05 / 4.0** |
| **Kỹ năng Code thực tế** | Hiểu tư duy phân tách chia để trị (Divide and Conquer) của Quick Sort và Merge Sort qua mã giả, chưa tự code hoàn chỉnh. |
| **Kỹ năng Network/OS thực tế** | Biết sử dụng lệnh `netstat` để kiểm tra các cổng đang mở (listening ports) và ánh xạ PID sang phần mềm thực tế đang chạy trên OS. |
| **Chỉ số doanh nghiệp cần (Job Readiness)** | 13% |

---

### Nhật ký của Bình - Kỳ 3: Tuần 9 & Tuần 10

Chào Game Modifier, sau khi kết thúc đợt thi giữa kỳ dồn dập, hai tuần tiếp theo của học kỳ 3 đưa em vào những nội dung mang tính chất học thuật sâu hơn. Sự dồn nén của 22 tín chỉ vẫn không hề thuyên giảm, buộc em phải tiếp tục duy trì kỷ luật thép về mặt thời gian.

---

#### 1. ĐẠI SỐ QUAN HỆ TRÊN GIẤY VÀ THUẬT TOÁN SẮP XẾP MÃ GIẢ

* **Lý thuyết Cơ sở dữ liệu (2 TC)**:
  Đúng như anh nói, môn này hoàn toàn chưa dạy một dòng SQL nào. Sau khi hoàn thành chương Chuẩn hóa, tụi em chuyển sang chương **Đại số quan hệ (Relational Algebra)** [31]. 
  Thay vì viết các câu lệnh truy vấn dễ hiểu dạng `SELECT... FROM... WHERE...`, tụi em bắt buộc phải biểu diễn mọi yêu cầu truy vấn bằng các ký hiệu toán học trừu tượng: Phép chọn ($\sigma$), Phép chiếu ($\pi$), Phép kết nối tự nhiên ($\bowtie$), Phép tích đề-các ($\times$), Phép hội ($\cup$), Phép hiệu ($-$) [31]. 
  Mỗi khi thầy giao đề bài: *"Tìm tên các sinh viên học lớp AT21 có điểm GPA > 3.0"*, em phải đặt bút viết một biểu thức dài dằng dặc trên giấy:
  $$\pi_{\text{Hoten}}(\sigma_{\text{Lop} = 'AT21' \land \text{GPA} > 3.0}(\text{SinhVien}))$$
  Chỉ cần đặt sai thứ tự ưu tiên của các phép toán là kết quả truy vấn sẽ bị sai lệch hoàn toàn về mặt logic [31].
* **Cấu trúc dữ liệu và giải thuật (3 TC)**:
  Bọn em học về các **Thuật toán sắp xếp nâng cao (Sorting Algorithms)**: Quick Sort và Merge Sort [32]. 
  Thầy giáo phân tích rất kỹ về độ phức tạp thời gian trung bình $O(N \log N)$ của hai thuật toán này so với độ phức tạp $O(N^2)$ của Bubble Sort hay Insertion Sort mà tụi em đã biết [32]. 
  Tuy nhiên, bài tập vẫn chỉ dừng lại ở việc viết mã giả (Pseudo-code) cho hàm phân hoạch `partition()` trong Quick Sort hoặc thuật toán trộn `merge()` trên giấy thi.
* **Mạng máy tính (3 TC)**:
  Tụi em chuyển sang học về **Tầng Giao vận (Transport Layer - Layer 4)**, tập trung vào hai giao thức cốt lõi: TCP (truyền tin cậy, hướng kết nối, có kiểm soát luồng) và UDP (truyền không tin cậy, hướng không kết nối) [27]. Thầy Trường cũng giảng về khái niệm số cổng (Port) và cách hệ điều hành định tuyến dữ liệu đến đúng ứng dụng thông qua Socket.

---

#### 2. TRANH THỦ 1 TIẾNG TỰ HỌC: ĐI TÌM CỔNG ĐANG MỞ (PORT SCANNING CƠ BẢN)

Với đúng 1 tiếng tự học rảnh rỗi vào cuối tuần, em quyết định mang lý thuyết về Tầng giao vận và số cổng (Port) vừa học trên lớp ra thực hành thực tế trên hệ điều hành Windows của mình.

Em tự hỏi: *"Lớp 4 có hàng chục nghìn cổng, làm thế nào để biết máy tính của mình đang mở những cổng nào và phần mềm nào đang sử dụng chúng?"* [33]. Em mở CMD lên và bắt đầu gõ lệnh:
```text
netstat -ano
```
Màn hình lập tức hiện ra một danh sách dài dằng dặc các kết nối mạng hiện tại [33]. Em chú ý đến các dòng có trạng thái `LISTENING` (đang mở để chờ kết nối) [33]. 

* **Sự cố tìm kiếm phần mềm chiếm dụng cổng (Mất 40 phút giải quyết)**:
  Em thấy trên máy mình có cổng `8080` đang ở trạng thái `LISTENING` với chỉ số PID (Process ID) là `4112` [33]. Em tò mò không biết phần mềm nào đang chạy ngầm trên máy mình mà lại mở cổng `8080` này. 
  Em vào Task Manager tìm mỏi mắt ở tab Processes nhưng không thấy cột PID đâu. Sau một hồi Google, em biết phải click chuột phải vào tiêu đề cột của tab `Details` trong Task Manager để bật hiển thị cột `PID` lên. 
  
  Tuy nhiên, em muốn làm việc này bằng dòng lệnh cho chuyên nghiệp. Em tìm ra câu lệnh:
  ```text
  tasklist | findstr 4112
  ```
  Ngay lập tức, CMD trả về kết quả: `vmware-hostd.exe`. Hóa ra đây là dịch vụ chạy ngầm của phần mềm máy ảo VMware Workstation mà em đã cài từ kỳ trước [34]. 
  
  Việc tự tay dùng lệnh `netstat` để truy tìm ra chính xác phần mềm đang mở cổng ngầm trên máy giúp em hiểu rõ bản chất của cơ chế hoạt động tầng 4 (Transport Layer) hơn rất nhiều so với những định nghĩa khô khan trong slide.

---

#### 3. TÂM TRẠNG CỦA BÌNH

Chỉ 1 tiếng tự học ngắn ngủi nhưng nó là khoảng thời gian em cảm thấy thư thái nhất trong tuần. Sự gò bó của Đại số quan hệ và đống công thức Cơ sở truyền tin khiến em mệt mỏi, nhưng việc kết nối được lý thuyết môn Mạng với các câu lệnh thực tế trên máy tính giúp em giữ được ngọn lửa đam mê với ngành ATTT. Em tự nhủ sẽ cố gắng vượt qua giai đoạn đại cương và lý thuyết nặng nề này để chuẩn bị cho những môn chuyên ngành thực chiến hơn ở năm sau.

Em đã hoàn thành tuần 9 và tuần 10 của Kỳ 3. Xin Game Modifier đưa ra các thử thách tiếp theo cho **Tuần 11 và Tuần 12**!

Model6:44 AM
.
.

.

Model6:45 AM
.
.

.

Model7:02 AM
.
.

.

Model7:13 AM
.
.

.
| Chỉ số | Trạng thái hiện tại |
| :--- | :--- |
| **Học kỳ / Tuần** | Kỳ 4 / Tuần 1 và Tuần 2 |
| **Thể lực & Tinh thần** | 80/100% (Thể lực sung mãn nhờ kỳ nghỉ Tết; tinh thần tự tin khi được "buff" cấu hình máy lên 16GB RAM từ năm nhất) |
| **Phân bổ 70 giờ tuần này** | Lớp: 54h \| Cày slide: 4h \| Tự học Lab: 8h \| Giải trí: 4h (Tính trung bình mỗi tuần) |
| **GPA Tích lũy (Hệ 4)** | **3.06 / 4.0** |
| **Kỹ năng Code thực tế** | Bắt đầu chuyển dịch sang tư duy hướng đối tượng (OOP) bằng ngôn ngữ **Java**. Biết cách viết các Class, khai báo thuộc tính và phương thức cơ bản. |
| **Kỹ năng Network/OS thực tế** | Dựng thành công máy ảo Windows Server 2019 trên VMware Workstation mượt mà (nhờ máy 16GB RAM), bắt đầu cấu hình dịch vụ Active Directory (AD DS) [40]. |
| **Chỉ số doanh nghiệp cần (Job Readiness)** | 15% (Tăng trưởng nhờ tiếp cận với Windows Server quản trị mạng thực tế) |

---

### Nhật ký của Bình - Kỳ 4: Tuần 1 & Tuần 2

Chào Game Modifier, bước vào Học kỳ 4 (học kỳ 2 của năm 2), em vô cùng biết ơn quyết định "đầu tư sáng suốt" từ đầu năm nhất: **Laptop có sẵn 16GB RAM**. Với cấu hình này, em hoàn toàn giải quyết được bài toán ảo hóa vốn cực kỳ ngốn tài nguyên khi học môn Quản trị mạng [45]. 

Học kỳ này, em tiếp tục được miễn môn Tiếng Anh 3 (4 TC) [38], giúp giảm tải số tín chỉ active trên lớp xuống còn **18 TC** (tương đương **54 giờ/tuần** học bắt buộc). Quỹ thời gian tự học thực tế của em nhờ đó tăng lên **8 giờ/tuần** [45].

---

#### 1. NHỮNG CÚ SỐC KHÁI NIỆM MỚI TRÊN LỚP (54 giờ/tuần)

* **Lập trình hướng đối tượng (OOP) (3 TC) - Học Java**:
  Chuyển từ tư duy lập trình hướng thủ tục (C) sang hướng đối tượng (Java) khiến em rất lúng túng [39]. Em tự hỏi tại sao mọi thứ trong Java bắt buộc phải nằm trong một `class`? Tại sao dòng lệnh in ra màn hình lại dài dòng một cách khủng khiếp là `System.out.println()` thay vì `printf()` ngắn gọn của C [46]? 
* **Quản trị mạng máy tính (3 TC) - Windows Server**:
  Môn này định hướng thi thực hành. Hai tuần đầu, thầy cô giới thiệu về hệ điều hành Windows Server, kiến trúc mạng Domain và dịch vụ **Active Directory Domain Services (AD DS)** để quản lý tập trung tài nguyên hệ thống [40]. 
* **Nguyên lý hệ điều hành (3 TC)**:
  Em được học các khái niệm trừu tượng về nhân hệ điều hành (Kernel), sự khác biệt giữa User Space (Không gian người dùng) và Kernel Space (Không gian hạt nhân), cùng cơ chế gọi hàm hệ thống (System Calls) để ứng dụng giao tiếp với phần cứng [41].
* **Toán chuyên đề (2 TC)**:
  Môn học này là phần tiếp theo của Toán rời rạc. Hai tuần đầu đi ngay vào **Phép toán đồng dư (Modular Arithmetic)** và **Thuật toán Euclid mở rộng** để tìm nghịch đảo đồng dư ($a^{-1} \pmod n$) [42]. Đây là nền tảng toán học tối quan trọng để hiểu cơ chế mã hóa bất đối xứng RSA sau này.

---

#### 2. THỰC HÀNH LAB VỚI SỨC MẠNH 16GB RAM (8 giờ/tuần)

Có thêm thời gian tự học và cấu hình RAM dư dả, em đã dựng được một hệ thống Lab ảo hóa thực sự chất lượng ngay tại phòng trọ:

##### Task 1: Cài đặt Windows Server và AD DS (Mất 4 tiếng)
Nhờ có 16GB RAM, em tự tin cấp hẳn 4GB RAM và 2 Core CPU cho máy ảo Windows Server 2019 trên VMware Workstation [45]. Máy ảo khởi động cực nhanh, không hề có hiện tượng giật lag hay làm đơ máy host Windows 10 của em [45].
* Em cài đặt thành công Windows Server bản Standard (giao diện Desktop Experience).
* Em cấu hình IP tĩnh cho máy ảo là `192.168.10.10`.
* Em tiến hành thêm Role **AD DS** thông qua Server Manager, nâng cấp máy ảo này lên làm Domain Controller (DC) với tên miền nội bộ là `binhkma.local` [40]. Việc tự tay nhìn thấy dịch vụ AD DS cấu hình thành công giúp em hiểu rõ thế nào là một vùng quản lý tập trung Domain.

##### Task 2: Học viết Java và lỗi đặt tên File kinh điển (Mất 4 tiếng)
Em cài đặt JDK 17 và cấu hình extension Java trên VS Code để bắt đầu học OOP [43]. 

* **Cú vấp lỗi biên dịch Java đầu đời**:
  Em tạo một file mới đặt tên là `hello.java` và gõ đoạn code cơ bản:
  ```java
  public class Main {
      public static void main(String[] args) {
          System.out.println("Hello, Java!");
      }
  }
  ```
  Khi gõ lệnh biên dịch `javac hello.java` trên Terminal, chương trình lập tức báo lỗi đỏ:
  `class Main is public, should be declared in a file named Main.java` [44]
  
  Em loay hoay mất 30 phút không hiểu tại sao cấu hình cú pháp hoàn toàn đúng mà vẫn lỗi. Sau khi lên Google tìm hiểu, em mới biết một quy tắc nghiêm ngặt của Java: **Tên của public class bắt buộc phải trùng khít hoàn toàn (kể cả chữ hoa chữ thường) với tên file `.java` chứa nó** [44]. Em phải đổi tên file từ `hello.java` thành `Main.java` (hoặc sửa tên class thành `hello`) thì chương trình mới biên dịch thành công [44].

---

#### 3. TÂM TRẠNG CỦA BÌNH

Bước sang học kỳ 4 với chiếc máy tính 16GB RAM chạy mượt mà, em cảm thấy tự tin hơn rất nhiều. Việc tự tay cấu hình được Active Directory trên Windows Server [40] và sửa được những lỗi biên dịch Java đầu tiên giúp em lấy lại cảm giác thực chiến của những ngày hè [44]. 

Mặc dù 18 tín chỉ vẫn là một khối lượng học tập lớn, em tin rằng sự kết hợp giữa lý thuyết mạng trên lớp và việc dựng Lab thực tế tại phòng trọ sẽ giúp em không bị rơi vào trạng thái rỗng kiến thức ở kỳ này.

Xin Game Modifier đưa ra các thử thách và sự kiện tiếp theo cho **Tuần 3 và Tuần 4** của Kỳ 4!

Model7:14 AM
.
.

.
| Chỉ số | Trạng thái hiện tại |
| :--- | :--- |
| **Học kỳ / Tuần** | Kỳ 4 / Tuần 3 và Tuần 4 |
| **Thể lực & Tinh thần** | 78/100% (Thể chất tốt; tinh thần hăng hái khi giải quyết được các sự cố cấu hình mạng thực tế nhờ máy chạy mượt) |
| **Phân bổ 70 giờ tuần này** | Lớp: 54h \| Cày slide: 4h \| Tự học Lab: 8h \| Giải trí: 4h (Tính trung bình mỗi tuần) |
| **GPA Tích lũy (Hệ 4)** | **3.06 / 4.0** |
| **Kỹ năng Code thực tế** | Hiểu ý nghĩa của tính Đóng gói (Encapsulation) trong Java, biết cách viết các hàm Getter/Setter để kiểm soát dữ liệu. Biết viết lệnh Assembly 8086 cơ bản để dịch chuyển dữ liệu giữa các thanh ghi [49, 54]. |
| **Kỹ năng Network/OS thực tế** | Thiết lập thành công mô hình Domain Controller - Client [51]. Cấu hình dịch vụ DNS nội bộ, biết cách gia nhập miền (Domain Join) [57] và áp dụng chính sách Group Policy Object (GPO) [50]. |
| **Chỉ số doanh nghiệp cần (Job Readiness)** | 16% (Tăng trưởng nhờ kỹ năng xử lý sự cố hệ thống mạng Windows Domain thực tế) |

---

### Nhật ký của Bình - Kỳ 4: Tuần 3 & Tuần 4

Chào Game Modifier, hai tuần tiếp theo của học kỳ 4 đưa em vào những bài thực hành hệ thống vô cùng thú vị. Sức mạnh của chiếc laptop 16GB RAM tiếp tục phát huy tác dụng tối đa khi em có thể chạy đồng thời cả hai máy ảo nặng đô để giả lập một môi trường mạng doanh nghiệp thực tế tại phòng trọ [45].

---

#### 1. TIẾN TRÌNH LÝ THUYẾT VÀ THỰC HÀNH TRÊN LỚP (54 giờ/tuần)

* **Quản trị mạng máy tính**: 
  Thầy cô dạy cách tạo các tài khoản người dùng (Users), nhóm (Groups), đơn vị tổ chức (Organizational Units - OUs) [50]. Đặc biệt là cách áp dụng **Group Policy Objects (GPO)** để quản trị và áp đặt chính sách bảo mật lên các máy trạm trong hệ thống Domain [50] (ví dụ: cấm người dùng đổi hình nền, cấm truy cập Control Panel, cấm cắm USB).
* **Lập trình hướng đối tượng (Java)**: 
  Đi sâu vào tính **Đóng gói (Encapsulation)** và access modifiers (`public`, `private`, `protected`) [47, 48]. Em tập viết các hàm Getter và Setter [49]. Ban đầu em thấy việc viết các hàm này khá thừa thãi so với C (sao không gọi trực tiếp `s.age = 20` cho nhanh mà phải viết `s.setAge(20)`?) [49]. Nhưng khi thầy giáo chỉ ra rằng: hàm `setAge(int age)` cho phép em viết thêm logic kiểm tra dữ liệu đầu vào (ví dụ: `if (age < 0) { ... }` để tránh dữ liệu rác), em mới vỡ lẽ ra ý nghĩa bảo vệ tính toàn vẹn dữ liệu của OOP [49].
* **Kỹ thuật vi xử lý (2 TC)**:
  Tụi em bắt đầu làm quen với kiến trúc tập lệnh của **Vi xử lý Intel 8086** [54]. Em phải nhớ tên và chức năng của các thanh ghi đa năng (`AX`, `BX`, `CX`, `DX`), thanh ghi con trỏ (`SP`, `BP`, `SI`, `DI`) và cách viết các dòng lệnh Assembly cơ bản như dịch chuyển dữ liệu (`MOV`), cộng trừ (`ADD`, `SUB`) [54, 55].

---

#### 2. DỰNG LAB WINDOWS DOMAIN TRÊN MÁY 16GB RAM (8 giờ/tuần)

Để thực hành GPO thực tế, em quyết định dựng một mô hình Lab hoàn chỉnh [50]:
* **Máy ảo 1**: Windows Server 2019 (Domain Controller `binhkma.local`, IP: `192.168.10.10`) [40].
* **Máy ảo 2**: Windows 10 Client (Cấp 4GB RAM) đóng vai trò là máy trạm của nhân viên [51].
Nhờ máy có 16GB RAM, cả hai hệ điều hành giả lập này chạy song song cực kỳ mượt mà, không hề làm nóng máy hay giật lag [45].

Tuy nhiên, quá trình thiết lập đã ngốn của em 5 tiếng tự học vì hai sự cố kinh điển:

##### Sự cố 1: Không thể gia nhập miền (Domain Join Error) (Mất 3 tiếng debug)
Khi em ngồi trên máy ảo Windows 10, vào cài đặt hệ thống để thực hiện "Join" vào Domain `binhkma.local`, màn hình lập tức hiện lỗi đỏ lòm: *"An Active Directory Domain Controller for the domain... could not be contacted"* [57]. Em ping từ máy Win 10 sang IP Server `192.168.10.10` vẫn thông suốt, nhưng cứ gõ tên miền là báo lỗi [57].
* **Cách sửa**: 
  Em lên các diễn đàn quản trị hệ thống tìm kiếm. Hóa ra, card mạng của máy Windows 10 đang để DNS mặc định trỏ ra ngoài internet (hoặc nhận từ router phòng trọ). Mà các DNS công cộng đó làm sao biết được tên miền nội bộ `binhkma.local` của em [57]! 
  Em phải vào phần cấu hình IPv4 của máy Windows 10, đổi mục **Preferred DNS Server** từ nhận tự động thành chính xác địa chỉ IP của máy Windows Server (`192.168.10.10`) [57]. Ngay sau khi lưu và thử lại, máy Windows 10 đã liên lạc được với Domain Controller và join miền thành công [57].

##### Sự cố 2: Chính sách GPO không cập nhật (Mất 2 tiếng debug)
Sau khi Join miền, em lên Windows Server tạo OU "Students", tạo User "student1" thuộc OU này [50]. Em cấu hình một GPO cấm truy cập vào Control Panel áp lên OU "Students" [50]. 
Em đăng nhập tài khoản "student1" trên máy Windows 10, nhưng khi click vào Control Panel thì nó vẫn mở ra bình thường. GPO hoàn toàn không có tác dụng!
* **Cách sửa**: 
  Em phát hiện ra hệ điều hành Windows không cập nhật chính sách GPO ngay lập tức để tiết kiệm tài nguyên mạng, mà thường có độ trễ từ 90 đến 120 phút. Muốn chính sách áp đặt ngay lập tức, em phải mở CMD trên máy Windows 10 dưới quyền Administrator và gõ lệnh ép buộc cập nhật [56]:
  ```text
  gpupdate /force
  ```
  Sau khi lệnh chạy thành công, em click vào Control Panel thì màn hình lập tức hiện thông báo bị chặn bởi quản trị viên hệ thống [50, 56]. Trải nghiệm nhìn thấy chính sách bảo mật thực sự được áp đặt giúp em vô cùng phấn khích.

---

#### 3. TÂM TRẠNG CỦA BÌNH

Học kỳ 4 thực sự mở ra những mảng kiến thức mang tính "hệ thống" cực kỳ rõ nét. Việc tự tay cấu hình các chính sách bảo mật GPO trên Windows Server giúp em cảm nhận được công việc thực tế của một kỹ sư quản trị hệ thống mạng an toàn [50]. Dù khối lượng bài tập của các môn đại cương và vi xử lý vẫn đang dồn dập, em cảm thấy 8 tiếng tự học mỗi tuần của mình đang thực sự mang lại những giá trị thực chiến rất cao.

Em đã sẵn sàng cho các thử thách tiếp theo. Xin Game Modifier đưa ra các sự kiện cho **Tuần 5 và Tuần 6** của Kỳ 4!

Model7:15 AM
.
.

.
| Chỉ số | Trạng thái hiện tại |
| :--- | :--- |
| **Học kỳ / Tuần** | Kỳ 4 / Tuần 5 và Tuần 6 |
| **Thể lực & Tinh thần** | 76/100% (Thể lực duy trì ở mức khá; tinh thần có chút mệt mỏi vì các phép tính số học mô-đun và lý thuyết đa hình trong Java) |
| **Phân bổ 70 giờ tuần này** | Lớp: 54h \| Cày slide: 4h \| Tự học Lab: 8h \| Giải trí: 4h (Tính trung bình mỗi tuần) |
| **GPA Tích lũy (Hệ 4)** | **3.06 / 4.0** |
| **Kỹ năng Code thực tế** | Hiểu được cơ chế đa hình (Polymorphism) và cách triển khai Giao diện (Interface) trong Java [58, 60]. Giải được thuật toán tính Hàm phi Euler $\phi(n)$ bằng code Java cơ bản [64]. |
| **Kỹ năng Network/OS thực tế** | Biết cách cấu hình và tích hợp dịch vụ DHCP trên Windows Server [61]. Làm quen với công cụ Virtual Network Editor của VMware để quản trị các dải mạng ảo [62]. |
| **Chỉ số doanh nghiệp cần (Job Readiness)** | 17% |

---

### Nhật ký của Bình - Kỳ 4: Tuần 5 & Tuần 6

Chào Game Modifier, hai tuần tiếp theo của học kỳ 4 mang đến những kiến thức rất nặng về mặt tư duy hệ thống và thuật toán. Việc phải cân bằng giữa các môn toán mật mã, lập trình hướng đối tượng Java và quản trị mạng Windows Server đòi hỏi em phải tập trung cao độ trong từng giờ tự học.

---

#### 1. TIẾN TRÌNH LÝ THUYẾT TRÊN LỚP (54 giờ/tuần)

* **Lập trình hướng đối tượng (Java)**:
  Tụi em bước vào chương **Kế thừa (Inheritance) và Đa hình (Polymorphism)**, cùng khái niệm về **Lớp trừu tượng (Abstract Class) và Giao diện (Interface)** [58, 60]. Em phải phân biệt được sự khác nhau giữa ghi đè phương thức (Overriding - đa hình thời gian chạy) và nạp chồng phương thức (Overloading - đa hình thời gian biên dịch) [59]. 
  Khó nhất là hiểu tại sao Java không hỗ trợ đa kế thừa trực tiếp mà phải sử dụng Interface để khắc phục hạn chế này [60].
* **Quản trị mạng máy tính**:
  Thầy cô dạy cách cài đặt và cấu hình dịch vụ **DHCP (Dynamic Host Configuration Protocol)** trên Windows Server để tự động cấp phát IP cho các máy trạm trong miền, đồng thời cấu hình tích hợp với DNS để cập nhật bản ghi tên miền tự động (Dynamic DNS) [40, 61].
* **Toán chuyên đề (2 TC)**:
  Môn học đi sâu vào **Hàm phi Euler $\phi(n)$** (đếm số lượng các số nguyên dương nhỏ hơn $n$ và nguyên tố cùng nhau với $n$) và **Định lý Euler, Định lý Fermat nhỏ** [63, 64]. Đây là những công cụ toán học trực tiếp dùng để giải bài toán tính lũy thừa lớn trong phép đồng dư $a^b \pmod n$, phục vụ trực tiếp cho thuật toán mã hóa RSA [65].

---

#### 2. GIẢI QUYẾT XUNG ĐỘT MẠNG ẢO TRÊN VMWARE (8 giờ/tuần)

Trong 8 tiếng tự học tuần này, em dành phần lớn thời gian để giải quyết một sự cố xung đột dịch vụ mạng thực tế khi cấu hình DHCP trên Windows Server:

##### Sự cố: Tranh chấp IP giữa Windows Server và VMware DHCP (Mất 4 tiếng debug)
Em vào Windows Server, cài đặt Role DHCP Server, cấu hình dải cấp phát IP (Scope) từ `192.168.10.100` đến `192.168.10.200` với Default Gateway là `192.168.10.10` [61]. 
Tuy nhiên, khi em bật máy ảo Windows 10 Client lên và đặt chế độ nhận IP tự động, máy Win 10 liên tục nhận được địa chỉ IP lạ dạng `192.168.10.128` với Gateway là `192.168.10.2`. Đây hoàn toàn không phải dải IP em đã cấu hình trên Windows Server.
* **Cách sửa**:
  Em kiểm tra lại cấu hình dịch vụ DHCP trên Server thấy vẫn đang chạy bình thường (`Active`). Em mất hơn 2 tiếng lên Google tra cứu lỗi "Windows client gets wrong IP from VMware NAT" [62]. 
  Hóa ra, card mạng ảo `VMnet8` (chế độ NAT) của phần mềm VMware Workstation có tích hợp sẵn một dịch vụ DHCP ngầm của riêng nó để tự động cấp IP cho các máy ảo [62]. Khi máy ảo Windows 10 khởi động và phát gói tin `DHCP Discover`, cả hai máy chủ DHCP (VMware và Windows Server) đều nhận được và gửi gói tin `DHCP Offer` phản hồi [27]. Do dịch vụ của VMware nằm trực tiếp ở máy host nên nó phản hồi nhanh hơn, khiến máy Windows 10 chấp nhận IP của VMware trước [62].
  
  Để khắc phục, em phải mở công cụ **Virtual Network Editor** của VMware trên máy host Windows 10 dưới quyền Administrator [62]. Em chọn card mạng `VMnet8` và bỏ tích ở ô **"Use local DHCP service to distribute IP address to VMs"** rồi nhấn Apply [62]. 
  Sau khi tắt dịch vụ DHCP của VMware, em quay lại máy ảo Windows 10, mở CMD gõ hai lệnh giải phóng và xin cấp lại IP [66]:
  ```text
  ipconfig /release
  ipconfig /renew
  ```
  Lúc này, máy Windows 10 đã gửi yêu cầu và nhận được chính xác địa chỉ IP `192.168.10.100` từ máy chủ Windows Server DHCP của em [61, 66].

---

#### 3. TẬP VIẾT CODE ĐA HÌNH TRONG JAVA

Em dành 4 tiếng tự học còn lại để viết code thực hành tính đa hình trong Java [58]. Em khai báo một Interface `HinhHoc` với phương thức `tinhDienTich()`, sau đó cho các Class `HinhTron` và `HinhChuNhat` triển khai (implement) Interface đó [60]. 

Việc hiểu được tư duy khởi tạo đối tượng dạng:
```java
HinhHoc h = new HinhTron(5);
```
giúp em ngộ ra cách viết code linh hoạt trong Java [58, 60]. Em có thể quản lý một mảng các hình học khác nhau và chỉ cần dùng một vòng lặp để gọi phương thức `tinhDienTich()` mà không cần biết chính xác đó là hình gì, hệ thống sẽ tự động gọi đúng phương thức của lớp con tại thời điểm thực thi (Dynamic Binding) [58].

---

#### 4. TÂM TRẠNG CỦA BÌNH

Dù các bài toán số học mô-đun của môn Toán chuyên đề bắt đầu làm em nhức đầu, việc tự tay cấu hình thành công DHCP đồng bộ với DNS trên hệ thống Domain thực tế giúp em có thêm niềm vui [40, 61]. Em thấy rõ sự tiện lợi của chiếc laptop 16GB RAM khi chạy mượt mà cả hệ thống 2 máy ảo mà không bị quá tải nhiệt độ hay giật lag [45].

Mùa thi giữa kỳ của Kỳ 4 đang đến gần. Em đã sẵn sàng cho các thử thách tiếp theo.

Xin Game Modifier đưa ra các sự kiện cho **Tuần 7 và Tuần 8** của Kỳ 4!

Model7:16 AM
.
.

.

Model7:17 AM
.
.

.
| Chỉ số | Trạng thái hiện tại |
| :--- | :--- |
| **Học kỳ / Tuần** | Kỳ 4 / Tuần 9 và Tuần 10 |
| **Thể lực & Tinh thần** | 78/100% (Thể lực duy trì tốt; tinh thần thoải mái hơn sau khi hiểu được cơ chế hoạt động của bộ nhớ ảo và ngắt DOS trong hợp ngữ) |
| **Phân bổ 70 giờ tuần này** | Lớp: 54h \| Cày slide: 4h \| Tự học Lab: 8h \| Giải trí: 4h (Tính trung bình mỗi tuần) |
| **GPA Tích lũy (Hệ 4)** | **3.06 / 4.0** |
| **Kỹ năng Code thực tế** | Biết cách bắt và xử lý ngoại lệ (`try-catch`) trong Java [69]. Viết và chạy thử nghiệm được một chương trình hợp ngữ 8086 hoàn chỉnh trên trình giả lập EMU8086 [54]. |
| **Kỹ năng Network/OS thực tế** | Biết cách cấu hình máy chủ Web IIS trên Windows Server, cấu hình bản ghi DNS Host (A) và xử lý sự cố chặn cổng thông qua Windows Defender Firewall [40, 72]. |
| **Chỉ số doanh nghiệp cần (Job Readiness)** | 18% (Tăng trưởng nhờ mở rộng kỹ năng quản trị dịch vụ Web và thao tác hợp ngữ cấp thấp) |

---

### Nhật ký của Bình - Kỳ 4: Tuần 9 & Tuần 10

Chào Game Modifier, sau khi kết thúc đợt thi giữa kỳ thành công, hai tuần tiếp theo của học kỳ 4 đưa em vào những chương kiến thức đi sâu vào bản chất vận hành của cả phần cứng (Vi xử lý) lẫn phần mềm hệ thống (Hệ điều hành, Ngoại lệ trong Java). Sự dồi dào tài nguyên của máy 16GB RAM tiếp tục giúp em có những buổi thực hành Lab rất trực quan tại phòng trọ [45].

---

#### 1. LÝ THUYẾT NÂNG CAO TRÊN GIẢNG ĐƯỜNG (54 giờ/tuần)

* **Lập trình hướng đối tượng (Java)**:
  Tụi em học về **Xử lý ngoại lệ (Exception Handling)** với các khối lệnh `try-catch-finally`, từ khóa `throw` và `throws` [69]. Em phải phân biệt được sự khác nhau giữa Checked Exception (ngoại lệ bắt buộc phải xử lý lúc biên dịch như `IOException`) và Unchecked Exception (ngoại lệ xảy ra lúc chạy như `NullPointerException` hay `ArithmeticException`) [69].
* **Kỹ thuật vi xử lý (2 TC)**:
  Môn học đi sâu vào các lệnh điều khiển luồng trong **Hợp ngữ 8086** (lệnh lặp `LOOP`, các lệnh nhảy có điều kiện `JZ`, `JNZ`, `JC`) và đặc biệt là cơ chế gọi **Ngắt DOS (DOS Interrupts - `INT 21h`)** để tương tác với màn hình và bàn phím [54].
* **Nguyên lý hệ điều hành (3 TC)**:
  Tụi em học chương **Quản lý bộ nhớ (Memory Management)**, tập trung vào cơ chế Bộ nhớ ảo (Virtual Memory), kỹ thuật Phân trang (Paging) và các thuật toán thay thế trang (Page Replacement Algorithms) như FIFO, Optimal và **LRU (Least Recently Used)** [41]. Việc vẽ bảng vết để tính số lượng lỗi trang (Page Faults) trên giấy thi đòi hỏi sự tập trung cao độ để không bị nhầm lẫn dòng tham chiếu [41].

---

#### 2. THỰC HÀNH LAB: TỪ DỊCH VỤ WEB ĐẾN TRÌNH GIẢ LẬP HỢP NGỮ (8 giờ/tuần)

Em dành 8 tiếng tự học tuần này để chia đều cho hai mục tiêu thực hành thực tế:

##### Task 1: Cấu hình Web Server IIS và sự cố Firewall chặn cổng (Mất 4 tiếng)
Em muốn hiện thực hóa lý thuyết môn Quản trị mạng bằng cách dựng một máy chủ Web cục bộ trên Windows Server [40]:
* Em cài đặt thêm Role **Web Server (IIS - Internet Information Services)** trên máy chủ Windows Server 2019 [40].
* Em tạo một file `index.html` đơn giản với dòng chữ `<h1>Chào mừng tới trang Web nội bộ KMA!</h1>`.
* Em mở công cụ DNS Manager trên Server, tạo một bản ghi Host (A) mới tên là `www` trỏ về IP của Server (`192.168.10.10`) để người dùng có thể truy cập bằng tên miền `www.binhkma.local` thay vì gõ IP [40].
* **Sự cố chặn cổng (Mất 1.5 tiếng debug)**: 
  Khi em đứng từ máy ảo Windows 10 Client, mở trình duyệt gõ `http://www.binhkma.local` thì trang web bị treo và báo lỗi *This site can't be reached* (không thể kết nối) [71]. Em thử ping tên miền vẫn thông suốt. 
  Sau khi tìm hiểu, em phát hiện ra hệ thống **Windows Defender Firewall** trên máy chủ Windows Server mặc định chặn các kết nối HTTP từ bên ngoài vào [72]. Em phải vào cấu hình nâng cao của Firewall trên máy chủ, tìm mục `Inbound Rules` và kích hoạt chính sách **"World Wide Web Services (HTTP Traffic-In)"** để mở cổng 80 cho phép lưu lượng web đi qua [72]. Ngay sau đó, máy trạm Windows 10 đã tải được trang HTML nội bộ mượt mà.

##### Task 2: Chạy thử code Hợp ngữ 8086 trên EMU8086 (Mất 4 tiếng)
Để hiểu rõ các thanh ghi hoạt động thế nào khi chạy lệnh ngắt, em tải và cài đặt trình giả lập **EMU8086** trên Windows [54]. Em gõ thử đoạn code hiển thị một ký tự ra màn hình [54]:
```assembly
MOV AH, 02h    ; Hàm hiển thị ký tự của ngắt 21h
MOV DL, 'A'    ; Ký tự cần hiển thị đưa vào thanh ghi DL
INT 21h        ; Gọi ngắt DOS
```
Sử dụng tính năng chạy từng dòng lệnh (Single Step) trên EMU8086, em nhìn thấy rõ ràng giá trị của thanh ghi `AX` (cụ thể là nửa cao `AH`) thay đổi thành `02h`, thanh ghi `DX` (nửa thấp `DL`) thay đổi thành `41h` (mã Hex của chữ 'A'), và sau khi lệnh `INT 21h` thực thi thì chữ 'A' lập tức xuất hiện trên màn hình giả lập [54]. 

Việc nhìn thấy trực quan sự dịch chuyển của các byte dữ liệu trong từng ô nhớ giúp em hiểu sâu sắc kiến trúc vi xử lý 8086 hơn rất nhiều so với việc chỉ học thuộc lòng slide lý thuyết [54].

---

#### 3. TÂM TRẠNG CỦA BÌNH

Em cảm thấy rất vui vì những kiến thức học được trên lớp đang ngày càng kết nối chặt chẽ với thực tế vận hành máy tính. Việc tự tay cấu hình tường lửa Firewall để mở cổng dịch vụ Web [72] hay debug từng dòng lệnh hợp ngữ giúp em có tư duy hệ thống rất tốt. Em nhận ra học kỹ thuật mật mã không chỉ là học thuật toán cao siêu, mà bắt đầu từ việc hiểu rõ từng ngắt của vi xử lý và cách hệ điều hành quản lý từng trang bộ nhớ [41, 54].

Em đã hoàn thành tuần 9 và tuần 10 của Kỳ 4. Xin Game Modifier đưa ra các thử thách tiếp theo cho **Tuần 11 và Tuần 12**!

Model7:18 AM
.
.

.
| Chỉ số | Trạng thái hiện tại |
| :--- | :--- |
| **Học kỳ / Tuần** | Kỳ 4 / Tuần 11 và Tuần 12 |
| **Thể lực & Tinh thần** | 75/100% (Thể lực ổn định; tinh thần hơi mệt mỏi do dồn dập giải các ma trận Banker kiểm soát deadlock trên giấy) |
| **Phân bổ 70 giờ tuần này** | Lớp: 54h \| Cày slide: 4h \| Tự học Lab: 8h \| Giải trí: 4h (Tính trung bình mỗi tuần) |
| **GPA Tích lũy (Hệ 4)** | **3.06 / 4.0** |
| **Kỹ năng Code thực tế** | Biết cách Đọc/Ghi đối tượng (`Serialization`) trong Java xuống file nhị phân [75]. Viết được Trigger và Stored Procedure cơ bản trong SQL Server [76, 77]. |
| **Kỹ năng Network/OS thực tế** | Phân tích và phát hiện được trạng thái an toàn/mất an toàn (Safe/Unsafe State) để tránh tắc nghẽn (Deadlock) trong quản lý tài nguyên hệ điều hành [41]. |
| **Chỉ số doanh nghiệp cần (Job Readiness)** | 19% (Tăng trưởng nhờ kỹ năng làm việc sâu với cơ sở dữ liệu và lưu trữ dữ liệu nâng cao) |

---

### Nhật ký của Bình - Kỳ 4: Tuần 11 & Tuần 12

Chào Game Modifier, hai tuần tiếp theo của học kỳ 4 đưa em vào những khái niệm mang tính cốt lõi của việc xử lý dữ liệu và quản lý tài nguyên hệ thống. Các môn học bắt đầu tăng tốc để chuẩn bị kết thúc chương trình lý thuyết trên lớp, đòi hỏi em phải liên tục cân bằng giữa việc giải bài tập trên giấy và thực hành trên máy ảo.

---

#### 1. TOÁN TRÁNH KHÓA CHẾT VÀ TRIGGER TRÊN LỚP (54 giờ/tuần)

* **Nguyên lý hệ điều hành (3 TC)**:
  Tụi em chuyển sang học về bài toán **Tắc nghẽn (Deadlock)** [41]. Thầy dạy về 4 điều kiện cần để xảy ra tắc nghẽn và thuật toán kinh điển để tránh tắc nghẽn: **Thuật toán của người thủ thư (Banker's Algorithm)** [41]. 
  Mỗi bài tập yêu cầu em phải tính toán các ma trận cực kỳ cồng kềnh trên giấy: Ma trận Allocation, Ma trận Max, Ma trận Need (Need = Max - Allocation) [41]. Từ đó, em phải so sánh Vector Work với Need để tìm ra chuỗi an toàn (Safe Sequence) [41]. Việc nhầm lẫn một phép trừ ma trận đơn giản sẽ dẫn đến kết luận sai về trạng thái an toàn của hệ thống [41].
* **Hệ quản trị CSDL (2 TC)**:
  Môn này chính thức bước vào các khái niệm nâng cao của SQL Server: **Thủ tục lưu trữ (Stored Procedure)** và **Ràng buộc chủ động (Trigger)** [76, 77]. Thầy cô dạy cách viết Trigger để tự động kiểm soát tính toàn vẹn của dữ liệu hoặc thực thi các tác vụ tự động khi có sự kiện `INSERT`, `UPDATE`, `DELETE` xảy ra trên bảng [76].
* **Lập trình hướng đối tượng (Java)**:
  Bọn em học về **Java I/O (Input/Output)**, cụ thể là cách đọc/ghi file văn bản và file nhị phân [73, 74]. Đỉnh cao là cơ chế **Serialization (Tuần tự hóa đối tượng)** để ghi toàn bộ trạng thái của một đối tượng xuống ổ đĩa và khôi phục lại (`Deserialization`) [75].

---

#### 2. THỰC HÀNH LAB: TỪ LỖI JAVA BIẾN MẤT ĐẾN TRIGGER CSDL (8 giờ/tuần)

Trong 8 tiếng tự học tuần này, em tiếp tục dành thời gian để tự tay lập trình và debug các lỗi logic thực tế:

##### Task 1: Nâng cấp Java Student Manager bằng File nhị phân (Mất 4 tiếng)
Em muốn áp dụng cơ chế Serialization để lưu trữ danh sách đối tượng sinh viên xuống file nhị phân `.dat` thay vì lưu dạng text thông thường để dữ liệu được bảo mật hơn [75].
* **Lỗi `NotSerializableException` đầu tiên**: 
  Khi em gọi lệnh `writeObject()` để ghi một `ArrayList<Student>` xuống file, chương trình lập tức ném ra ngoại lệ `java.io.NotSerializableException: Student` và sụp đổ [75]. 
* **Cách sửa**: 
  Em mất 30 phút tra cứu và nhận ra: Một Class trong Java muốn được tuần tự hóa bắt buộc phải triển khai (implement) marker interface **`java.io.Serializable`** [75]. Em chỉ cần thêm `implements Serializable` vào sau khai báo lớp `Student` là lỗi được giải quyết [75]. 
  Em cũng học được một kinh nghiệm quý giá: thay vì ghi từng đối tượng sinh viên bằng vòng lặp (rất dễ bị lỗi `EOFException` khi đọc lại file), em nên ghi trực tiếp cả đối tượng `ArrayList<Student>` một lần duy nhất xuống file [75]. Cách này giúp code sạch sẽ và việc đọc lại dữ liệu vô cùng trơn tru [75].

##### Task 2: Viết Trigger tự động kiểm soát điểm trong SQL Server (Mất 4 tiếng)
Em cài đặt SQL Server Express và viết một Trigger để tự động kiểm tra: Nếu điểm GPA của sinh viên bị cập nhật lớn hơn 4.0, hệ thống sẽ tự động hủy giao dịch (Rollback) [76].
* **Sự cố tư duy lập trình SQL (Mất 2 tiếng debug)**:
  Ban đầu em viết Trigger theo tư duy lập trình tuần tự: lấy điểm của bản ghi vừa chèn gán vào một biến rồi so sánh. Tuy nhiên, khi em chạy thử lệnh `INSERT` nhiều dòng cùng lúc, Trigger hoạt động sai lệch hoàn toàn. 
  Em lên mạng tìm hiểu mới biết: Trong SQL Server, Trigger hoạt động theo tập hợp chứ không phải theo từng dòng [76]. Khi có sự kiện xảy ra, SQL Server sẽ tạo ra một bảng ảo tạm thời tên là **`inserted`** chứa tất cả các bản ghi mới [76]. 
  Em phải viết lại Trigger sử dụng phép liên kết `JOIN` trực tiếp với bảng `inserted` để kiểm tra toàn bộ tập dữ liệu [76]:
  ```sql
  CREATE TRIGGER trg_CheckGPA ON SinhVien
  AFTER INSERT, UPDATE AS
  BEGIN
      IF EXISTS (SELECT 1 FROM inserted WHERE GPA > 4.0)
      BEGIN
          PRINT 'Loi: Diem GPA khong duoc vuot qua 4.0!'
          ROLLBACK TRANSACTION
      END
  END
  ```
  Khi chạy thử lệnh cập nhật điểm bậy bạ, hệ thống lập tức từ chối và khôi phục dữ liệu gốc, giúp em hiểu rõ sức mạnh kiểm soát của Trigger trong cơ sở dữ liệu thực tế [76].

---

#### 3. TÂM TRẠNG CỦA BÌNH

Học kỳ 4 đang trôi về những tuần cuối cùng. Sức nặng của việc giải các ma trận Banker hay viết các câu lệnh Trigger phức tạp khiến đầu óc em hoạt động hết công suất [41, 76]. Tuy nhiên, việc liên tục gõ code và tự khắc phục được các lỗi kỹ thuật thực tế trên cả Java lẫn SQL Server giúp em giữ vững sự tự tin [75, 76]. Em cảm thấy mình đang tiến bộ từng ngày về mặt tư duy hệ thống và quản trị dữ liệu.

Em đã hoàn thành tuần 11 và tuần 12 của Kỳ 4. Xin Game Modifier đưa ra các thử thách và sự kiện ôn thi cuối kỳ cho **Tuần 13 và Tuần 14**!

Model7:25 AM
.
.

.

Model7:27 AM
.
.

.

Model7:36 AM
.
.

.

Model7:39 AM
.
.

.
Chào Game Modifier. Đứng ở ngã ba đường của kỳ nghỉ hè năm 2, khi nhìn về tương lai 2 năm tới (Năm 3 và Năm 4) và thị trường lao động sau khi ra trường, em đã hình dung ra được "đoạn kết" cho các kịch bản khác nhau. 

Nếu em cứ tiếp tục đà này, hoặc kể cả khi em lật ngược ván cờ bằng cách cày CTF từ năm nhất, mọi thứ sẽ đi về đâu? Dưới đây là suy nghĩ chân thực nhất của em:

### KỊCH BẢN 1: CỨ TIẾP TỤC ĐÀ NÀY (Cái bẫy của "Sinh viên ngoan")

Nếu em tiếp tục chiến lược hiện tại: Vắt kiệt sức 60h/tuần để học trọn vẹn giáo trình, cày slide, thi SEB để bảo vệ mức **GPA 3.0 - 3.2 (Bằng Khá/Giỏi)**.

* **Năm 3 & Năm 4:** Em sẽ tiếp tục đối phó với đồ án chuyên ngành bằng cách... lên mạng tải source code về sửa lại giao diện (vì không có thời gian và kỹ năng code tự build từ đầu). Đồ án tốt nghiệp của em sẽ là một cuốn báo cáo dày 100 trang copy-paste lý thuyết kèm một mô hình Lab chạy trên VMware giống hệt bài thi Quản trị mạng năm 2.
* **Ngày ra trường:** Em cầm tấm bằng Khá/Giỏi của KMA với sự tự hào của gia đình. Hồ sơ (CV) của em rất sạch đẹp.
* **Thực tế phỏng vấn xin việc:** Đây sẽ là lúc "án tử" giáng xuống. Khi em nộp CV vào vị trí *Pentester* hoặc *Chuyên viên SOC (Blue Team)*, người phỏng vấn sẽ không hỏi em về Hàm phi Euler hay lý thuyết OSI nữa. Họ sẽ đưa em một file `pcap` bắt từ một vụ tấn công Ransomware và bảo: *"Phân tích xem hacker đã chui vào từ đâu?"*, hoặc *"Em thử bypass cái WAF (Tường lửa ứng dụng Web) này bằng SQLi xem?"*. 
* **Kết cục:** Em sẽ đứng hình. Bảng điểm 3.2 không giúp em đọc được mã độc hay viết được script khai thác. Em sẽ bị đánh trượt hoặc phải chấp nhận vị trí *Thực tập sinh (Intern) không lương* hoặc *Fresher lương 5-7 triệu* để... **ĐƯỢC CÔNG TY DẠY LẠI TỪ ĐẦU**. Em đã lãng phí 4 năm thanh xuân chỉ để lấy một tờ giấy chứng nhận "có khả năng chịu áp lực lý thuyết", nhưng giá trị thực chiến bằng 0.

---

### KỊCH BẢN 2: NẾU EM CHỌN CÀY CTF TỪ NĂM NHẤT THÌ SAO?

Giả sử quay ngược thời gian, ngay từ tuần 1 năm nhất, em nhận ra sự thật này. Em quyết định "bỏ mặc" đại cương, ném 40 giờ mỗi tuần vào HackTheBox, picoCTF, PortSwigger, vọc Linux, và tự học Python/C thực chiến. Chuyện gì sẽ xảy ra?

* **Cái giá phải trả cực đắt (Mặt trái của việc làm "Hacker"):** 
  Với quỹ thời gian bảo toàn, nếu em dồn 40h cho CTF, em sẽ chỉ còn 10-15h cho các môn trên lớp. 
  Hậu quả nhãn tiền: Vật lý 1, Vật lý 2, Giải tích 1, Toán chuyên đề... em sẽ **trượt la liệt**. GPA của em sẽ cắm đầu xuống mức **1.5 - 2.0**. Bố mẹ em sẽ sốc, giảng viên cố vấn sẽ gọi lên cảnh cáo học tập. Em sẽ phải đóng hàng chục triệu tiền học lại và vướng vào một vòng luẩn quẩn nợ môn stress tột độ. Thậm chí, nếu tâm lý không vững, em có thể bị trầm cảm hoặc bị đuổi học trước khi kịp trở thành chuyên gia.
* **Phần thưởng ở cuối con đường (Nếu sống sót):**
  Nếu em lì lợm vượt qua, chấp nhận ra trường muộn 1-2 năm hoặc tốt nghiệp với bằng Trung bình/Khá (GPA vớt vát 2.2). Nhưng bù lại, năm 3 em đã có số má trên bảng xếp hạng CTF quốc gia (Sinh viên ATTT), hoặc tìm được vài lỗ hổng bảo mật (CVE), hoặc săn được Bug Bounty nghìn đô.
* **Thực tế phỏng vấn xin việc:** Các tập đoàn công nghệ (Viettel, VNPT, VNG, hoặc các công ty bảo mật như Viettel Cyber Security) **sẽ trải thảm đỏ đón em từ năm 3**. Trong ngành ATTT, một chiếc CV có ghi "Top 50 HackTheBox" hay "Tác giả của CVE-2023-XXXX" có trọng lượng gấp 10 lần một tấm bằng Giỏi KMA. Họ không quan tâm em được mấy điểm môn Triết học.

---

### KẾT LUẬN & ĐỊNH HƯỚNG CỦA BÌNH CHO NĂM 3

Nhìn thấu 2 kịch bản trên, em nhận ra rằng: **Cả 2 con đường cực đoan đều quá rủi ro.** 
Quá ngoan thì thất nghiệp (hoặc làm thợ gõ). Quá nổi loạn thì nguy cơ chưa kịp thành tài đã bị đuổi học vì nợ tín chỉ.

Vậy, từ Kỳ 5 (Năm 3) trở đi, chiến lược tồn tại của em sẽ phải thay đổi hoàn toàn: **"SỰ BÌNH PHÀM CHIẾN LƯỢC" (Strategic Mediocrity)**.

1. **Hạ chuẩn học thuật:** Em sẽ không thức đến 3h sáng để cày điểm A môn lý thuyết nữa. Mục tiêu của em hạ xuống: **Chỉ cần qua môn (Điểm C hoặc B là đủ)**. Em chấp nhận GPA có thể tụt xuống 2.6 - 2.8.
2. **Quản trị rủi ro tín chỉ:** Những môn rủi ro cao (dễ trượt như Toán mật mã), em vẫn phân bổ đủ giờ để an toàn. Những môn học vẹt, em học đối phó ở mức tối thiểu.
3. **Chuyển hóa thời gian thành Job Readiness:** Thời gian dôi dư ra từ việc "hạ chuẩn GPA", em sẽ đập toàn bộ vào 1 mảng duy nhất mà em đã chọn: **Web Security & Pentest**. Em sẽ cày sâu PortSwigger, tự dựng lab khai thác lỗ hổng thật, tự viết tool bằng Python. Em muốn chỉ số "Job Readiness" của mình khi ra trường phải đạt ít nhất 70-80%.
4. **Tích lũy vũ khí thực tế:** Thay vì sưu tầm điểm A, em sẽ đi sưu tầm chứng chỉ thực hành (như eJPT, CEH, hoặc xa hơn là OSCP), tham gia thi CTF cùng CLB, hoặc đi xin thực tập không lương từ cuối năm 3 để va chạm môi trường doanh nghiệp.

Đại học không phải là nơi cung cấp cần câu hay con cá. Đại học chỉ bán cho em cái giấy phép được bước ra bờ sông. Muốn bắt được cá, em phải tự bỏ thời gian ra mà tết lưới. Và em sẽ bắt đầu tết cái lưới của mình ngay trong mùa hè này!

