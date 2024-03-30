from turtle import*
color('red')
begin_fill()
pensize(10)
left(50)
forward(133)
circle(50,200)
right(140)
circle(50,200)
forward(133)
end_fill# Import turtle package 
import turtle 

# Creating a turtle object(pen) 
pen = turtle.Turtle() 

# Defining a method to draw curve 
def curve(): 
	for i in range(200): 

		# Defining step by step curve motion 
		pen.right(1) 
		pen.forward(1) 

# Defining method to draw a full heart 
def heart(): 

	# Set the fill color to a faded pink
	pen.fillcolor('antiquewhite') 

	# Start filling the color 
	pen.begin_fill() 

	# Draw the left line 
	pen.left(140) 
	pen.forward(113) 

	# Draw the left curve 
	curve() 
	pen.left(120) 

	# Draw the right curve 
	curve() 

	# Draw the right line 
	pen.forward(112) 

	# Ending the filling of the color 
	pen.end_fill() 

# Defining method to write text 
def txt(): 

	# Move turtle to air 
	pen.up() 

	# Move turtle to a given position 
	pen.setpos(-68, 95) 

	# Move the turtle to the ground 
	pen.down() 

	# Set the text color to red (may look like maroon with pink backdrop)
	pen.color('red') 

	# Write the specified text in 
	# specified font style and size...make it cuteee!!!
	pen.write("I love you<33", font=( 
	"Times New Roman", 12, "bold")) 


# Draw a heart 
heart() 

# Write text 
txt() 

# To hide turtle 
pen.ht() 
