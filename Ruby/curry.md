## Curry
Learned a new concept called currying in ruby where we can pass partial arguments to a function.
Example : 

	multiply = Proc.new{|x,y| x * y}
	double = multiply.curry.(2) # .(2) is syntactic sugar for .call(2)
	double.(4) # => 8

Refer https://ruby-doc.org/core-1.9.3/Proc.html#method-i-curry
