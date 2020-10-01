list_of_numbers = []  # тут хранятся введеные числа и символы операций


def calculation():
    # Метод pop удаляет последний элемент списка и возвращает его
    second_number = int(list_of_numbers.pop())  # Второе число будет записано первым,
                                                # тогда вычитание работает корректно
    math_symbol = list_of_numbers.pop() # Между вводами чисел, появится символ мат.действия
    first_number = int(list_of_numbers.pop())
    result = 0
    if math_symbol == "+":
        result = first_number + second_number
    elif math_symbol == "-":
        result = first_number - second_number
    elif math_symbol == "*":
        result = first_number * second_number
    elif math_symbol == "/":
        result = first_number / second_number
    elif math_symbol == "^":
        result = first_number ** second_number
    #elif math_symbol == "sqrt":             корень пока не придумал
        #result = first_number ** 1/2
    return(result)


while True:
    # консольная версия исполняется в бесконечном цикле, ввод букв вместо цифр даст ошибку
    new_value = input("First number : ")
    while new_value == "":  # этот цикл проверяет что пустая строка не передастся в список
        print("Type a number")
        new_value = input("First number : ")
    list_of_numbers.append(new_value)

    new_value = input("Operation symbol (+,-,*,/,^) : ")
    while new_value == "":
        print("Type an operator")
        new_value = input("Operation symbol (+,-,*,/,^) : ")
    list_of_numbers.append(new_value)

    new_value = input("Second number : ")
    while new_value == "":
        print("Type a number")
        new_value = input("Second number : ")
    list_of_numbers.append(new_value)

    print(calculation())
