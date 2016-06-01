#PRIVATE - DO NOT USE

##Stuff to remind myself

    make clean && make && sudo make install
    sudo depmod -a

    sudo rmmod b43 ssb bcma
    sudo modprobe wl

    printf 'blacklist b43\nblacklist ssb\nblacklist bcma\n' | sudo tee /etc/modprobe.d/wl.conf
    echo 'wl' | sudo tee /etc/modules-load.d/wl.conf
