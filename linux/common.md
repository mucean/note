*   boot partition space not enough

    [see detail](http://www.cnblogs.com/rossoneri/p/4017861.html)

        dpkg --get-selection | grep linux-image         //see installed linux kernel
        uname -a                                        // look linux image is using
        sudo apt-get purge linux-image....              // delete old linux image
        sudo apt-get purge linux-headers...             // delete old linux header
