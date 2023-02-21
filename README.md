# HW18.8.19

cost = 0
number_of_tickets = int(input('Сколько билетов желаете приобрести: '))
for i in range(number_of_tickets):
    i += 1
    age_by_ticket = int(input(f'Укажите возраст посетителя по {i} билету: '))
    if age_by_ticket < 18:
            print('К оплате - 0 руб.')
    elif 18 <= age_by_ticket < 25:
            cost += 990
            print('К оплате - 990 руб.')
    else:
            cost += 1390
            print('К оплате - 1390 руб.')
if number_of_tickets > 3:
    total_cost = cost - ((cost / 100) * 10)
    print(f'Сумма к оплате - {total_cost} руб. (с учетом скидки 10%)')
else:
    print(f'Сумма к оплате - {cost} руб.')
