# ASSEMBLY
Örnek olarak helloas isimli assembly program dosyamızı derlememiz ve çalıştırmamız için önce linux dağıtımımızda nasm derleyicisini kullanarak bir object dosyası oluşturuyoruz.
Daha sonra oluşturduğumuz object dosyasını bir bağlayıcı vasıtası ile çalıştırılabilir dosya haline getirip çalıştırıyoruz.(linux tabanlı sistemlerde çalıştırılabilir dosya formatı elftir.)  





root@b3kc4t:~#nasm -f elf hello.asm


root@b3kc4t:~#ld -m elf_i386 -s -o hello helloas.o


root@b3kc4t:~#./hello
