```
if choice == 1:
    option = str(input('Enter Booking Type: [Online or Gate]: '))
    if option.lower() == 'online':
        ticket_type = 'LEGOLAND Dubai'
        booking_type = 'Online'
        ticket_price = 295
        staffOrNot = str(input('Are you a staff?: [Staff or Not Staff]: '))
        numberoftickets = int(input('Enter the Number of Tickets: '))
        total_tickets_price = numberoftickets * ticket_price

        print('Ticket')
        print('Ticket Type: {}\nNumber Of Tickets: {}\nBooking Type: {}\nStaff or Not: {} \nTicket Price: {}\nTotal Price: {:.2f}'.format(
            ticket_type, numberoftickets, booking_type, staffOrNot, ticket_price, total_tickets_price))

    elif option.lower() == 'gate':
        ticket_type = 'LEGOLAND Dubai'
        booking_type = 'Gate'
        ticket_price = 330
        staffOrNot = str(input('Are you a staff?: [Staff or Not Staff]: '))
        numberoftickets = int(input('Enter the Number of Tickets: '))
        total_tickets_price = numberoftickets * ticket_price
        if staffOrNot.lower() == 'staff':
            discount = (70/100 * ticket_price)
            total_tickets_pric = numberoftickets * discount
            print('Ticket')
            print('Ticket Type: {}\nNumber Of Tickets: {}\nBooking Type: {}\nStaff or Not: {} \nTicket Price: {}\nTotal Price: {:.2f}'.format(
                ticket_type, numberoftickets, booking_type, staffOrNot, ticket_price, total_tickets_pric))

        elif staffOrNot.lower() == 'not staff':
            total_tickets_price = numberoftickets * ticket_price
            print('Ticket')
            print('Ticket Type: {}\nNumber Of Tickets: {}\nBooking Type: {}\nStaff or Not: {} \nTicket Price: {}\nTotal Price: {:.2f}'.format(
                ticket_type, numberoftickets, booking_type, staffOrNot, ticket_price, total_tickets_price))
                
                ```
