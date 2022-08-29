---
sidebar_position: 2
---

# Cơ chế đồng thuận

Tìm hiểu về cơ chế đồng thuận (Consensus Mechanism)? Các cơ chế đồng thuận phổ biến?

Công nghệ chuỗi khối cũng đã góp phần quan trọng xây dựng nền kinh tế số và được dự đoán sẽ dẫn dắt công nghệ tương lai. Cơ chế đồng thuận có ý nghĩa quan trọng đối với công nghệ chuỗi khối.

Thuật toán đồng thuận là một cơ chế cho phép người dùng hoặc máy móc phối hợp hoạt động trong một thiết lập phi tập trung. Nó đảm bảo rằng tất cả các tác nhân trong hệ thống có thể đồng ý về một sự thật duy nhất, ngay cả khi một số tác nhân trong hệ thống thất bại. Nói cách khác, hệ thống phải có khả năng chịu lỗi.

Trong một thiết lập tập trung, chỉ có một thực thể duy nhất có quyền đối với hệ thống. Trong hầu hết các trường hợp, thực thể này có thể thực hiện các thay đổi khi họ muốn – không có một hệ thống quản trị phức tạp nào để đạt được sự đồng thuận giữa nhiều quản trị viên. 

Nhưng trong một thiết lập phi tập trung, đó là một câu chuyện hoàn toàn khác. Giả sử chúng ta đang làm việc với cơ sở dữ liệu phân tán – làm cách nào để chúng ta đạt được thỏa thuận về những mục được thêm vào?

Giải quyết được bài toán đồng thuận giữa những người xa lạ, không cần tin tưởng nhau là một trong những ưu điểm lớn nhất của blockchain. Trong bài viết này, chúng ta sẽ tìm hiểu các thuật toán đồng thuận quan trọng như thế nào đối với hoạt động của tiền mã hóa và sổ cái phân tán.

## Thuật toán đồng thuận và tiền mã hóa

Với tiền mã hóa, số dư của người dùng được ghi lại trong cơ sở dữ liệu – tức blockchain. Mọi người (hay chính xác hơn là mọi node) phải duy trì một bản sao cơ sở dữ liệu giống hệt nhau. Nếu không, thông tin sẽ bị xung đột. Từ đó, mạng lưới tiền mã hoá sẽ bị phá vỡ.
Mật mã khóa công khai đảm bảo rằng người dùng không thể tiêu tiền của nhau. Nhưng vẫn cần phải có một nguồn xác thực duy nhất để những người tham gia mạng lưới có thể xác định xem tiền đã được chi chưa.
Satoshi Nakamoto, người tạo ra Bitcoin, đã đề xuất một hệ thống Proof of Work để điều phối hoạt động này. Chúng ta sẽ sớm tìm hiểu cách PoW hoạt động – nhưng trước mắt, chúng ta sẽ tìm hiểu một số đặc điểm chung các thuật toán đồng thuận đang có.

Điểm chung tiên quyết là khi người dùng (trình xác thực) muốn thêm khối, họ phải **stake** một giá trị gì đó. Việc stake một giá trị khiến cho trình xác thực có xu hướng hành động trung thực. Nếu họ gian lận, họ sẽ mất những thứ họ đã stake. Những thứ có thể stake bao gồm sức mạnh tính toán, tiền mã hóa hoặc thậm chí danh tiếng. 

Tại sao người dùng lại muốn mạo hiểm nguồn lực của chính họ? Bởi vì việc này mang đến cho họ cơ hội nhận **phần thưởng**. Phần thưởng thường là tiền mã hóa gốc của giao thức và được tạo thành từ các khoản phí do người dùng khác trả, các đơn vị tiền mã hóa mới được tạo hoặc cả hai.

Điều cuối cùng chúng ta cần là sự **minh bạch**. Chúng ta cần khả năng phát hiện khi ai đó đang gian lận. Lý tưởng nhất là họ phải tốn kém chi phí để sản xuất các khối, nhưng lại rất rẻ để bất kỳ ai muốn xác thực chúng. Điều này đảm bảo rằng các trình xác thực được người dùng thường xuyên kiểm tra.

## Các loại thuật toán đồng thuận

### Proof of Work (PoW)

Proof of Work (PoW) là "tổ tiên" của các loại thuật toán đồng thuận blockchain. Nó được triển khai lần đầu tiên trên Bitcoin, nhưng khái niệm này thực tế đã xuất hiện trước đó. Trong Proof of Work, trình xác thực (được gọi là thợ đào ) băm dữ liệu họ muốn thêm cho đến khi họ tạo ra một giải pháp cụ thể.
Chuỗi băm (hash) là một chuỗi ký tự và số ngẫu nhiên được tạo ra khi bạn chạy dữ liệu thông qua một hàm băm. Tuy nhiên, nếu bạn chạy lại cùng một dữ liệu, bạn sẽ luôn nhận được cùng một kết quả. Tuy nhiên, nếu bạn thay đổi dù chỉ một chi tiết, chuỗi băm của bạn sẽ hoàn toàn khác.
Nhìn vào đầu ra, bạn không thể biết thông tin nào đã được đưa vào hàm. Do đó, chúng rất hữu ích để chứng minh rằng bạn đã biết một phần dữ liệu trước một thời điểm nhất định. Bạn có thể cung cấp cho ai đó hàm băm của nó và khi bạn tiết lộ dữ liệu sau đó, người đó có thể chạy nó thông qua hàm để đảm bảo đầu ra giống nhau.

Trong Proof of Work, giao thức đặt ra các điều kiện cho một khối hợp lệ. Chẳng hạn, nó có thể cho rằng chỉ một khối có chuỗi băm bắt đầu bằng 00 mới hợp lệ. Cách duy nhất để thợ đào tạo ra một kết quả phù hợp với sự kết hợp đó là đầu vào brute-force. Họ có thể điều chỉnh một tham số trong dữ liệu của mình để tạo ra một kết quả khác cho mỗi lần đoán, cho đến khi họ có được chuỗi băm phù hợp. 
Với các blockchain lớn, rất khó để tìm được chuỗi băm chính xác. Để cạnh tranh với các thợ đào khác, bạn sẽ cần một kho chứa đầy đủ các thiết bị phần cứng có khả năng chạy hàm băm cực mạnh (như ASIC) để có cơ hội tạo ra một khối hợp lệ.

Khoản tiền mà bạn stake khi đào là chi phí của những chiếc máy này và lượng điện cần thiết để chạy chúng. ASIC là một thiết bị chuyên dụng. Vì vậy, ngoài khai thác tiền mã hóa, chúng không được sử dụng trong các ứng dụng khác. Cách duy nhất để thu lại khoản đầu tư ban đầu của bạn là đào tiền mã hóa, điều này mang lại phần thưởng đáng kể nếu bạn thêm thành công một khối mới vào blockchain.
Việc mạng xác minh rằng bạn đã thực sự tạo đúng khối là điều không cần thiết. Ngay cả khi bạn đã thử hàng nghìn tỷ kết hợp để có được chuỗi băm phù hợp, họ chỉ cần chạy dữ liệu của bạn thông qua một hàm một lần. Nếu dữ liệu của bạn tạo ra một chuỗi băm hợp lệ, nó sẽ được chấp nhận và bạn sẽ nhận được phần thưởng. Nếu không, mạng sẽ từ chối nó, và bạn sẽ lãng phí thời gian và điện năng mà không thu được gì.

### Proof of Stake (PoS)

Trong những ngày đầu của Bitcoin xuất hiện, Proof of Stake (PoS) đã được đề xuất như một giải pháp thay thế cho Proof of Work. Trong hệ thống PoS, không có khái niệm về công cụ đào, phần cứng chuyên dụng hoặc mức tiêu thụ năng lượng lớn. Tất cả những gì bạn cần là một chiếc PC thông thường.
Thực tế thì không phải tất cả. Bạn vẫn cần đầu tư nhiều thứ hơn. Trong PoS, bạn không chi trả quá nhiều tài nguyên bên ngoài (như điện hoặc phần cứng), mà là tài nguyên từ bên trong – tiền mã hóa. Các quy tắc khác nhau với mọi giao thức, nhưng nhìn chung bạn cần có một số tiền tối thiểu để đủ điều kiện stake.
Khi đó, bạn cần khóa tiền của mình trong một chiếc ví (bạn không thể di chuyển tiền của mình khi đang stake). Thông thường, bạn sẽ đồng ý với các trình xác thực khác về những giao dịch nào sẽ đi vào khối tiếp theo. Theo một nghĩa nào đó, bạn đang stake vào một khối có thể được chọn và giao thức sẽ chọn một khối.

Nếu khối của bạn được chọn, bạn sẽ nhận được một tỷ lệ phí giao dịch, tùy thuộc vào số tiền bạn stake. Bạn càng khóa nhiều tiền, bạn càng có thể kiếm được nhiều tiền hơn. Nhưng nếu bạn cố gắng gian lận bằng cách đề xuất các giao dịch không hợp lệ, bạn sẽ mất một phần (hoặc tất cả) phần tài sản mình đã stake. Do đó, chúng ta có một cơ chế tương tự như PoW - hành động trung thực sẽ có lợi hơn hành động không trung thực.
Nhìni chung, không có tiền mới được tạo ra để làm phần thưởng dành cho các trình xác thực. Do đó, đồng tiền gốc của blockchain phải được phát hành theo một số cách khác. Điều này có thể được thực hiện thông qua phân phối ban đầu (tức là ICO hoặc IEO) hoặc bằng cách khởi chạy giao thức với cơ chế PoW trước khi chuyển đổi sang PoS.

Cho đến nay, Proof of Stake thuần túy chỉ thực sự được triển khai với các loại tiền mã hóa nhỏ. Do đó, không rõ liệu nó có thể phục vụ như một giải pháp thay thế khả thi cho PoW hay không. Về mặt lý thuyết, nó được đánh giá là hiệu quả nhưng thực tế có thể sẽ rất khác. 

Một khi PoS được triển khai trên một mạng lưới với một lượng lớn giá trị, hệ thống sẽ trở thành một sân chơi của lý thuyết trò chơi và các khuyến khích tài chính. Bất kỳ ai có bí quyết “hack” hệ thống PoS chỉ muốn làm như vậy nếu họ có thể thu được lợi ích từ nó – do đó, cách duy nhất để tìm hiểu xem nó có khả thi hay không là trực tiếp sử dụng mạng.

Chúng ta sẽ sớm thấy PoS được thử nghiệm trên quy mô lớn – Casper sẽ được triển khai như một phần của loạt các nâng cấp mạng Ethereum (được gọi chung là Ethereum 2.0).

### Proof of Staked Authority (PoSA)

BSC sử dụng thuật toán **Proof of Staked Authority (PoSA)**, là mô hình kết hợp giữa Poof of Authority và Proof of Stake. Trong hệ thống Binance Smart Chain thì những người xác thực vào mạng là những người đã stake một lượng Binance (BNB) nhất định và sau đó nhận phí giao dịch sau khi xác thực các khối được chấp nhận trên mạng này. 

Binance Chain và Binance Smart Chain có thiết kế hoàn toàn đồng bộ và được tích hợp sẵn khả năng tương tích chuỗi chéo giữa 2 hình thức này. Với BSC lượng tài sản có thể được di chuyển nhanh chóng giữa các blockchain nên sẽ kết hợp được khả năng giao dịch tiền mã hoánhanh chóng của bản gốc với chức năng của hợp đồng thông minh ở bản cải tiến. 

Binance Chain có Token BEP-2 và BEP-8 cũng có thể hoán đổi với token BEP-20 của Smart Chain. Người tạo dApp trên các blockchain khác có thể chuyển EVM sang Binance Smart Chain tương đối dễ dàng nhờ khả năng tương thích. 

BSC sẽ rất hấp dẫn các nhà vận hành dApp khi Ethereum không ngừng phát triển và phí GAS sẽ tăng mặc dù kế hoạch chuyển đổi sang mô hình PoS của Etherum trong bản Ethereum 2.0 có khả năng sẽ làm giảm bớt một số lo ngại về quy mô hiện tại. 