# virtual env
source ~/zephyrproject/.venv/bin/activate

# To build
west build -b dual_h755zi_q/stm32h755xx/m7 blinky -DBOARD_ROOT=$(pwd) -p always

OR

west build -b dual_h755zi_q/stm32h755xx/m4 blinky -DBOARD_ROOT=$(pwd) -p always
