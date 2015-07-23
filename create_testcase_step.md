- Common item part
  - Phần thay đổi dynamic của hiển thị thì có phải đang là data giống như chỉ thị của spec hay không
  - Phần hoạt động (nếu có) thì có phải đang là data theo như chỉ thị của spec hay không
Part riêng
- Phần hiển thị
     - Có phải đang là data theo như chỉ thị của spec hay không
- Phần input
     - Có hoạt động đúng với giá trị input cơ bản (ví dụ thành công) hay không
     - Item riêng
          - Xử lý khi là số lượng ký tự tối đa thì có phù hơp với spec hay không 
          - Xử lý khi là số lượng ký tự tối thiểu thì có phù hơp với spec hay không
          - Xử lý khi là NULL thì có phù hơp với spec hay không (or error message có đúng như spec hay không)
          - Xử lý của số lượng ký tự tối đa +1 ký tự  thì error message có đúng như spec hay không
          - Xử lý của số lượng ký tự tối thiểu -1 ký tự  thì error message có đúng như spec hay không
          - Error message của xử lý khi sai format thì có đúng như spec hay không
          - Xử lý khi nhập ký tự kiểm tra XSS ?
          - Xử lý khi nhập ký tự kiểm tra SQLInjection ?
       - Multi item
          - Hiển thị khi error message bị trùng lặp thì có xuất hiện nhiều cái đúng như spec hay không
          - Khi phát sinh error số lượng tối đa thì hiển thị có bị lệch hay không
- Flow màn hình
   - Xử lý khi ấn button「Back」đúng ?
   - Xử lý khi ấn button「Next」đúng ?
   - Xử lý khi reload(F5)?  (Phương pháp xử lý đúng thì có đang được định nghĩa trong expected hay không)
   - Xử lý khi browser back? (giống như trên)
   - Xử lý khi browser back  -> forward? (giống như trên)
   - Xử lý khi browser back  -> di chuyển màn hình đúng?

- Flow xử lý song song (parallel) (Cái này hơi khác nên sẽ là item của test tổng thể) 
    - Trường hợp trong khi đang input, nếu mở cùng màn hình đó bằng tab khác và cứ để nguyên như vậy mà kết thúc xử lý bằng data khác, sau đó back lại thì sẽ như thế nào?
    - Trong khi đang input, mở bằng browser khác (giống như trên) (edited)

--
->Nếu làm như thế này thì block của testcase sẽ được phân chia đẹp mắt hơn và người tạo testcase sẽ ít để phát sinh「thiếu sót」.

->Ngoài ra, có thể tổng kết「quy trình để có thể tạo testcase」cơ bản.
