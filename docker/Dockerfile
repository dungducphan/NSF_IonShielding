FROM ddp822/pps:0.1

RUN mkdir -p ~/IonShield/build; \
    cd ~/IonShield; \
    git clone https://github.com/dungducphan/NSF_IonShielding.git
RUN cd ~/IonShield/build; \
    cmake ../NSF_IonShielding; \
    make -j `grep -c processor /proc/cpuinfo`