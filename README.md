erbhomework
===========

irb
require 'erb'

x = 42
template = ERB.new "The value of x is: <%= x %>"
puts template.result(binding)

instrument = "guitar"
puts instrument
"guitar"
puts "play" + instrument + "play"

Array#each
instruments = ['piano', 'violin', 'guitar']
instruments.each do |instrument|
  puts "I play #{instrument}"
	end

puts instruments
['piano', 'violin', 'guitar']


name = 'Gonzo'
erb_string = "<h2><%= name.upcase %></h2>"

template = ERB.new(erb_string)
puts template.result(binding)
# => <h2>GONZO</h2>