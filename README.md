# crawling-VietNam-News
Crawl dữ liệu từ các trang tin tức ở Việt Nam

### Trang web được hỗ trợ crawl
- [VNExpress](http://vnexpress.net/)
- [Việt Nam Net](http://vietnamnet.vn/)
- [Thanh niên](http://thanhnien.vn/)
##### Danh mục : Thời sự, bạn có thể thay đổi danh mục bạn cần dựa vào đường link

# Sử dụng
   - [Cài đặt scarpy](https://docs.scrapy.org/en/latest/intro/install.html)  `pip install Scrapy`
   - Clone git `git clone git://github.com/smoothkt4951/crawling-VietNam-News.git`  
   - Chạy 2 dòng lệnh đầu tiên để cài các module cần thiết [xem Requirements.txt](Requirements.txt)

# Hướng dẫn crawling dữ liệu
Để có thể thu thập được nhiều trang tin, khi thu thập xong một trang tin tức, ta cần gửi request đến trang tin tức đó một request “next-page” để sang trang kế tiếp và tiếp tục crawl. Mình nên chọn các trang web có cấu trúc ‘next-page’ thay vì scroll xuống để xem tin mới để tiện xử lý url next sang một trang mới. Ví dụ như trang vnexpress.com sẽ có cấu trúc như sau:

 
  
         
 
                  
                  


