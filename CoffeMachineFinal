class CoffeMachine:
    def __init__(self, Water = 400, Milk = 540, Coffee = 120, Disposable_cups = 9, Money = 550):
        self.Water = Water
        self.Milk = Milk
        self.Coffee = Coffee
        self.Disposable_cups = Disposable_cups
        self.Money = Money

    def take(self):
        print("I gave you $" + str(self.Money))
        self.Money = self.Money - self.Money

    def filling(self):
        New_Water = int(input("Write how many ml of water do you want to add: "))
        self.Water = self.Water + New_Water
        New_Milk = int(input("Write how many ml of milk do you want to add: "))
        self.Milk = self.Milk + New_Milk
        New_Coffee = int(input("Write how many grams of coffee beans do you want to add: "))
        self.Coffee = self.Coffee + New_Coffee
        New_Cups = int(input("Write how many disposable cups of coffee do you want to add: "))
        self.Disposable_cups = self.Disposable_cups + New_Cups

    def remaining(self):
        print(f"""The coffee machine has:
        {self.Water} of water
        {self.Milk} of milk
        {self.Coffee} of coffee beans
        {self.Disposable_cups} of disposable cups
        ${self.Money} of money""")
        
        
    def buy(self):
        buy = (input("What do you want to buy? 1 - espresso, 2 - latte, 3 - cappuccino, back - to main menu: ")).lower()
        
        if buy == "1":
            if self.Water < 250:
                print("Sorry, not enough water!")
            elif self.Coffee < 16:
                print("Sorry, not enough coffee beans!")
            elif self.Disposable_cups < 1:
                print("Sorry, not enough disposable cups!")
            else:
                print("I have enough resources, making you a coffee!")
                self.Water = self.Water - 250
                self.Coffee = self.Coffee - 16
                self.Disposable_cups = self.Disposable_cups - 1
                self.Money = self.Money + 4
        elif buy == "2":
            if self.Water < 350:
                print("Sorry, not enough water!")
            elif self.Milk < 75:
                print("Sorry, not enough milk!")
            elif self.Coffee < 20:
                print("Sorry, not enough coffee beans!")
            elif self.Disposable_cups < 1:
                print("Sorry, not enough disposable cups")
            else:
                print("I have enough resources, making you a coffee!")
                self.Water = self.Water - 350
                self.Milk = self.Milk - 75
                self.Coffee = self.Coffee - 20
                self.Disposable_cups = self.Disposable_cups - 1
                self.Money = self.Money + 7
        elif buy == "3":
            if self.Water < 200:
                print("Sorry, not enough water!")
            elif self.Milk < 100:
                print("Sorry, not enough milk!")
            elif self.Coffee < 12:
                print("Sorry, not enough coffee beans!")
            elif self.Disposable_cups < 1:
                print("Sorry, not enough disposable cups")
            else:
                print("I have enough resources, making you a coffee!")
                self.Water = self.Water - 200
                self.Milk = self.Milk - 100
                self.Coffee = self.Coffee - 12
                self.Disposable_cups = self.Disposable_cups - 1
                self.Money = self.Money + 6
        elif buy == "back":
            print("")
            
    def machine_actions(self):
        while True:
            user_input = str(input("Write action (buy, fill, take, remaining, exit): ")).lower()
            if (user_input == "buy"):
                self.buy()
            elif (user_input == "fill"):
                self.filling()
            elif (user_input == "take"):
                self.take()
            elif (user_input == "remaining"):
                self.remaining()
            elif (user_input == "exit"):
                break
start = CoffeMachine()
start.machine_actions()
 
