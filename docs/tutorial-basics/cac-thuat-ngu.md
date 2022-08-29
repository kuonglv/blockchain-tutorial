---
sidebar_position: 8
---

# Các thuật ngữ

Các thuật ngữ hay dùng trong công nghệ blockchain.

## 1. Fork

Fork được biết đến là một kỹ thuật sửa đổi mã nguồn mở. Thuật ngữ lập trình này thường sử dụng để chỉ các hoạt động cập nhật, nâng cấp hoặc sửa đổi phần mềm. Thông thường, một bản Fork rẽ nhánh khá tương đồng với bản gốc, khác biệt là chúng được thêm một vài sửa đổi quan trọng.

## 3 dạng chính của quá trình Fork
### Temporary Fork – Phân tách tạm thời
Khi hai người cùng khai thác được một khối mới trong cùng một thời điểm, toàn bộ mạng có thể không đạt được sự đồng thuận trong việc lựa chọn khối nào để thêm vào Blockchain. Một số thành viên trong mạng có thể không thống nhất chung ý kiến, dẫn đến việc xuất hiện cùng lúc nhiều chuỗi khối khác.

Đồng thời, Blockchain có tính chất phi tập trung và độ trễ lan truyền dữ liệu nên mất khá nhiều thời gian để thông tin có thể di chuyển đều trong toàn bộ mạng lưới. Điều này dẫn đến một số thành viên có thể nhận được phiên bản này, một số khác lại nhận được phiên bản khác, dẫn tới sự mâu thuẫn về ý kiến liên quan đến thứ tự thời gian của các sự kiện.

Trường hợp phân tách này sẽ tồn tại hai hoặc nhiều chuỗi khối có cùng độ dài. Phân tách tạm thời có thể tự giải quyết dựa trên giao thức đồng thuận của mạng lưới Blockchain. Trong các hệ thống PoS như Bitcoin, các thợ mỏ sẽ tự lựa chọn chuỗi khai thác để tiếp tục khai thác khối tiếp theo. Một thời gian sau đó, Blockchain dài nhất được xem là Blockchain ‘’đúng’’, có hiệu quả và sẽ thắng. các chuỗi ngắn hơn sẽ bị loại bỏ. Khi đó, một trong các chuỗi còn lại không được khai thác và thêm khối mới để đồng bộ. Điều này dẫn đến sự đồng thuận về trạng thái của chuỗi khối trong một thời gian ngắn, hay còn gọi là phân tách tạm thời.

### Soft Fork – Phân tách mềm
Đây là sự phân tách do những cập nhật chức năng và giao thức mới trên Blockchain nhưng sau khi thay đổi, vẫn tương thích ngược với giao thức và phiên bản cũ. Có nghĩa là các trạng thái của Blockchain vẫn được chấp nhận trong phiên bản mới. Các nút không cập nhật vẫn có thể tự do xử lý các giao dịch và đẩy khối mới vào Blockchain, miễn là chúng không phá vỡ quy tắc trong giao thức mới.

Tất cả các khối trên Blockchain Soft Fork đều tuân theo quy tắc đồng thuận đã được xây dựng ban đầu. Do đó, Soft Fork không yêu cầu các nút trên mạng phải nâng cấp để duy trì sự đồng thuận. Tuy nhiên, các khối được tạo bởi nút tuân theo bộ quy tắc đồng thuận cũ sẽ vi phạm những quy tắc mới khiến cho quá trình xác thực bị lỗi. Một số trường hợp đặc biệt, bạn vẫn có thể sử dụng những tính năng của phiên bản cũ trên phiên ban mới và ngược lại.

Trên Blockchain, nếu bạn muốn giảm kích thước khối từ 3MB xuống 2MB. Lúc này, các nút sử dụng phiên bản cũ vẫn có thể xử lý giao dịch và đẩy khối mới có dung lượng 2MB xuống. Tuy nhiên, chúng không thể xử lý và đẩy lên một khối có kích thước lớn hơn 2MB vào mạng. Các nút trong phiên bản mới sẽ từ chối vì điều này vi phạm quy tắc mới.

### Hard Fork – Phân tách cứng
Quá trình Hard Fork được sử dụng để thay đổi hoặc cải thiện một giao thức hiện có, thậm chí là tạo ra một giao thức và Blockchain mới, hoàn toàn độc lập.

Lúc này, các node chạy trên những phiên bản cũ sẽ không được chấp nhận trên những phiên bản mới nữa. Do đó, những người tham gia trong mạng bắt buộc phải nâng cấp lên phiên bản mới nhất của phần mềm để có thể xác thực các khối giao dịch mới.

Hard Fork được thực hiện vô cùng phức tạp vì chúng thường diễn ra nhiều sự mâu thuẫn, không thống nhất trong mạng lưới. Một số người dùng không muốn cập nhật, trong khi đó nhiều người lại muốn tạo ra sự thay đổi mới.

Vì thế, người muốn tham gia sẽ tự nâng cấp phần mềm của họ theo quy tắc mới, loại bỏ phiên bản cũ. Ngược lại, những người không cập nhật vẫn sẽ khai thác trên chuỗi khối cũ. Điều này đã chia rẽ và tạo thành hai Blockchain độc lập khác nhau. Chúng sẽ có một cộng đồng riêng và các nhà phát triển sẽ hoạt động theo cách mà họ tin là tốt, hiệu quả nhất. Bao gồm hai trường hợp như sau:

- Hard Fork có kế hoạch: Đây là một bản Hard Fork nâng cấp cho giao thức được lên kế hoạch sẵn đã được các nhà phát triển dự án làm rõ từ trước.
- Hard Fork cạnh tranh: Trường hợp này thường xảy ra khi có sự bất đồng nghiêm trọng giữa các bên liên quan trong dự án như: nhà phát triển, người dùng mạng và người khai thác.

## 2. Burn

Coin Burning, Token Burning, hay còn được gọi là đốt token - là một hành động tiêu hủy một lượng coin/token vĩnh viễn ra khỏi số lượng token đang được lưu hành. Thường thì chủ dự án hoặc anh em nắm giữ những đồng coin/token này sẽ tham gia vào quá trình đốt coin nếu có nguyện vọng đốt coin. Hiểu đơn giản, đốt coin sẽ khiến lượng coin/token lưu hành giảm, từ đó giá của đồng coin/token đó sẽ tăng trưởng.

Trong tài chính chuyền thống thì đốt coin giống như việc mua lại cổ phiếu của những công ty do chính họ phát hành trước đó. Việc mua lại cổ phiếu đến từ công ty sẽ làm giảm tổng số lượng cổ phiếu đang lưu hành, từ đó có tác dụng làm tăng giá trị cổ phiếu của nhà đầu tư.

Mục đích của đốt coin chính là thúc đẩy sự phát triển bền vững của toàn bộ dự án và cân bằng lợi ích giữa các bên tham gia.

### Quá trình đốt coin diễn ra thế nào?
Hiểu đơn giản, để “đốt” coin trên mạng blockchain thì chúng sẽ được gửi tới một địa chỉ ví được gọi là Dead Address. Tại địa chỉ ví này, lượng token này sẽ được giữ trong đó và không thể rút được ra.

Ví dụ trên mạng BNB Chain thì các Dead Address thường sẽ có đuôi là “dEaD”, hoặc 0x000…000 như trên mạng Ethereum. Đặc biệt, các ví dạng này sẽ được các Blockchain Explorer phân loại vào hashtag “Burn”.

### Cơ chế Buyback and Burn - Mua lại và đốt coin/token
Trong thế giới crypto, Buyback and Burn có thể hiểu đơn giản là việc mua lại token và đốt lượng token đó. Ưu điểm nổi bật nhất của cơ chế này là giúp giá token tăng trưởng bền vững về dài hạn và giúp nhà đầu tư có thêm niềm tin để hold.

Buyback and Burn làm tăng volume giao dịch và tăng thanh khoản, giúp giá token tránh có những pha biến động mạnh. Điều này cũng củng cố tính ổn định của giá token.

Nhưng câu hỏi bây giờ sẽ là: Bên nào và nguồn tiền nào sẽ mua lại coin/token để đốt?

Thông thường, các blockchain hoặc protocol sẽ trích một phần phí, lợi nhuận có được để mua lại token rồi đem đi đốt. Quá trình đốt có thể được lập trình ngay từ đầu hoặc thông qua các đề xuất được bỏ phiếu bởi cộng đồng.

### Khi nào cần đốt coin?
Bởi vì đốt coin là hành động tự phát và không bắt buộc, nên mỗi dự án crypto sẽ có một chiến lược phát triển riêng.

Đối với những dự án có tokenomics được thiết kế chưa hợp lý khiến token chịu một áp lực đến từ lạm phát tăng cao thì có thể dùng cách đốt coin để giảm phát. Một trong những mục đích chính của đốt coin là cân bằng lợi ích giữa các bên khi họ giữ coin/token.

Ngược lại, có những dự án mới ra mắt token và chỉ có rất ít holder mà đã có cơ chế đốt coin riêng với mục đích để quảng bá. Khả năng rất cao dự án sẽ khó để đạt được thành công, vì đơn giản ở giai đoạn đầu thì việc đốt token gần như là vô nghĩa. Cách hợp lý nhất sẽ là khóa token với một khoảng thời gian trả dần để thị trường thích ứng cũng như có nhiều incentive hơn để phát triển.

### Thách thức của đốt coin
**Cân bằng tokenomics**
Giá của crypto theo lý thuyết cung cầu: khi nguồn cung giảm mà cầu giữ nguyên thì giá sẽ chỉ có tăng.

- Nhà đầu tư thấy giá tăng liên tục thì sẽ dần dần hạn chế mua vào, khiến khối lượng giao dịch bị giảm.
- Ngược lại, nếu token được tạo ra trong một thời gian dài thì nhà đầu tư cũng sẽ hạn chế mua vào để tránh việc khoản đầu tư của họ tiếp tục thua lỗ.
Vậy nên, tìm điểm cân bằng giữa lạm phát và giảm phát của token trong thiết kế tokenomics sẽ là một thách thức lớn cho những builder tâm huyết.

Tham khảo thêm [https://coin98.net/dot-coin-la-gi](https://coin98.net/dot-coin-la-gi)

## 3. Halving
**Block halving (chia đôi khối) là gì?**
Chia đôi khối là quá trình giảm tốc độ tạo ra các đơn vị tiền mã hóa mới. Cụ thể, thuật ngữ này nhắc đến quy trình giảm một nửa số phần thưởng cho các thợ đào khi họ khai thác được một khối bitcoin mới, được diễn ra định kỳ.

**Quy trình Bitcoin Block Halving hoạt động như thế nào?**
Bitcoin Halving là một hàm thiết yếu của giao thức bitcoin. Mã này có thể tìm được trên Bitcoin Core Github, dưới đây là một phần của đoạn mã để tạo nên quy trình bitcoin halving. Như được ghi trong đoạn mã, cứ sau mỗi 210.000 khối được tạo ra, thì phần thưởng cho mỗi khối mới sẽ được giảm một nửa.

### Tại sao Bitcoin lại xảy ra Halving?
Một số mục đích khiến cho Bitcoin phải Halving như sau:

- Ngăn chặn lạm phát
- Gia tăng giá trị của Bitcoin
- Tạo thời gian để ngành công nghiệp tiền điện tử trưởng thành

Tham khảo thêm [https://cryptoviet.com/bitcoin-halving-la-gi](https://cryptoviet.com/bitcoin-halving-la-gi)

## 4. Staking
Trước khi hiểu về staking bạn cần tìm hiểu về thuật toán đồng thuận cổ phần PoS – Proof of Stake trước.

PoS là một thuật toán đồng thuận tương đối mới mẻ đối với một số loại tiền kỹ thuật số. Cơ chế này tạo ra các khối mới được thêm vào blockchain. Các khối này được đặt bởi những người nắm giữ một số lượng đồng tiền điện tử để giúp xác thực một giao dịch mới trên nền tảng. Những người tham gia PoS sẽ được nhận phần thưởng (gồm phần thưởng khối và phí giao dịch) để làm động lực cho các đóng góp của họ.

Như vậy, Staking là việc lưu trữ 1 số lượng đồng tiền kỹ thuật số nhất định trong ví của 1 dự án Blockchain trong 1 khoảng thời gian cụ thể để nhận được phần thưởng. Số lượng phần thưởng phụ thuộc vào sự đầu tư ban đầu của bạn, bao gồm: Số lượng coin stake, thời lượng stake.

Điều này tương tự như cách bạn gửi tiền tiết kiệm trong tài khoản ngân hàng để rút lãi khi đến kỳ hạn.

**Staking được phân thành 2 loại hình như sau:**
- Staking với cơ chế đồng thuận PoS: Như khái niệm bạn đã được biết ở trên, bạn dùng 1 số lượng tiền điện tử nhất định để staking và nhận lại phần thưởng cho hoạt động xác minh giao dịch. Dạng staking này được thực hiện và tác động trực tiếp đến mạng lưới Blockchain.
- Staking bằng cách ủy thác: Bạn gửi lại đồng coin vào ví của nhóm phát triển dự án (không phải Blockchain riêng) và nhận lợi nhuận định kỳ. Dạng Staking này không trực tiếp tham gia vào việc xác thực các giao dịch hay bất cứ nhiệm vụ gì liên quan tới các hoạt động trong mạng lưới nhưng nó vẫn được gọi là staking. Nó không khác gì đầu tư ủy thác.

Tham khảo thêm [https://cryptoviet.com/staking-la-gi](https://cryptoviet.com/staking-la-gi)

## 5. Hash (hàm băm)
Hash (hàm băm) là một trong những phần quan trọng nhất của thứ công nghệ giúp giữ an toàn cho mạng lưới Bitcoin.

Về cơ bản hashing là quá trình biến một dữ liệu đầu vào có độ dài bất kỳ thành một chuỗi đầu ra đặc trưng có độ dài cố định. Hashing được thực hiện thông qua hàm băm (hash function).

Một cách tổng quát hàm băm là bất kỳ hàm nào có thể được sử dụng để ánh xạ dữ liệu có kích thước tùy ý thành các giá trị kích thước cố định. Các giá trị được trả về bởi hàm băm được gọi là giá trị băm, mã băm, thông điệp băm, hoặc đơn giản là “hash”.

Ví dụ, khi bạn download một video trên YouTube có dung lượng 50 MB và thực hiện hashing trên nó bằng thuật toán băm SHA-256, thì đầu ra bạn thu được sẽ là một giá trị băm có độ dài 256 bit. Tương tự, nếu bạn lấy một tin nhắn văn bản có dung lượng 5 KB, để hashing bằng SHA-256 thì giá trị băm đầu ra bạn thu được vẫn sẽ là 256 bit.

Như bạn có thể thấy, trong trường hợp SHA-256, cho dù đầu vào của bạn lớn hay nhỏ như thế nào đi chăng nữa, thì đầu ra bạn nhận được sẽ luôn có độ dài 256 bit cố định. Điều này trở nên quan trọng khi bạn xử lý một lượng lớn dữ liệu và giao dịch. Khi đó, thay vì bạn phải xử lý toàn bộ lượng dữ liệu đầu vào (có thể có kích thước rất lớn), bạn chỉ cần xử lý và theo dõi một lượng dữ liệu rất nhỏ là các giá trị băm.

Trong blockchain, các giao dịch có độ dài khác nhau sẽ được băm thông qua một thuật toán băm nhất định và tất cả đều cho đầu ra có độ dài cố định bất kể độ dài của giao dịch đầu vào là bao nhiêu. Chẳng hạn, Bitcoin sử dụng thuật toán SHA-256 để băm các giao dịch cho kết quả đầu ra có độ dài cố định là 256 bit (32 byte) cho dù giao dịch chỉ là một từ hoặc giao dịch phức tạp với lượng dữ liệu khổng lồ. Điều làm cho việc theo dõi các giao dịch trở nên dễ dàng hơn khi truy xuất và theo dõi lại các giá trị băm. Kích thước của hàm băm sẽ phụ thuộc vào hàm băm được sử dụng.

Kỹ thuật hashing thường được sử dụng và có ứng dụng rộng rãi nhất trong việc đảm bảo tính toàn vẹn cho dữ liệu trong blockchain là các hàm băm mật mã (cryptographic hash function) chẳng hạn như SHA-1. SHA-2. SHA-3, SHA-256…Sỡ dĩ như vậy là do các hàm băm mật mã có một số tính chất quan trọng phù hợp cho việc đảm bảo an toàn dữ liệu.

Xem thêm về hàm băm [https://cryptoviet.com/hash-la-gi](https://cryptoviet.com/hash-la-gi)