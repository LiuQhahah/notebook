 
- echo 输出空字符＋空行
- echo -n 输出空字符不加空行＝＝什么都不输出
- echo -e 能够识别以\开头的一些特殊字符,转义字符

 - Print a text message. Note: quotes are optional:
   echo "{{Hello World}}"

 - Print a message with environment variables:
   echo "{{My path is $PATH}}"

 - Print a message without the trailing newline:
   echo -n "{{Hello World}}"

 - Append a message to the file:
   echo "{{Hello World}}" >> {{file.txt}}

 - Enable interpretation of backslash escapes (special characters) 开启反斜杠转义 :
   echo -e "{{Column 1\tColumn 2}}"