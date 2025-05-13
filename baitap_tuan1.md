1. Mong muốn và định hướng của bạn là gì sau khi học xong môn học?
Sau khi học xong môn học, mình mong muốn có thể nắm vững kiến thức cơ bản về phát triển ứng dụng di động, đặc biệt là về thiết kế giao diện người dùng (UI) và xử lý logic phía client. Định hướng của mình là phát triển kỹ năng chuyên sâu hơn trong lĩnh vực lập trình mobile, đặc biệt là sử dụng Flutter hoặc React Native để phát triển ứng dụng đa nền tảng. Mục tiêu cuối cùng là có thể tự phát triển các ứng dụng hữu ích, phục vụ nhu cầu thực tế hoặc làm việc trong một công ty công nghệ chuyên về mobile app.

2. Theo bạn, trong tương lai gần (10 năm) lập trình di động có phát triển không? Giải thích tại sao?
Theo mình, lập trình di động sẽ tiếp tục phát triển mạnh trong 10 năm tới. Lý do là vì:

Số lượng người dùng smartphone ngày càng tăng trên toàn thế giới.

Nhu cầu sử dụng các ứng dụng mobile trong đời sống hằng ngày (mua sắm, học tập, giải trí, chăm sóc sức khỏe, v.v.) ngày càng nhiều.

Sự phát triển của công nghệ mới như 5G, AI tích hợp vào ứng dụng di động sẽ mở ra nhiều cơ hội mới cho lập trình viên.

Doanh nghiệp ngày càng ưu tiên phát triển ứng dụng mobile để tiếp cận khách hàng nhanh hơn, tiện lợi hơn.

3. Viết một ứng dụng có UI như sau và đẩy lên GitHub:
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      home: UserProfileScreen(),
    );
  }
}

class UserProfileScreen extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('User Profile'),
        backgroundColor: Colors.blue,
      ),
      body: Center(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: [
            CircleAvatar(
              radius: 50,
              backgroundImage: AssetImage('assets/profile.jpg'), // Thay bằng đường dẫn ảnh
            ),
            SizedBox(height: 10),
            Text(
              'Johan Smith',
              style: TextStyle(fontSize: 22, fontWeight: FontWeight.bold),
            ),
            Text(
              'California, USA',
              style: TextStyle(fontSize: 18, color: Colors.grey),
            ),
            SizedBox(height: 20),
            ElevatedButton(
              onPressed: () {
                // Thêm chức năng cần thiết
              },
              child: Text('Edit Profile'),
            ),
          ],
        ),
      ),
    );
  }
}


