def right ():
    turn_left()
    turn_left()
    turn_left()
    
while not at_goal():
    
    if wall_in_front() and wall_on_right():
        turn_left()
    if wall_in_front() and right_is_clear():
        right()

    if front_is_clear():
        move()   
    
    if front_is_clear()and right_is_clear():
        right() or move()
        
