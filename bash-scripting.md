#### expect
    #!/usr/bin/expect

    set timeout 1
    spawn sudo -i
    expect "*password*"
    send "password\r";
    expect "*root*"
    send "echo \"nameserver 8.8.8.8\" > /etc/resolv.conf\r"
    expect "*root*"

    send "exit\r"
    expect "*$*"
    
#### .bash_alias
    alias qwertyu='expect /home/l50/Application/expect/change_dns && exit'
