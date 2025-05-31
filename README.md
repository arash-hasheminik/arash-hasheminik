- 👋 Hi, I’m @arash-hasheminik
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!-class CircularQueue:
    def __init__(self, size):
        self.size = size
        self.queue = [None] * size
        self.front = self.rear = -1
        self.logs = []

    def enqueue(self, data):
        if (self.rear + 1) % self.size == self.front:
            print("صف پر است")
            return

        if self.front == -1:
            self.front = 0
        self.rear = (self.rear + 1) % self.size
        self.queue[self.rear] = data
        self.logs.append(data)

    def dequeue(self):
        if self.front == -1:
            print("صف خالی است")
            return None

        removed = self.queue[self.front]
        self.queue[self.front] = None

        if self.front == self.rear:
            self.front = self.rear = -1
        else:
            self.front = (self.front + 1) % self.size

        return removed

    def show_valid(self):
        if self.front == -1:
            print("[]")
            return
        i = self.front
        valid = []
        while True:
            valid.append(self.queue[i])
            if i == self.rear:
                break
            i = (i + 1) % self.size
        print("داده‌های معتبر:", valid)

    def show_invalid(self):
        invalid = []
        for i in range(self.size):
            if self.queue[i] is None:
                invalid.append(i)
        print("اندیس‌های خانه‌های نامعتبر:", invalid)

    def show_last_logs(self, n=3):
        print("آخرین لاگ‌ها:", self.logs[-n:])

    def to_linear_queue(self):
        linear = []
        if self.front == -1:
            return linear
        i = self.front
        while True:
            linear.append(self.queue[i])
            if i == self.rear:
                break
            i = (i + 1) % self.size
        print("صف خطی:", linear)
        return linear
--
arash-hasheminik/arash-hasheminik is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
