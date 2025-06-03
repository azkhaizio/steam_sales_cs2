Phân tích dữ liệu người chơi steam, EDA, xây dựng predictive model cơ bản (dự đoán khả năng tài khoản có chơi cs2 hay không) dựa trên dataset kaggle có sẵn.

Original dataset : https://www.kaggle.com/datasets/artyomkruglov/gaming-profiles-2025-steam-playstation-xbox/data. Dữ liệu này chỉ là một phần nhỏ so với dữ liệu thực tế, đồng thời phân tích trong đây giả định rằng tất cả những cột library bị trống ( dù là tại tài khoản để chế độ riêng tư hoặc dữ liệu bị thiếu hoặc thực sự không có) đều sẽ được quy là không chơi gì. Vì vậy dữ liệu này sẽ khác so với dữ liệu thực tế.  

Giải thích các column:
-playerid : ID của các player trong danh sách  
-country : Quốc gia của tài khoản steam  
-created : Ngày thành lập tài khoản steam  
-library	: Danh sách các game có trong thư viện của tài khoản  
-friends : Danh sách bạn bè của tài khoản  
-year_created : Được trích từ "created", năm thành lập  
-play_cs2 : Giá trị Binary, 0 tức là không chơi cs2, 1 là có chơi cs2  
-total_friends : Tổng số bạn bè trong tài khoản  
-total_games : Tổng số game trong tài khoản  
