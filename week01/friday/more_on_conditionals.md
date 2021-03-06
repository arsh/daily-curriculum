More About Conditionals and Flow Control
=======================

In the calculator project, we talked about conditionals

```ruby
if 1 > 0
  # do something
else
  # do something different
end
```
Comparisons
===========

- >
- <
- ==
- \>=
- <=
- !=


Compound Conditions
===================

Comparison expressions are often combined:

+ **OR** or **||**
+ **AND** or **&&**

```ruby
if command == "add"
  # add numbers
elsif command == "+"
  # also adds numbers
end
```

```ruby
if command == "add" || command == "+"
  # adds numbers
elsif command == "subtract" || command == "-"
  # subtract the numbers
end
```

Wait a ```while```
=============

```ruby
command = gets.chomp

while command != "add" && command != "+"
  puts "Please tell me to add (+)!"
  command = gets.chomp
end

puts "OMG It's about time!"
```


Make it clearer by using ```Until```
==================

```ruby
command = gets.chomp

until command == "add" || command == "+" || command == "subtract" || command == "-"
  puts "Please tell me to add (+) or subtract (-)!"
  command = gets.chomp
end

puts "OMG It's about time!"
```

Make it clearer by using `include?`

```ruby
command = gets.chomp

until ["add", "+", "subtract", "-"].include? command
  puts "Please tell me to add (+) or subtract (-)!"
  command = gets.chomp
end

puts "OMG It's about time!"
```

case/when
==================

```ruby
if command == "add" || command == "+"
  # adds numbers
elsif command == "subtract" || command == "-"
  # subtract the numbers
elsif command == "multiply" || command == "*"
  # multiply the numbers
elsif command == "divide" || command == "/"
  # divide the numbers
elsif command == "exponify" || command == "**"
  # exponify the number
elsif command == "sqrt"
  # find the square root of the number
end
```

case/when
==================

```ruby
case command
when "add", "+"
  # adds numbers
when "subtract", "-"
  # subtract the numbers
when "multiply", "*"
  # multiply the numbers
when "divide", "/"
  # divide the numbers
when "exponify", "**"
  # exponify the number
when "sqrt"
  # find the square root of the number
end
```

Ranges
======

```ruby
(1..10).each { |number| puts number }
('a'..'z').each { |letter| puts letter }
```

What would this do?

```ruby
first = 10
last = 20
(first..last).each { |number| puts number }
```
