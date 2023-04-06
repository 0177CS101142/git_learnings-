The code starts by defining constants for the number of rows in the coach (NUM_ROWS), the number of seats in each row (NUM_SEATS_PER_ROW), and the number of seats in the last row (LAST_ROW_SEATS).

An initial 2D array called $coach is created to represent the coach, with all seats initially set to 0 to indicate they are available.

The displayCoach() function is defined to display the current layout of the coach, showing which seats are available and which are booked.

The bookSeats($numSeats) function is defined to book a specified number of seats. It first checks if the input number of seats is valid (i.e., greater than 0 and less than or equal to the number of seats per row). If not, an error message is displayed.

The function then iterates through the coach to find consecutive available seats in a row. If found, the seats are booked by setting the corresponding values in the $coach array to 1 to indicate they are booked, and a success message is displayed.

If consecutive available seats are not found, the function then iterates through the coach again to find nearby available seats. If found, the seats are booked, and a success message is displayed.

If no nearby available seats are found, a failure message is displayed.

The displayCoach() function is called initially to display the initial layout of the coach.

The code enters a while loop that continuously prompts the user to enter the number of seats to book. If the input is 0, the loop breaks and the program ends. Otherwise, the bookSeats() function is called with the user's input as the number of seats to book.
