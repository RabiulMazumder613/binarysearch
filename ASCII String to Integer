s = "11aa32bbb5"

def solve(s):

	# Temporary string to get multiple consecutive digits so that they are 
	# considered as one number.
	temp = "0"

	# gets the sum of all numbers in the s string
	total = 0

	# read each character in the input string
	for i in s:

		# if the current character is a digit add it to temp
		if i.isdigit():
			temp += i

		# when the character is an alphabet this is how the program knows that
		# is the end of the consecutive digits that'll be considered one numer
		# like it see's 1 and 1 at the beginning of "11aa32bbb5" 
		# but will put it together to be 11 once it reads a
		else:
			# now we have the one number convert it to an int and add it to total
			total += int(temp)
			# reset temp so we can continue the process over again to get 32 for this example
			# but if it was loner it would get more numbers
			temp = "0"
	# we need to add temp as it is holding 5 and it doesn't have a alphabet after it
	# to go to the else statement which is used to know when we got the whole number
	return total + int(temp)

print(solve(s))
