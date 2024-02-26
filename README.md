class Ticket:
    def __init__(self, issue, status="Новый"):
        self.issue = issue
        self.status = status

    def update_status(self, new_status):
        self.status = new_status

    def __str__(self):
        return f"Тикет: {self.issue} (Статус: {self.status})"

# Пример использования класса Ticket
ticket1 = Ticket("Проблема с сетью")
print(ticket1)

ticket1.update_status("В процессе решения")
print(ticket1)
