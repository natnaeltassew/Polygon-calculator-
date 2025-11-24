🔷 Shape Calculator – Rectangle & Square Classes (Python)

This project implements two geometric classes — Rectangle and Square — with methods for calculating area, perimeter, diagonal length, ASCII drawings, and spatial fitting.
It follows the specifications of the FreeCodeCamp Shape Calculator project.


---

🚀 Features

✅ Rectangle Class

Supports:

Setting width and height

Computing:

Area

Perimeter

Diagonal


Drawing a visual ASCII picture using *

Checking how many times another shape fits inside it

Clean string representation:
Rectangle(width=10, height=5)



---

✅ Square Class (inherits from Rectangle)

A special type of rectangle with equal sides

Methods:

set_side()

set_width() (overridden)

set_height() (overridden)


String representation:
Square(side=9)



---

📂 File Included

shape_calculator.py – Contains Rectangle and Square implementations.



---

🧠 Key Methods

🔹 Rectangle

Method	Description

set_width(value)	Change rectangle width
set_height(value)	Change rectangle height
get_area()	Returns width × height
get_perimeter()	Returns 2 × (width + height)
get_diagonal()	Returns √(width² + height²)
get_picture()	Returns star-pattern ASCII drawing
get_amount_inside(shape)	Calculates how many times another shape fits



---

🔹 Square

Inherits all rectangle methods and enforces equal sides.

Method	Description

set_side(value)	Update width & height together
set_width(value)	Overridden to keep sides equal
set_height(value)	Overridden to keep sides equal



---

🖼️ Example Usage

from shape_calculator import Rectangle, Square

rect = Rectangle(10, 5)
square = Square(3)

print(rect.get_area())         # 50
print(square.get_perimeter())  # 12

rect.set_height(8)
print(rect)                    # Rectangle(width=10, height=8)

print(rect.get_picture())
# **********
# **********
# **********
# **********
# **********
# **********
# **********
# **********

print(rect.get_amount_inside(square))  # 8


---

⚠️ Picture Size Limit

get_picture() returns:

Too big for picture.

if width > 50 or height > 50
(to prevent extremely large ASCII output).


---

📜 Requirements

Python 3.6 or above



---

🤝 Contributing

Contributions, bug fixes, and enhancements are welcome!
Please open an issue before making major changes.


---

📄 License

This project is open-source and free to use.
