# Winter-arc-2026
Code n code
10/1/2026 Tui bắt đầu học code lại với mục tiêu là có thể tiếp cận với các bài leetcode hoặc codeforces tốt nhất, bên cạnh đó cũng muốn hiểu rõ bản chân hơn về ngôn ngữ thay vì lạm dụng AI quá mức. Thừa nhận có dùng AI nhưng chủ yếu ở lúc bí còn lại là tự code :V
Hôm nay học tiếp class & object trên freecodecamp cảm giác lâu không code nó không làm suy giảm hay quên kiến thức code của tui mà tui cảm thấy mình có cách nhìn khác hơn nhờ học hỏi 1 người bạn học cùng lớp ở đại học ( ổng học C++ ) tui đang học python
Đây là bài tui làm hôm nay ( nhánh bài tập trong tiến độ học python )

class Planet:
    def __init__(self, name, planet_type, star):
        if not isinstance(name, str) or not isinstance(planet_type, str) or not isinstance(star, str):
            raise TypeError("name, planet type, and star must be strings")
        if name == "" or planet_type == "" or star == "":
            raise ValueError("name, planet_type, and star must be non-empty strings")
            
        self.name = name
        self.planet_type = planet_type
        self.star = star

    def orbit(self):
        return f"{self.name} is orbiting around {self.star}..."

    def __str__(self):
        return f"Planet: {self.name} | Type: {self.planet_type} | Star: {self.star}"

planet_1 = Planet("Earth", "Terrestrial", "Sun")
planet_2 = Planet("Jupiter", "Gas Giant", "Sun")
planet_3 = Planet("Kepler-22b", "Exoplanet", "Kepler-22")

print(planet_1)
print(planet_1.orbit())

print(planet_2)
print(planet_2.orbit())

print(planet_3)
print(planet_3.orbit())

----2/10/2026 ----
Tui làm challenges trên codédex. Thật ra là luyện bài tập và củng cố kiến thức bài cũng không thức sự khó lém
earth_weight = float(input('Enter your weight: '))
planet = int(input('Enter the planet number: '))
destination_weight = earth_weight * 0.38
if planet == 1:
  destination_weight = earth_weight * 0.38
  print(destination_weight)
elif planet == 2:
  destination_weight = earth_weight * 0.91
  print(destination_weight)
elif planet == 3:
  destination_weight = earth_weight * 0.38 
  print(destination_weight)
elif planet == 4:
  destination_weight = earth_weight * 2.53
  print(destination_weight)
elif planet == 5:
  destination_weight = earth_weight * 1.07
  print(destination_weight)
elif planet == 6:
  destination_weight = earth_weight * 0.89
  print(destination_weight)
elif planet == 7:
  destination_weight = earth_weight * 1.14
  print(destination_weight)
else:
  print('Invalid number')

--4/10/2026--- Hôm qua học lý thuyết nên không có up bài. Hôm nay tui làm được 1 chút xíu code về class và object cụ thể là tới step 16 trong freecodecamp ( Build an Email Simulator )
class Email:
    def __init__(self, sender, receiver, subject, body):
        self.sender = sender
        self.receiver = receiver
        self.subject = subject
        self.body = body
        self.read = False

    def mark_as_read(self):
        self.read = True

class User:
    def __init__(self, name):
        self.name = name
        self.inbox = Inbox()
        
    def send_email(self, receiver, subject, body):
        email = Email(sender=self, receiver=receiver, subject=subject, body=body)
    def receive_email        

class Inbox:
    def __init__(self):
        self.emails = []

    def receive_email(self, email):
        self.emails.append(email)
