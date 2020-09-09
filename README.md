# circle_calculations
#this program allows you to calculate the area or the circumference if the radius is given or also the vice-versa
import math
print('hi i am python and can solve the find the circumference or area for you')
area_or_circumference = input('area or circuference or radius: ')
if area_or_circumference.upper() == 'AREA':
    radius = int(input('whats the radius of your circle? '))
    print('the area of your circle is: ')
    print(2*math.pi*radius**2)
elif area_or_circumference.upper() == 'CIRCUMFERENCE':
    radius = int(input('whats the radius of your circle? '))
    print('the circumference of your circle is: ')
    print(2 * math.pi * radius )
elif area_or_circumference.upper() == 'RADIUS':
        area_or_circumference_new = input("please enter 'circumference' or 'area' : ")
        if area_or_circumference_new.upper() == 'CIRCUMFERENCE':
            circumference = int(input('circumference of the circle: '))
            print(circumference/(2*math.pi))
        elif area_or_circumference_new.upper() == 'AREA':
            area = int(input('area of the circle: '))
            print(math.sqrt((area/(2*math.pi))))
        else:
            print('please enter circumference or area only!!')
            area_or_circumference_new = input("please enter 'circumference' or 'area' : ")
else:
    print('i dont understand!! please enter things from one of these two:')
    print(" 'area' or 'circumference' or 'radius' ")





