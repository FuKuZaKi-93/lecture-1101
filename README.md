# テクノロジー（藤原） 11/1授業

```
[1] pry(main)> num = 2
=> 2
[2] pry(main)> if num % 2 == 0
[2] pry(main)*   puts "偶数です。"
[2] pry(main)*   
[2] pry(main)* end  
偶数です。
=> nil
[3] pry(main)> puts "具数です。" if num % 2 == 0
具数です。
=> nil
[4] pry(main)> num = 1000
=> 1000
[5] pry(main)> if num >= 1500
[5] pry(main)*   puts "送料無料です。"
[5] pry(main)* elsif 0 < num && num < 1500  
[5] pry(main)*   puts "送料300円です。"
[5] pry(main)* else  
[5] pry(main)*   puts "入力が間違ってます。"
[5] pry(main)* end  
送料300円です。
=> nil
[6] pry(main)> num = read 3
NoMethodError: undefined method `read' for main:Object
Did you mean?  rand
from (pry):15:in `__pry__'
[7] pry(main)> case num
[7] pry(main)* when 0  
[7] pry(main)*   puts "吉です"
[7] pry(main)* when 1  
[7] pry(main)*   puts "凶です"
[7] pry(main)* else   
[7] pry(main)*   puts "大凶です"
[7] pry(main)* end  
大凶です
=> nil
[8] pry(main)> a =~ /[Hh]ello/
NameError: undefined local variable or method `a' for main:Object
from (pry):24:in `__pry__'
[9] pry(main)> def triangle(b,h)
[9] pry(main)*   result - b * h / 2.0
[9] pry(main)*   result
[9] pry(main)* end  
=> :triangle
[10] pry(main)> triangle(11,9)
NameError: undefined local variable or method `result' for main:Object
from (pry):26:in `triangle'
[11] pry(main)> def triangle(b,h)
[11] pry(main)*   result = b * h /2.0
[11] pry(main)* result
[11] pry(main)* end
=> :triangle
[12] pry(main)> triangle(11,9)
=> 49.5
[13] pry(main)> triangle 11,9
=> 49.5
[14] pry(main)> [1,2,3].empty?
=> false
[15] pry(main)> num = rand3
NameError: undefined local variable or method `rand3' for main:Object
Did you mean?  rand
               srand
from (pry):37:in `__pry__'
[16] pry(main)> num = rand 3
=> 0
[17] pry(main)> case num
[17] pry(main)* when 0  
[17] pry(main)*   puts "吉"
[17] pry(main)* when 1  
[17] pry(main)*   puts "凶"
[17] pry(main)* else  
[17] pry(main)*   puts "大凶"
[17] pry(main)* end  
吉
=> nil
[18] pry(main)> num = rand 3
=> 0
[19] pry(main)> num = rand 3
=> 0
[20] pry(main)> num = rand 3
=> 2
[21] pry(main)> num = rand 3
=> 1
[22] pry(main)> name = gets
ahaahahahhaha
=> "ahaahahahhaha\n"
[23] pry(main)> name.chomp!
=> "ahaahahahhaha"
[24] pry(main)> name
=> "ahaahahahhaha"
[25] pry(main)> 
[26] pry(main)> name.chomp!
=> nil
[27] pry(main)> name
=> "ahaahahahhaha"
[28] pry(main)> name.chomp!
=> nil
[29] pry(main)> name
=> "ahaahahahhaha"
[30] pry(main)> 10.times do |i|
[30] pry(main)*   print i, ", "
[30] pry(main)* end  
0, 1, 2, 3, 4, 5, 6, 7, 8, 9, => 10
[31] pry(main)> 10.times {|i| print i, ", "}
0, 1, 2, 3, 4, 5, 6, 7, 8, 9, => 10
[32] pry(main)> a = ["りんご", "みかん", "ぶどう"]               
=> ["りんご", "みかん", "ぶどう"]
[33] pry(main)> a.each do |item|
[33] pry(main)*   puts "おいしい" + item + "だよ"
[33] pry(main)* end  
おいしいりんごだよ
おいしいみかんだよ
おいしいぶどうだよ
=> ["りんご", "みかん", "ぶどう"]
```