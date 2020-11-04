
Trong bài viết này tôi sẽ trình bày với các bạn chi tiết về định nghĩa, các dạng tấn công DoS và DDoS, cùng hàng loạt các kiến thức liên quan được tổng hợp. DoS và DDoS là một trong những dạng tấn công nguy hiểm nhất đối với một hệ thống mạng. Bài viết này tôi không muốn các bạn dựa vào các tools trong này để tấn công, mục đích trình bày để các bạn hiểu về kiểu tấn công này, và có những giải pháp phòng chống.

Phần I: của bài viết tập trung vào DoS

Phần II của bài viết về định nghĩa, các tools và cách phòng chống DDoS

1. Lịch sử các cuộc tấn công DoS và DDoS

2. Định nghĩa về: Denial of Service Attack

3. Các dạng tấn công DoS

4. Các tool tấn công DoS

5. Mạng BOT net

6. Tấn công DDoS

7. Phân loại tấn công DDoS

8. Các tools tấn công DDoS

9. Sâu máy tính (worms) trong tấn công DDoS

**I. Lịch sử của tấn công DoS**

**1. Mục tiêu**

- Mục tiêu các cuộc tấn công thường vào các trang web lớn và các tổ chức thương mại điện tử trên Internet.

**2. Các cuộc tấn công.**

- Vào ngày 15 tháng 8 năm 2003, Microsoft đã chịu đợt tấn công DoS cực mạnh và làm gián đoạn websites trong vòng 2 giờ.

- Vào lúc 15:09 giờ GMT ngày 27 tháng 3 năm 2003: toàn bộ phiên bản tiếng anh của website Al-Jazeera bị tấn công làm gián đoạn trong nhiều giờ

**II. Định nghĩa về tấn công DoS**

Tấn công DoS là kiểu tấn công vô cùng nguy hiểm, để hiểu được nó ta cần phải lắm rõ định nghĩa của tấn công DoS và các dạng tấn công DoS.

- Tấn công DoS là một kiểu tấn công mà một người làm cho một hệ thống không thể sử dụng, hoặc làm cho hệ thống đó chậm đi một cách đáng kể với người dùng bình thường, bằng cách làm quá tải tài nguyên của hệ thống.

- Nếu kẻ tấn công không có khả năng thâm nhập được vào hệ thống, thì chúng cố gắng tìm cách làm cho hệ thống đó sụp đổ và không có khả năng phục vụ người dùng bình thường đó là tấn công Denial of Service (DoS).

Mặc dù tấn công DoS không có khả năng truy cập vào dữ liệu thực của hệ thống nhưng nó có thể làm gián đoạn các dịch vụ mà hệ thống đó cung cấp. Như định nghĩa trên DoS khi tấn công vào một hệ thống sẽ khai thác những cái yếu nhất của hệ thống để tấn công, những mục đích của tấn công DoS:

**1. Các mục đích của tấn công DoS**

- Cố gắng chiếm băng thông mạng và làm hệ thống mạng bị ngập (flood), khi đó hệ thống mạng sẽ không có khả năng đáp ứng những dịch vụ khác cho người dùng bình thường.

- Cố gắng làm ngắt kết nối giữa hai máy, và ngăn chặn quá trình truy cập vào dịch vụ.

- Cố gắng ngăn chặn những người dùng cụ thể vào một dịch vụ nào đó

- Cố gắng ngăn chặn các dịch vụ không cho người khác có khả năng truy cập vào.

- Khi tấn công DoS xảy ra người dùng có cảm giác khi truy cập vào dịch vụ đó như bị:

+ Disable Network - Tắt mạng

+ Disable Organization - Tổ chức không hoạt động

+ Financial Loss – Tài chính bị mất

**2. Mục tiêu mà kẻ tấn công thường sử dụng tấn công DoS**

Như chúng ta biết ở bên trên tấn công DoS xảy ra khi kẻ tấn công sử dụng hết tài nguyên của hệ thống và hệ thống không thể đáp ứng cho người dùng bình thường được vậy các tài nguyên chúng thường sử dụng để tấn công là gì:

- Tạo ra sự khan hiếm, những giới hạn và không đổi mới tài nguyên

- Băng thông của hệ thống mạng (Network Bandwidth), bộ nhớ, ổ đĩa, và CPU Time hay cấu trúc dữ liệu đều là mục tiêu của tấn công DoS.

- Tấn công vào hệ thống khác phục vụ cho mạng máy tính như: hệ thống điều hoà, hệ thống điện, hệt hống làm mát và nhiều tài nguyên khác của doanh nghiệp. Bạn thử tưởng tượng khi nguồn điện vào máy chủ web bị ngắt thì người dùng có thể truy cập vào máy chủ đó không.

- Phá hoại hoặc thay đổi các thông tin cấu hình.

- Phá hoại tầng vật lý hoặc các thiết bị mạng như nguồn điện, điều hoà…

**III. Các dạng tấn công**

Tấn công Denial of Service chia ra làm hai loại tấn công

- Tấn công DoS: Tấn công từ một cá thể, hay tập hợp các cá thể.

- Tấn công DDoS: Đây là sự tấn công từ một mạng máy tính được thiết kế để tấn công tới một đích cụ thể nào đó.

**1. Các dạng tấn công DoS**

- Smurf

- Buffer Overflow Attack

- Ping of Death

- Teardrop

- SYN Attack

**a. Tấn công Smurf**

- Là thủ phạm sinh ra cực nhiều giao tiếp ICMP (ping) tới địa chỉ Broadcast của nhiều mạng với địa chỉ nguồn là mục tiêu cần tấn công.

* Chúng ta cần lưu ý là: Khi ping tới một địa chỉ là quá trình hai chiều – Khi máy A ping tới máy B máy B reply lại hoàn tất quá trình. Khi tôi ping tới địa chỉ Broadcast của mạng nào đó thì toàn bộ các máy tính trong mạng đó sẽ Reply lại tôi. Nhưng giờ tôi thay đổi địa chỉ nguồn, thay địa chỉ nguồn là máy C và tôi ping tới địa chỉ Broadcast của một mạng nào đó, thì toàn bộ các máy tính trong mạng đó sẽ reply lại vào máy C chứ không phải tôi và đó là tấn công Smurf.

- Kết quả đích tấn công sẽ phải chịu nhận một đợt Reply gói ICMP cực lớn và làm cho mạng bị dớt hoặc bị chậm lại không có khả năng đáp ứng các dịch vụ khác.

- Quá trình này được khuyếch đại khi có luồng ping reply từ một mạng được kết nối với nhau (mạng BOT).

- tấn công Fraggle, chúng sử dụng UDP echo và tương tự như tấn công Smurf.

[![](https://megacode.vn/media/files/2014_05/2014_05_27/vne001531.jpg)](https://megacode.vn/media/files/2014_05/2014_05_27/vne001531.jpg)

Hình hiển thị tấn công DoS - dạng tấn công Smurf sử dụng gói ICMP làm ngập các giao tiếp khác.

**b. Tấn công Buffer overflow.**

- Buffer Overflow xảy ra tại bất kỳ thời điểm nào có chương trình ghi lượng thông tin lớn hơn dung lượng của bộ nhớ đệm trong bộ nhớ.

- Kẻ tấn công có thể ghi đè lên dữ liệu và điều khiển chạy các chương trình và đánh cắp quyền điều khiển của một số chương trình nhằm thực thi các đoạn mã nguy hiểm. - Tấn công Buffer Overflow tôi đã trình bày cách khai thác lỗi này trong bài viết trước về hacking windows cũng trên trang www.vnexperts.net.

- Quá trình gửi một bức thư điện tử mà file đính kèm dài quá 256 ký tự có thể sẽ xảy ra quá trình tràn bộ nhớ đệm.

**c. Tấn công Ping of Death**

![](http://megacode.vn/media/files/2014_05/vne001532.jpg)

- Kẻ tấn công gửi những gói tin IP lớn hơn số lương bytes cho phép của tin IP là 65.536 bytes.

- Quá trình chia nhỏ gói tin IP thành những phần nhỏ được thực hiện ở layer II.

- Quá trình chia nhỏ có thể thực hiện với gói IP lớn hơn 65.536 bytes. Nhưng hệ điều hành không thể nhận biết được độ lớn của gói tin này và sẽ bị khởi động lại, hay đơn giản là sẽ bị gián đoạn giao tiếp.

- Để nhận biết kẻ tấn công gửi gói tin lớn hơn gói tin cho phép thì tương đối dễ dàng.

**d. Tấn công Teardrop**

- Gói tin IP rất lớn khi đến Router sẽ bị chia nhỏ làm nhiều phần nhỏ.

- Kẻ tấn công sử dụng sử dụng gói IP với các thông số rất khó hiểu để chia ra các phần nhỏ (fragment).

- Nếu hệ điều hành nhận được các gói tin đã được chia nhỏ và không hiểu được, hệ thống cố gắng build lại gói tin và điều đó chiếm một phần tài nguyên hệ thống, nếu quá trình đó liên tục xảy ra hệ thống không còn tài nguyên cho các ứng dụng khác, phục vụ các user khác.

**e. Tấn công SYN**

![](http://megacode.vn/media/files/2014_05/vne001533.jpg)

- Kẻ tấn công gửi các yêu cầu (request ảo) TCP SYN tới máy chủ bị tấn công. Để xử lý lượng gói tin SYN này hệ thống cần tốn một lượng bộ nhớ cho kết nối.

- Khi có rất nhiều gói SYN ảo tới máy chủ và chiếm hết các yêu cầu xử lý của máy chủ. Một người dùng bình thường kết nối tới máy chủ ban đầu thực hiện Request TCP SYN và lúc này máy chủ không còn khả năng đáp lại - kết nối không được thực hiện.

- Đây là kiểu tấn công mà kẻ tấn công lợi dụng quá trình giao tiếp của TCP theo – Three-way.

- Các đoạn mã nguy hiểm có khả năng sinh ra một số lượng cực lớn các gói TCP SYN tới máy chủ bị tấn công, địa chỉ IP nguồn của gói tin đã bị thay đổi và đó chính là tấn công DoS.

- Hình bên trên thể hiện các giao tiếp bình thường với máy chủ và bên dưới thế hiện khi máy chủ bị tấn công gói SYN đến sẽ rất nhiều trong khi đó khả năng trả lời của máy chủ lại có hạn và khi đó máy chủ sẽ từ chối các truy cập hợp pháp.

- Quá trình TCP Three-way handshake được thực hiện: Khi máy A muốn giao tiếp với máy B. (1) máy A bắn ra một gói TCP SYN tới máy B – (2) máy B khi nhận được gói SYN từ A sẽ gửi lại máy A gói ACK đồng ý kết nối – (3) máy A gửi lại máy B gói ACK và bắt đầu các giao tiếp dữ liệu.

- Máy A và máy B sẽ dữ kết nối ít nhất là 75 giây, sau đó lại thực hiện một quá trình TCP Three-way handshake lần nữa để thực hiện phiên kết nối tiếp theo để trao đổi dữ liệu.

- Thật không may kẻ tấn công đã lợi dụng kẽ hở này để thực hiện hành vi tấn công nhằm sử dụng hết tài nguyên của hệ thống bằng cách giảm thời gian yêu cầu Three-way handshake xuống rất nhỏ và không gửi lại gói ACK, cứ bắn gói SYN ra liên tục trong một thời gian nhất định và không bao giờ trả lời lại gói SYN&ACK từ máy bị tấn công.

- Với nguyên tắc chỉ chấp nhận gói SYN từ một máy tới hệ thống sau mỗi 75 giây nếu địa chỉ IP nào vi phạm sẽ chuyển vào Rule deny access sẽ ngăn cản tấn công này.

**IV. Các công cụ tấn công DoS**

- Jolt2

- Bubonic.c

- Land and LaTierra

- Targa

- Blast20

- Nemesy

- Panther2

- Crazy Pinger

- Some Trouble

- UDP Flood

- FSMax

**1. Tools DoS – Jolt2**

![](http://megacode.vn/media/files/2014_05/vne001534.jpg)

- Cho phép kẻ tấn từ chối dịch vụ (DoS) lên các hệ thống trên nền tảng Windows

- Nó là nguyên nhân khiên máy chủ bị tấn công có CPU luôn hoạt động ở mức độ 100%, CPU không thể xử lý các dịch vụ khác.

- Không phải trên nền tảng Windows như Cisco Router và một số loại Router khác cũng có thể bị lỗ hổng bảo mật này và bị tools này tấn công.

**2. Tools DoS: Bubonic.c**

- Bubonic.c là một tools DoS dựa vào các lỗ hổng bảo mật trên Windows 2000

- Nó hoạt động bằng cách ngẫu nhiên gửi các gói tin TCP với các thiết lập ngẫu nhiên làm cho máy chủ tốn rất nhiều tài nguyên để xử lý vấn đề này, và từ đó sẽ xuất hiện những lỗ hổng bảo mật.

- Sử dụng bubonic.c bằng cách gõ câu lệnh: bubonic 12.23.23.2 10.0.0.1 100

![](http://megacode.vn/media/files/2014_05/vne001535.jpg)

**3. Tools DoS: Land and LaTierra**

- Giả mạo địa chỉ IP được kết hợp với quá trình mở các kết nối giữa hai máy tính.

- Cả hai địa chỉ IP, địa chỉ nguồn (source) và địa chỉ IP đích, được chỉnh sửa thành một địa chỉ của IP đích khi đó kết nối giữa máy A và máy B đang được thực hiện nếu có tấn công này xảy ra thì kết nối giữa hai máy A và B sẽ bị ngắt kết nối.

- Kết quả này do địa chỉ IP nguồn và địa chỉ IP đích của gói tin giống nhau và gói tin không thể đi đến đích cần đến.

**4. Tools DoS: Targa**

- Targa là một chương chình có thể sử dụng 8 dạng tấn công DoS khác nhau.

- Nó được coi như một bộ hướng dẫn tích hợp toàn bộ các ảnh hưởng của DoS và thường là các phiên bản của Rootkit.

- Kẻ tấn công sử dụng một trong các phương thức tấn công cụ thể tới một hệ thống bao giờ đạt được mục đích thì thôi.

- Targa là một chương trình đầy sức mạnh và nó có khả năng tạo ra một sự nguy hiểm rất lớn cho hệ thống mạng của một công ty.

**5. Tools DoS Blast 2.0**

- Blast rất nhỏ, là một công cụ dùng để kiểm tra khả năng của dịch vụ TCP nó có khả năng tạo ra một lưu lượng rất lớn gói TCP và có thể sẽ gay nguy hiểm cho một hệ thống mạng với các server yếu.

- Dưới đây là cách sử dụng để tấn công HTTP Server sử dụng Blast2.0

+ Blast 192.168.1.219 80 40 50 /b "GET /some" /e "url/ HTTP/1.0" /nr /dr /v

- Tấn công máy chủ POP

+ Blast 192.168.1.219 110 15 20 /b "user te" /e "d" /v

**6. Tools DoS – Nemesys**

![](http://megacode.vn/media/files/2014_05/vne001536.jpg)

- Đây là một chương trình sinh ra những gói tin ngẫu nhiên như (protocol, port, etc. size, …)

- Dựa vào chương trình này kẻ tấn công có thể chạy các đoạn mã nguy hiểm vào máy tính không được bảo mật.

**7. Tool DoS – Panther2.**

![](http://megacode.vn/media/files/2014_05/vne001537.jpg)

- Tấn công từ chối dịch vụ dựa trên nền tảng UDP Attack được thiết kế dành riêng cho kết nối 28.8 – 56 Kbps.

- Nó có khả năng chiếm toàn bộ băng thông của kết nối này.

- Nó có khả năng chiếm băng thông mạng bằng nhiều phương pháp ví như thực hiện quá trình Ping cực nhanh và có thể gây ra tấn công DoS

**8. Tool DoS – Crazy Pinger**

- Công cụ này có khả năng gửi những gói ICPM lớn tới một hệ thống mạng từ xa.

![](http://megacode.vn/media/files/2014_05/vne001538.jpg)

**9. Tool DoS – Some Trouble**

![](http://megacode.vn/media/files/2014_05/vne001539.jpg)

- SomeTrouble 1.0 là một chương trình gây nghẽn hệ thống mạng

- SomeTrouble là một chương trình rất đơn giản với ba thành phần

+ Mail Bomb (tự có khả năng Resole Name với địa chỉ mail có)

+ ICQ Bomb

+ Net Send Flood

**10. DoS Tools – UDP Flood**

![](http://megacode.vn/media/files/2014_05/vne001540.jpg)

- UDPFlood là một chương trình gửi các gói tin UDP

- Nó gửi ra ngoài những gói tin UDP tới một địac hỉ IP và port không cố định

- Gói tin có khả năng là một đoạn mã văn bản hay một số lượng dữ liệu được sinh ngẫu nhiên hay từ một file.

- Được sử dụng để kiểm tra khả năng đáp ững của Server

**11. Tools DoS – FSMAX**

![](http://megacode.vn/media/files/2014_05/vne001541.jpg)

- Kiểm tra hiệu năng đáp ứng của máy chủ.

- Nó tạo ra một file sau đó chạy trên Server nhiều lần lặp đi lặp lại một lúc.

- Tác dụng của tools này là tìm cách tấn công làm chàn bộ nhớ đệm và tấn công DoS tới máy chủ.

**V. Kết luận phần I.**

- Khi sử dụng một Tool tấn công DoS tới một máy chủ đôi khi không gây ảnh hưởng gì cho máy chủ - Giả sử bạn sử dụng tool Ping of Death tới một máy chủ, trong đó máy chủ kết nối với mạng tốc độ 100Mbps bạn kết nối tới máy chủ tốc độ 3Mbps - Vậy tấn công của bạn không có ý nghĩa gì.

- Nhưng bạn hãy tưởng tượng có 1000 người như bạn cùng một lúc tấn công vào máy chủ kia khi đó toàn bộ băng thông của 1000 người cộng lại tối đa đạt 3Gbps và tốc độ kết nối của máy chủ là 100 Mbps vậy kết quả sẽ ra sao các bạn có khả năng tưởng tượng.

- Trong phần II của loạt bài viết tôi sẽ trình bày với các bạn những nội dung về định nghĩa BOT, BOTNET, cách xây dựng, cách sử dụng các BOTNET từ đó chúng ta hiểu cách hoạt động và tìm ra những giải pháp để chống tấn công DDoS một cách hiệu quả nhất.
