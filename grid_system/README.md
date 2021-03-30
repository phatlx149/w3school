# Grid Object

Class "_grid_" giúp chúng ta chứa nội dung chính hoặc các thành phần chính trên layout website.

**Grid** được tạo dựng linh động, có thể sử dụng cho trường hợp (full-width) với class "**_grid_**" (tượng tự class "container-fluid" trong bootstrap). Và khi muốn sử dụng _1200px_ Grid system _12 columns_ các bạn có thể sử dụng 2 class là "**_grid wide_**" (tương tự như class "container" trong bootstrap).

**Grid** tự động thay đổi chiều rộng trên các thiết bị khác nhau. Để đơn giản hóa việc tạo responsive layout với grid system - ở đây, mình sẽ handle việc tự động thay đổi chiều rộng của "grid" với 3 breakpoints.

# Row Object

**Row** nghĩa là hàng, được sử dụng để chứa các _Columns_. **Row** giúp định hướng các _Columns_ theo chiều ngang. **Row** sử dụng `margin` với giá trị âm sang 2 phía trái/phải để "bù trừ" cho khoảng `padding` trái/phải của _Columns_ (Column `padding` trái/phải để tạo ra rãnh ngăn - hay còn gọi là _gutters_).

# Column Object

- Chứa các thành phần trên website

- Các bạn chú ý:
  Hãy thêm `box-sizing: border-box;` vào trang web của bạn. Ví dụ:

  `<style> * { box-sizing: border-box; } </style>`

  Nếu thiếu thuộc tính trên thì các _column_ của bạn có thể không nằm trên một chiều ngang.

- **Column** là gì?

  **Column** nghĩa là cột, được sử dụng để chứa nội dung/thành phần hiển thị trên website của bạn. **Column** sử dụng padding trái/phải để tạo nên gutters - rãnh ngăn cách giữa các **column** trong Grid layout. **Column** luôn luôn là con trực tiếp của Row.

  **Column** được sử dụng với class "col", đi kèm theo đó là một số class "c-\*" "m-\_" và "l-\*":

  - c-\*: nghĩa là **column**, prefix class này có tác dụng trên mobile. \_ từ 0 tới 12. Trong đó 0 được sử dụng để ẩn **column**, 1 - 12 tương ứng với độ rộng chúng ta muốn sử dụng cho **column** (trên cơ sở 12 columns trong Grid system)
  - m-\*: nghĩa là medium, prefix class này có tác dụng trên Tablet.
  - l-\*: nghĩa là large, prefix class này có tác dụng trên PC.

# Version 2

- Thêm tính năng column offset

# Version 3

- Thêm tính năng no-gutter
