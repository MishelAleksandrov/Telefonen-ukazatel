# Telefonen-ukazatel
Telefonen Ukazatel
ukazatel = []

while True:
    print('1,search phone')
    print('2,add phone')
    print('3,delete phone')
    print('4,all phones')
    print('5,exit')
    choise = input('what do you want to do')

    if choise == '1':
        name = input('enter name: ')
        if name in ukazatel:
            print(ukazatel[name])
        else:
            print('no such name')
    elif choise == '2':
        name = input('enter name: ')
        number = input('enter phone number: ')
        if name in ukazatel:
            print('Ima takova ime')
    elif choise == '3':
        name = input('enter name: ')
        del(ukazatel)
    elif choise == '4':
        print(ukazatel)
    elif choise == '5':
        break
    else:
        print('Invalid choise. Try again')
