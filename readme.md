### Bài tập nhóm cuối kỳ
---
**Môn Xử Lý Đa Chiều**

Chủ đề: Kernel Methods (Nhóm)

**Nội dung**
    ![Alt text](image-5.png)

Kernel methods là một lớp các thuật toán được sử dụng để phân tích mẫu, phân loại trong máy
học, phương pháp phổ biến nhất của lớp thuật toán này là Support Vector Machines (SVMs). Kernel
methods liên quan đến việc sử dụng các phân loại tuyến tính (linear classifiers) để giải quyết các vấn đề phi tuyến (nonlinear problems) bằng cách sử dụng một hàm toán học gọi là kernel function để chuyển dữ liệu đầu vào sang một không gian khác có số chiều cao hơn.

Kernel methods là một công cụ mạnh vì nó có thể tìm hiểu các mối quan hệ phức tạp giữa các features. Ngoài ra, nó có thể xử lý dữ liệu nhiều chiều một cách hiệu quả mà thường yêu cầu ít tài nguyên tính toán hơn so với các kỹ thuật máy học khác. Một số ví dụ của kernel methods như SVMs, Gaussian Processes, kernel PCA,...

![Alt text](image.png)
    
Với khả năng làm mịn 

![Alt text](image-6.png)

Nhận xét: Ta thấy các vùng có cường độ thấp (các vùng mịn) sẽ xuất hiện tối hơn, trong khi các vùng có cường độ cao (các cạnh hoặc vùng chi tiết) sẽ xuất hiện sáng hơn.

![Alt text](image-7.png)

Nhận xét: Ta có thể quan sát cách mà the kernel trick cho phép SVM tìm ranh giới quyết định phi tuyến tính trong không gian đối tượng, phân tách hiệu quả các lớp trong data ban đầu.

Các phương Kmeans, Greedy , Spectral trong không gian kernel RKHS

![Alt text](image-8.png)

- kernel Greedy Kmeans
    - Kết quả phân cụm không tốt. Tuy nhiên thời gian chạy ngắn
Kernel Greedy rút ngắn thời gian nhưng sẽ không hiệu quả trong 1 số trường hợp 

- Kernel Kmeans 
    - Kết quả phân cụm tốt. Tuy nhiên thời gian chạy dài hơn 

- Kernel Spectral 
    - Kết quả phân cụm tốt. Tuy nhiên thời gian chạy ngắn hơn kernel kmeans.
    
    - => Phương pháp Kernel Spectral có độ phức tạp cao hơn , điều này có nghĩa thời gian chạy lâu hơn. Trong 1 số trường hợp. Kernel Spectral có thời gian thực hiện ngắn hơn 

- Giảm chiều giữa Kernel PCA và Kernel CCA

    - PCA và CCA tuy đề có thể giảm chiều dữ liệu.
Tuy nhiên mục đích của 2 phương pháp là khác nhau.
Điều đó dẫn đến việc giảm chiều cho ra kết quả khác nhau

    - Dùng Kmeans cho dữ liệu đã kernel CCA
    ![Alt text](image-9.png)

    - CCA có thể được dùng để tìm mối quan hệ các tập dữ liệu với nhau
Và có thể kết hợp với các phương pháp khác để phân cụm, dự đoán ,....