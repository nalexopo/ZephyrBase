# virtual env
source ~/zephyrproject/.venv/bin/activate

# To build dual core stm32h755xx
west build -b dual_h755zi_q/stm32h755xx/m7 blinky -DBOARD_ROOT=$(pwd) -p always

OR for m4 core

west build -b dual_h755zi_q/stm32h755xx/m4 blinky -DBOARD_ROOT=$(pwd) -p always


# To build pynqz2
west build -b pynqz2 hello_world -DBOARD_ROOT=$(pwd) -p always