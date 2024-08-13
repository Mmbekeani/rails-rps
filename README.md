conditions = {
  "Rock": "Scissors",
  "Paper": "Rock",
  "Scissors": "Paper"
}

puts "Rock, Paper or Scissors"
choice = gets.chomp.capitalize
cchoice = conditions.keys.sample
puts "Computer chose #{ cchoice }"
  
if conditions[choice] == cchoice
  puts "You won!"
elsif cchoice == choice
  puts "Its a draw."
elsif conditions[cchoice] == choice
  puts "You lost."
else
  puts "#{choice} is not a valid option"
end
