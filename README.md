# Random-Password-Generator
#It's generate random password

#Here is the code

lower="abcdefghijklmnopqrstuvwxyz". split(//)

upper ="ABCDEFGHIJKLMNOPQRSTUVWXYZ".split(//)

num ="0123456789". split(//)

sym ="@#_&-+()/*:;!?£¢€^{}∆~¶¥{®{™¥™[¢}€¶¥{". split (//)

mix = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ01234567@#_&-+()/*:;!?£¢€¥^°=\%©®™✓". split(//)

password = ""

puts "Enter what type of password you need : "

passwordtype = gets.chomp

puts "How much longer password you need : "

passwordlenght = gets.chomp.to_i

passwordlenght -=1

while passwordtype == "lower" and passwordlenght >0

password += lower.sample

  passwordlenght-=1

end

while passwordtype == "upper" and passwordlenght >0

password += upper.sample

  passwordlenght-=1

end

while passwordtype == "num" and passwordlenght >0

password += num.sample

  passwordlenght-=1

end

while passwordtype == "sym" and passwordlenght >0

password += sym.sample

  passwordlenght-=1

end

while passwordtype == "mix" and passwordlenght >0

password += mix.sample

  passwordlenght-=1

end

puts "Your new password is "+  password









