*   boot partition space not enough

        dpkg --get-selection | grep linux-image         //see installed linux kernel
        uname -a                                        // look linux image is using
        sudo apt-get purge linux-image....              // delete old linux image
        sudo apt-get purge linux-headers...             // delete old linux header
