ĐÂY LÀ FILE CSS DÙNG RIÊNG CHO RESPONSIVE WEB VỚI GRID SYSTEM

NOTE

- div có các class "grid wide" và 2 class này có chứa thuộc tính width và max-width
nên tuỳ vào chiều rộng của màn hình thì nó sẽ ưu tiên thằng nào nhỏ hơn

- Column : .col
+, Prefix class
    s - mobile
    m - tablet
    l - PC
CSS cho thiết bị nào thì dùng prefix cho thiết bị đấy

+, Prefix offset
    s-o
    m-o
    l-o
Có tác dụng điều chỉnh linh động vị trí của các item trên thiết bị tương ứng theo ứng dụng của 12 col
VD : l-o-4 là tính từ cột số 4 trở đi thì sẽ hiện

VD: xem lại vài lần là hiểu. Như khúc đầu căn giữa cái l-6 thì cái grid tổng là 3 6 3 = 12 cột. Để thằng l-6 nằm giữa thì điểm offset là sau 3 nên có kết quả là l-o-3.
Còn để hai thằng column 1 sang phải thì grid tổng là 3 3 3 3 = 12 cột. Hai thằng column 1 nằm bên phải thì nó chiếm mất hai con 3 cuối. Ép nó sang phải thì điểm offset nằm sau con 3 thứ hai là 1 2 3 4 5 6 sau số 6, thì điểm offset là l-o-6
Chia cái grid thành 12 cột ( từ 1 đến 12, dựa vào 12 cột này để chọn điểm offset ) và xem từ từ là hiểu.
- nên css lần lượt từng thiết bị để tránh bị nhầm lẫn
- class no-gutter để xóa gutter giữa các column

MADE BY :  Thắng Ngô
INSPIRE BY : F8